# Comparing `tmp/twitchify-1.0.5.tar.gz` & `tmp/twitchify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.0.5.tar", last modified: Wed Jun 21 11:45:16 2023, max compression
+gzip compressed data, was "twitchify-1.1.0.tar", last modified: Fri Jun 23 01:21:06 2023, max compression
```

## Comparing `twitchify-1.0.5.tar` & `twitchify-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:45:16.406209 twitchify-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-21 11:45:05.000000 twitchify-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-21 11:45:16.406209 twitchify-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-21 11:45:05.000000 twitchify-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:45:16.406209 twitchify-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-21 11:45:05.000000 twitchify-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:45:16.402209 twitchify-1.0.5/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:45:16.406209 twitchify-1.0.5/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:45:16.406209 twitchify-1.0.5/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-21 11:45:05.000000 twitchify-1.0.5/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:45:16.406209 twitchify-1.0.5/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-21 11:45:16.000000 twitchify-1.0.5/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-21 11:45:16.000000 twitchify-1.0.5/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:45:16.000000 twitchify-1.0.5/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 11:45:16.000000 twitchify-1.0.5/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 11:45:16.000000 twitchify-1.0.5/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.022052 twitchify-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 01:20:48.000000 twitchify-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 01:21:06.022052 twitchify-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 01:20:48.000000 twitchify-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 01:21:06.022052 twitchify-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 01:20:48.000000 twitchify-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.014052 twitchify-1.1.0/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.018052 twitchify-1.1.0/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.018052 twitchify-1.1.0/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.022052 twitchify-1.1.0/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 01:21:06.000000 twitchify-1.1.0/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.0.5/LICENSE` & `twitchify-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/PKG-INFO` & `twitchify-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.0.5/README.md` & `twitchify-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/setup.py` & `twitchify-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from setuptools import setup
 import re
+from setuptools import setup
 
 
 def version() -> str:
-    with open('twitch/__init__.py') as f:
-        text = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
+    with open('twitch/__init__.py', encoding='utf-8') as file:
+        text = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', file.read(),
+                         re.MULTILINE).group(1)
         return text
 
 
 def readme() -> str:
-    with open('README.md') as file:
+    with open('README.md', encoding='utf-8') as file:
         text = file.read()
         return text
 
 
 setup(
     name='twitchify',
     version=version(),
@@ -26,21 +27,21 @@
     project_urls={'Issue tracker': 'https://github.com/mrsnifo/twitchify/issues'},
     long_description=readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=['aiohttp>=3.8.0'],
     license='MIT',
     classifiers=[
-            'Development Status :: 5 - Production/Stable',
-            'License :: OSI Approved :: MIT License',
-            'Intended Audience :: Developers',
-            'Natural Language :: English',
-            'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Topic :: Software Development :: Libraries',
-            'Topic :: Software Development :: Libraries :: Python Modules',
-            'Topic :: Utilities',
-            'Typing :: Typed',
-        ],
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Typing :: Typed',
+    ],
 )
```

### Comparing `twitchify-1.0.5/twitch/__init__.py` & `twitchify-1.1.0/twitch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 __title__ = 'Twitchify'
-__version__ = '1.0.5'
+__version__ = '1.1.0'
 __license__ = 'MIT License'
 __author__ = 'Snifo'
 __email__ = 'Snifo@mail.com'
 __github__ = 'https://github.com/mrsnifo/twitchify'
 
 from .client import Client
```

### Comparing `twitchify-1.0.5/twitch/channel.py` & `twitchify-1.1.0/twitch/channel.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,64 +20,90 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
 from .message import Message
 from .user import User
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import channel as chl
-    from typing import Optional
+    from .types import channel as ch
+    from typing import Optional, List, Union
 
 
 class Category:
     """
     Represents a category for a channel.
+
+    :param channel: The channel data.
     """
     __slots__ = ('id', 'name')
 
-    def __init__(self, channel: chl.Update) -> None:
-        self.id: Optional[str] = channel['category_id']
-        self.name: Optional[str] = channel['category_name']
+    def __init__(self, channel: Union[chl.Update, ch.Channel]) -> None:
+        self.id: Optional[str] = channel.get('category_id') or channel.get('game_id')
+        self.name: Optional[str] = channel['category_name'] or channel.get('game_name')
+
+    def __repr__(self):
+        return f'Category id={self.id} name={self.name}'
 
 
 class Channel:
     """
     Represents a channel.
+
+    :param channel: The channel data.
     """
-    __slots__ = ('title', 'language', '_category', 'is_mature')
+    __slots__ = ('title', 'description', 'delay', 'tags', 'category')
+
+    def __init__(self, channel: ch.Channel):
+        self.description: Optional[str] = None
+        self.title: Optional[str] = channel['title']
+        self.delay: int = channel['delay']
+        self.tags: List[str] = channel['tags']
+        # Category.
+        _c = Category(channel=channel) if channel['game_id'] != '' else None
+        self.category: Optional[Category] = _c
+
+    def __repr__(self) -> str:
+        return f'<Channel title={self.title} description={self.description}>'
+
+
+# -------------------------------------------
+#                  EventSub
+# -------------------------------------------
+
+class Update:
+    """
+    Represents when a channel updates their information.
+
+    :param channel: The channel update data.
+    """
+    __slots__ = ('title', 'language', 'is_mature', 'category')
 
     def __init__(self, channel: chl.Update) -> None:
         self.title: str = channel['title']
         self.language: str = channel['language']
-        self._category: Category = Category(channel=channel)
         self.is_mature: bool = channel['is_mature']
+        # Category.
+        _c = Category(channel=channel) if channel['category_id'] != '' else None
+        self.category: Optional[Category] = _c
 
     def __repr__(self) -> str:
-        return f'<Channel title={self.title} language={self.language}>'
-
-    @property
-    def category(self) -> Optional[Category]:
-        """
-        Retrieves the category of the channel.
-        """
-        if self._category.id:
-            return self._category
-        else:
-            return None
+        return f'<Update title={self.title} language={self.language}>'
 
 
 class Subscription:
     """
     Represents a channel subscription.
+
+    :param channel: The subscription data.
     """
     __slots__ = ('user', 'tier', 'is_gift')
 
     def __init__(self, *, channel: chl.Subscribe | chl.SubscriptionEnd) -> None:
         self.user: User = User(user=channel)
         self.tier: str = channel['tier']
         self.is_gift: bool = channel['is_gift']
@@ -85,14 +111,16 @@
     def __repr__(self) -> str:
         return f'<Subscription {super().__repr__()} tier={self.tier} is_gift={self.is_gift}>'
 
 
 class SubscriptionGift:
     """
     Represents a channel subscription gift.
+
+    :param channel: The subscription gift data.
     """
     __slots__ = ('user', 'tier', 'total', 'cumulative_total', 'is_anonymous')
 
     def __init__(self, channel: chl.SubscriptionGift) -> None:
         self.user: User = User(user=channel)
         self.tier: str = channel['tier']
         self.total: int = channel['total']
@@ -102,32 +130,36 @@
     def __repr__(self) -> str:
         return f'<SubscriptionGift tier={self.tier} total={self.total}>'
 
 
 class SubscriptionMessage:
     """
     Represents a channel re-subscription.
+
+    :param channel: The subscription message data.
     """
     __slots__ = ('user', 'tier', 'message', 'cumulative', 'duration', 'streak')
 
     def __init__(self, channel: chl.SubscriptionMessage) -> None:
         self.user: User = User(user=channel)
         self.tier: str = channel['tier']
         self.message: Message = Message(message=channel['message'])
         self.cumulative: int = channel['cumulative_months']
         self.duration: int = channel['duration_months']
         self.streak: Optional[int] = channel['streak_months']
 
     def __repr__(self) -> str:
-        return f'<SubscriptionMessage tier={self.tier} duration={self.duration} message={self.message.__repr__()}>'
+        return f'<SubscriptionMessage tier={self.tier} message={self.message.__repr__()}>'
 
 
 class Cheer:
     """
     Represents a channel cheer.
+
+    :param channel: The cheer data.
     """
     __slots__ = ('user', 'bits', 'message', 'is_anonymous')
 
     def __init__(self, channel: chl.Cheer) -> None:
         self.user: User = User(user=channel)
         self.bits: int = channel['bits']
         self.message: str = channel['message']
@@ -136,17 +168,19 @@
     def __repr__(self) -> str:
         return f'<Cheer bits={self.bits} message={self.message} user={self.user.__repr__()}>'
 
 
 class Raid:
     """
     Represents a channel raid.
+
+    :param raid: The raid data.
     """
     __slots__ = ('from_user', 'to_user', 'viewers')
 
     def __init__(self, raid: chl.Raid) -> None:
         self.from_user: User = User(user=raid, prefix='from_broadcaster_user')
         self.to_user: User = User(user=raid, prefix='to_broadcaster_user')
         self.viewers: int = raid['viewers']
 
     def __repr__(self) -> str:
-        return f'<Raid from_user={self.from_user.__repr__()} to_user={self.to_user.__repr__()} viewers={self.viewers}>'
+        return f'<Raid from_user={self.from_user.__repr__()} to_user={self.to_user.__repr__()}'
```

### Comparing `twitchify-1.0.5/twitch/client.py` & `twitchify-1.1.0/twitch/goals.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,159 +20,221 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
-from .gateway import EventSubWebSocket
-from .state import ConnectionState
-from .utils import setup_logging
-from .http import HTTPClient
-
-# Libraries
-import asyncio
+from .utils import parse_rfc3339_timestamp
+from .user import User
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
-    from typing import Any, List, Optional, Callable
-    from .user import Broadcaster
+    from .types.eventsub import hypertrain as ht
+    from .types.eventsub import charity as ch
+    from typing import Optional, Union, List
+    from .types.eventsub import goal as gl
+    from datetime import datetime
+
+
+class CharityInfo:
+    """
+    Information about a charity.
+
+    :param charity: A dictionary containing charity information.
+    """
+    __slots__ = ('name', 'description', 'logo', 'website')
+
+    def __init__(self, charity: ch.SpecificCharity) -> None:
+        self.name: str = charity['charity_name']
+        self.description: Optional[str] = charity.get('charity_description')  # Beta
+        self.logo: str = charity['charity_logo']
+        self.website: Optional[str] = charity.get('charity_website')  # Beta
+
+    def __repr__(self) -> str:
+        return f'<CharityInfo name={self.name} description={self.description}>'
+
+
+class CharityAmount:
+    """
+    Represents an amount with its value and currency.
+
+    :param amount: A dictionary containing amount information.
+    """
+    __slots__ = ('value', 'currency')
+
+    def __init__(self, amount: ch.Amount) -> None:
+        self.value: float = (amount['value'] / 10 ** amount['decimal_places'])
+        self.currency: str = amount['currency']
+
+    def __repr__(self) -> str:
+        return f'<_Amount value={self.value} currency={self.currency}>'
+
+
+class Charity:
+    """
+    Represents a channel charity.
+
+    :param charity: An object representing a charity.
+    """
+    __slots__ = ('id', 'charity', 'current_amount', 'target_amount', '_started_at', '_stopped_at')
+
+    def __init__(self, charity: Union[ch.Start, ch.Progress, ch.Stop]) -> None:
+        self.id: str = charity['id']
+        self.charity: CharityInfo = CharityInfo(charity=charity)
+        self.current_amount: CharityAmount = CharityAmount(amount=charity['current_amount'])
+        self.target_amount: CharityAmount = CharityAmount(amount=charity['target_amount'])
+        self._started_at: Optional[str] = charity.get('started_at')
+        self._stopped_at: Optional[str] = charity.get('stopped_at')
+
+    @property
+    def started_at(self) -> Optional[datetime]:
+        """The datetime when the charity started."""
+        return parse_rfc3339_timestamp(self._started_at) if self._started_at else None
+
+    @property
+    def stopped_at(self) -> Optional[datetime]:
+        """The datetime when the charity stopped."""
+        return parse_rfc3339_timestamp(self._stopped_at) if self._stopped_at else None
+
+
+class Donation:
+    """
+    Represents a donation made to a charity.
+
+    :param donation: An object representing a donation.
+    """
+    __slots__ = ('id', 'charity', 'user', 'amount')
+
+    def __init__(self, donation: ch.Donation) -> None:
+        self.id: str = donation['id']
+        self.charity: CharityInfo = CharityInfo(charity=donation)
+        self.user: User = User(user=donation)
+        self.amount: CharityAmount = CharityAmount(amount=donation['amount'])
+
+    def __repr__(self) -> str:
+        return f'<Donation id={self.id} user={self.user.__repr__()}>'
+
+
+class _GoalAmount:
+    """
+    Represents the amount and type of goal.
+
+    :param goal: A dictionary containing goal information.
+    """
+
+    def __init__(self, goal: gl.Goal) -> None:
+        self.value: int = goal['current_amount']
+        self.type: str = goal['type']
+
+    def __repr__(self) -> str:
+        return f'<_GoalAmount value={self.value} type={self.type}>'
+
+
+class Goal:
+    """
+    Represents a channel goal.
+
+    :param goal: An object representing a goal.
+    """
+    __slots__ = ('id', 'description', 'amount', 'started_at', 'is_achieved', '_ended_at')
 
-import logging
-_logger = logging.getLogger(__name__)
+    def __init__(self, goal: Union[gl.Begin, gl.Progress, gl.End]) -> None:
+        self.id: str = goal['id']
+        self.description: str = goal['description']
+        self.amount: _GoalAmount = _GoalAmount(goal=goal)
+        self.started_at: datetime = parse_rfc3339_timestamp(goal['started_at'])
+        self.is_achieved: bool = goal.get('is_achieved') or False
+        self._ended_at: Optional[str] = goal.get('ended_at')
 
+    def __repr__(self) -> str:
+        return f'<Goal id={self.id} amount={self.amount.__repr__()} started_at={self.started_at}>'
+
+    @property
+    def ended_at(self) -> Optional[datetime]:
+        """The datetime when the goal ended."""
+        return parse_rfc3339_timestamp(self._ended_at) if self._ended_at else None
 
-class Client:
+
+class _Contributor:
+    """
+    Hyper train top contributor.
+
+    :param contributor: A dictionary containing contributor information.
+    """
+    __slots__ = ('user', 'type', 'total')
+
+    def __init__(self, contributor: ht.Contributor) -> None:
+        self.user: User = User(user=contributor)
+        self.type: str = contributor['type']
+        self.total: int = contributor['total']
+
+    def __repr__(self) -> str:
+        return f'<_Contributor user={self.user.__repr__()} total={self.total} type={self.type}>'
+
+
+class Train:
+    """
+    Hyper train progress.
     """
-    Represents a Twitch client for interacting with the Twitch API and receiving event notifications.
-
-    :param client_id: The client ID associated with the Twitch application.
-    :param client_secret: The client secret for the Twitch application, if applicable.
-    """
-
-    def __init__(self, client_id: str, client_secret: Optional[str] = None) -> None:
-        self.client_secret = client_secret
-        self.client_id = client_id
-        self.loop: Optional[asyncio.AbstractEventLoop] = None
-        self._connection: ConnectionState = ConnectionState(dispatcher=self.dispatch)
-        self._http = HTTPClient(connection=self._connection, client_id=self.client_id, client_secret=self.client_secret)
-
-    @property
-    def user(self) -> Optional[Broadcaster]:
-        return self._connection.broadcaster
-
-    @property
-    def _sub_events(self) -> List[str]:
-        """Retrieve the names of the subscribed events."""
-        return [attr.replace('on_', '', 1) for attr in dir(self) if attr.startswith('on_')]
-
-    async def _run_event(self, coro: Callable[..., Any], event_name: str, *args: Any, **kwargs: Any) -> None:
-        """
-        Execute the specified event coroutine with the given arguments.
-        """
-        try:
-            await coro(*args, **kwargs)
-        except asyncio.CancelledError:
-            pass
-        except Exception as error:
-            try:
-                await self.on_error(str(error), event_name, args, kwargs)
-            except asyncio.CancelledError:
-                pass
-
-    def dispatch(self, event: str, /, *args: Any, **kwargs: Any) -> asyncio.Task:
-        """
-        Dispatch the specified event with the given arguments.
-        """
-        _logger.debug('Dispatching event %s', event)
-        event_name = "on_" + event
-        try:
-            coro = self.__getattribute__(event_name)
-        except AttributeError:
-            pass
-        else:
-            wrapped = self._run_event(coro, event_name, *args, **kwargs)
-            # Schedules the task
-            return self.loop.create_task(wrapped, name=f'Twitchify:{event_name}')
-
-    @staticmethod
-    async def on_error(event_name: str, error: str, /, *args: Any, **kwargs: Any) -> None:
-        """
-        The default error handler for events.
-
-        :param event_name: The name of the event where the error occurred.
-        :param error: The error message.
-        :param args: Variable length argument list passed to the event when the error occurred.
-        :param kwargs: Arbitrary keyword arguments passed to the event when the error occurred.
-        """
-        _logger.exception('Ignoring error: %s from %s, args: %s kwargs: %s', error, event_name, args, kwargs)
-
-    def event(self, coro: Callable[..., Any], /):
-        """
-        Decorator to register an event coroutine.
-
-        :param coro: The event coroutine to be registered.
-        :raises TypeError: If the registered event is not a coroutine function.
-        """
-        if not asyncio.iscoroutinefunction(coro):
-            raise TypeError("The registered event must be a coroutine function")
-
-        setattr(self, coro.__name__, coro)
-
-    async def connect(self, access_token: str, refresh_token: Optional[str]) -> None:
-        """
-        Establishes a connection to Twitch services.
-
-        :param access_token: The access token for authentication.
-        :param refresh_token: The refresh token for refreshing the access token, if applicable.
-        """
-        # Setup logger
-        setup_logging()
-        if self.loop is None:
-            self.loop = asyncio.get_running_loop()
-        # Validating the access key and opening a new session.
-        validation = await self._http.open_session(access_token=access_token, refresh_token=refresh_token)
-        # Retrieving the client.
-        self._connection.broadcaster = await self._http.get_client()
-        # Creating an EventSub websocket.
-        EventSub = EventSubWebSocket(http=self._http, connection=self._connection,
-                                     loop=self.loop,
-                                     events=self._sub_events)
-        # Creating tasks.
-        tasks = [
-            self.loop.create_task(self._http.Refresher(expires_in=validation['expires_in']),
-                                  name="Twitchify:Refresher")
-        ]
-        self.dispatch('connect')
-        # Makes sure that there are events to subscribe to.
-        if len(EventSub.subscriptions) >= 1:
-            tasks.append(self.loop.create_task(EventSub.connect(), name="Twitchify:EventSub"))
-
-        await asyncio.gather(*tasks)
-
-    async def start(self, access_token: str, refresh_token: Optional[str] = None) -> None:
-        """
-        Starts the Twitch client by establishing a connection and initiating the event loop.
-
-        :param access_token: The access token for authentication.
-        :param refresh_token: The refresh token for refreshing the access token, if applicable.
-        """
-        try:
-            await self.connect(access_token, refresh_token)
-        # Automatically close the HTTP session when an error occurs.
-        except Exception as error:
-            # Checks if the _http session is open.
-            if self._http is not None and self._http.is_open:
-                await self._http.close()
-            raise error
-
-    def run(self, access_token: str, refresh_token: Optional[str] = None):
-        """
-       Runs the Twitch client by establishing a connection and initiating the event loop.
-
-       :param access_token: The access token for authentication.
-       :param refresh_token: The refresh token for refreshing the access token, if applicable.
-       """
-        async def runner():
-            await self.start(access_token, refresh_token)
-        asyncio.run(runner())
+    __slots__ = ('progress', 'goal', 'expires_at', '_last_contribution')
+
+    def __init__(self, train: ht.Begin) -> None:
+        self.goal: int = train['goal']
+        self.progress: int = train['progress']
+        self.expires_at: datetime = parse_rfc3339_timestamp(train['expires_at'])
+        self._last_contribution: List[ht.Contributor] = train['last_contribution']
+
+    def __repr__(self) -> str:
+        return f'<_Train goal={self.goal} progress={self.progress} expires_at={self.expires_at}>'
+
+    @property
+    def last_contribution(self) -> List[_Contributor]:
+        """The list of top contributors in the last contribution."""
+        return [_Contributor(contributor=c) for c in self._last_contribution]
+
+
+class HyperTrain:
+    """
+    Represents a channel Hyper Train.
+
+    :param hypertrain: An object representing a Hyper Train.
+    """
+    __slots__ = (
+        '__hypertrain', 'id', 'total', 'level', '_top_contributions', 'started_at', '_ended_at',
+        '_cooldown_ends_at')
+
+    def __init__(self, hypertrain: Union[ht.Begin, ht.Progress, ht.End]) -> None:
+        self.__hypertrain = hypertrain
+        self.id: str = hypertrain['id']
+        self.level: int = hypertrain['level']
+        self.total: int = hypertrain['total']
+        self._top_contributions: List[ht.Contributor] = hypertrain['top_contributions']
+        self.started_at: datetime = parse_rfc3339_timestamp(hypertrain['started_at'])
+        self._ended_at: Optional[str] = hypertrain.get('ended_at')
+        self._cooldown_ends_at: Optional[str] = hypertrain.get('cooldown_ends_at')
+
+    def __repr__(self) -> str:
+        return f'<HyperTrain id={self.id} level={self.level} total={self.total}>'
+
+    @property
+    def top_contributions(self) -> List[_Contributor]:
+        """The list of top contributors in the Hyper Train."""
+        return [_Contributor(contributor=c) for c in self._top_contributions]
+
+    @property
+    def train(self) -> Optional[Train]:
+        """The Hyper Train progress if it's ongoing, None otherwise."""
+        if not self._ended_at:
+            return Train(train=self.__hypertrain)
+        return None
+
+    @property
+    def ended_at(self) -> Optional[datetime]:
+        """The datetime when the Hyper Train ended."""
+        return parse_rfc3339_timestamp(self._ended_at) if self._ended_at else None
+
+    @property
+    def cooldown_ends_at(self) -> Optional[datetime]:
+        """The datetime when the Hyper Train cooldown ends."""
+        return parse_rfc3339_timestamp(self._cooldown_ends_at) if self._cooldown_ends_at else None
```

### Comparing `twitchify-1.0.5/twitch/errors.py` & `twitchify-1.1.0/twitch/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,31 +42,35 @@
     Exception raised when an operation in the Client class fails.
     """
 
     def __init__(self):
         super().__init__('Twitch API server error.')
 
 
+# ------------------------------------------
+#               HTTPException
+# ------------------------------------------
+
 class HTTPException(TwitchException):
     """
-    Exception raised when an HTTP request operation fail.
+    Exception raised when an HTTP request operation fails.
     """
     pass
 
 
 class SessionClosed(HTTPException):
     """
     Exception raised when the session is not open.
     """
     pass
 
 
 class BadRequest(HTTPException):
     """
-    Exception raised when twitch refused the request.
+    Exception raised when Twitch refuses the request.
     """
 
     def __init__(self, message: str = ''):
         super().__init__(message)
 
 
 class Unauthorized(HTTPException):
@@ -83,33 +87,50 @@
     Exception raised when the request is Forbidden.
     """
 
     def __init__(self, message: str = ''):
         super().__init__(message)
 
 
+# -------------------------------------------
+#                  Websocket
+# -------------------------------------------
+
 class WebSocketError(HTTPException):
     """
-    Exception raised when websocket error occurred.
+    Exception raised when a websocket error occurs.
     """
 
     def __init__(self, message: str = ''):
         super().__init__(message)
 
 
 class WebsocketClosed(WebSocketError):
     """
-    Exception raised when the websocket connection closed.
+    Exception raised when the websocket connection is closed.
     """
     pass
 
 
+class WsReconnect(WebSocketError):
+    """
+    Exception raised to indicate that WebSocket should reconnect to a new URL.
+    """
+
+    def __init__(self, url: str):
+        super().__init__(url)
+
+
+# -------------------------------------------
+#               ClientException
+# -------------------------------------------
+
 class ClientException(TwitchException):
     """
-    Exception raised when Client operation fails.
+    Exception raised when a Client operation fails.
     """
     pass
 
 
 class NotFound(ClientException):
     """
     Exception raised when the user does not exist.
@@ -121,9 +142,9 @@
 
 class SubscriptionError(ClientException):
     """
     Exception raised when the authorization is revoked.
     """
 
     def __init__(self, subscription: str, version: str):
-        message = f'Subscription type `%s` and version `%s`.' % (subscription, version)
+        message = f'Subscription type `{subscription}` and version `{version}`.'
         super().__init__(message)
```

### Comparing `twitchify-1.0.5/twitch/gateway.py` & `twitchify-1.1.0/twitch/gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,193 +20,181 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
-from .errors import (WebSocketError, WebsocketClosed, NotFound, SessionClosed, Forbidden, SubscriptionError)
+from .errors import (WebSocketError, WebsocketClosed, NotFound, SessionClosed, Forbidden,
+                     SubscriptionError, WsReconnect)
 from .utils import to_json, get_subscriptions
 
 # Libraries
-from asyncio import wait_for, sleep, TimeoutError, AbstractEventLoop
 from json import JSONDecodeError
 from aiohttp import WSMsgType
+import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionPayload
+    from asyncio import AbstractEventLoop
     from typing import Optional, List, Dict, Any
     from aiohttp import ClientWebSocketResponse
     from .state import ConnectionState
     from .http import HTTPClient
-    from .types.gateway import *
+    from .types.gateway import Session, Subscription
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
-class WsReconnect(Exception):
-    """
-    Reconnect to a new websocket.
-    """
-
-    def __init__(self, url: str):
-        super().__init__(url)
-
-
 class EventSubWebSocket:
     DEFAULT_URL = 'wss://eventsub.wss.twitch.tv/ws'
 
-    __slots__ = ('_http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive', '_ws', '_ws_switch',
-                 'session_id', 'retry_count')
+    __slots__ = ('__http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive',
+                 '_ws', '_ws_switch', 'session_id', 'retry_count')
 
-    def __init__(self, *, http: HTTPClient, connection: ConnectionState, loop, events: List[str]) -> None:
+    def __init__(self, *, http: HTTPClient, cnx: ConnectionState, loop, events: List[str]) -> None:
         """
         Initialize the EventSubWebSocket.
 
-        :param http:
-         The HTTP client for making API requests.
-
-        :param events:
-         A list of events.
-       """
-        self._http: HTTPClient = http
-        self.__connection = connection
+        :param http: The HTTP client for making API requests.
+        :param cnx: The ConnectionState object.
+        :param loop: The event loop.
+        :param events: A list of events.
+        """
+        self.__http: HTTPClient = http
+        self.__connection: ConnectionState = cnx
         self.__loop: AbstractEventLoop = loop
         self.subscriptions: List[SubscriptionPayload] = get_subscriptions(events=events)
-
+        # Default subscription
+        self.subscriptions.append({'name': 'user.update', 'version': '1'})
         # Default Session KeepAlive.
         self._keep_alive: int = 10
         self._ws: Optional[ClientWebSocketResponse] = None
         self._ws_switch: Optional[ClientWebSocketResponse] = None
         self.session_id: Optional[str] = None
         self.retry_count: int = 0
 
     async def _connect(self, url) -> None:
         """
         Establish a WebSocket connection.
 
-        :param url:
-         The URL to connect to.
+        :param url: The URL to connect to.
         """
-
-        if self._http.is_open:
-            _ws = await self._http.ws_connect(url=url)
-            if (self._ws is not None) and (not self._ws.closed):
+        if self.__http.is_open:
+            _ws = await self.__http.ws_connect(url=url)
+            if self._ws is not None and not self._ws.closed:
                 self._ws_switch = self._ws
                 self._ws = _ws
             else:
                 self._ws = _ws
             self.retry_count = 0
             await self.handle_messages()
         else:
             raise SessionClosed
 
     async def connect(self, url: str = DEFAULT_URL) -> None:
         """
         Connect to the WebSocket.
 
-        :param url:
-         The URL to connect to. Default is the DEFAULT_URL.
-       """
+        :param url: The URL to connect to. Default is the DEFAULT_URL.
+        """
         while True:
             try:
                 await self._connect(url=url)
             except WsReconnect as reconnect_url:
-                url = reconnect_url.__str__()
-                _logger.debug("Reconnecting to URL: %s", url)
+                url = str(reconnect_url)
+                _logger.debug('Reconnecting to URL: %s', url)
                 continue
             except (OSError, WebSocketError, SessionClosed, TimeoutError) as error:
                 self.retry_count += 1
                 if 3 >= self.retry_count:
                     if isinstance(error, WebSocketError):
-                        _logger.error(f'WebSocket connection closed. Retrying in %s seconds...', (5 * self.retry_count))
-                    elif isinstance(error, SessionClosed):
-                        _logger.error(f'Cannot connect because the session is closed. Retrying in %s seconds...',
+                        _logger.error('WebSocket connection closed. Retrying in %s seconds...',
                                       (5 * self.retry_count))
-                    elif isinstance(error, TimeoutError):
-                        _logger.error(
-                            f'Timeout occurred while waiting for WebSocket message. Retrying in %s seconds...',
-                            (5 * self.retry_count))
+                    elif isinstance(error, SessionClosed):
+                        _logger.error('Cannot connect because the session is closed.'
+                                      ' Retrying in %s seconds...', (5 * self.retry_count))
+                    elif isinstance(error, asyncio.TimeoutError):
+                        _logger.error('Timeout occurred while waiting for WebSocket message. '
+                                      'Retrying in %s seconds...', (5 * self.retry_count))
                     else:
-                        _logger.info(f'Retrying to connect to the WebSocket (%s) in %s seconds...', url,
-                                     5 * self.retry_count)
+                        _logger.info('Retrying to connect to the WebSocket (%s) in %s seconds...',
+                                     url, (5 * self.retry_count))
                 else:
-                    if isinstance(error, OSError):
-                        raise WebSocketError
-                    else:
-                        raise
-                await sleep(5 * self.retry_count)
+                    raise  # Re-raise the original error
+                await asyncio.sleep(5 * self.retry_count)
 
     async def handle_messages(self) -> None:
         """
         Handle incoming WebSocket messages.
         """
         while True:
-            try:
-                msg = await wait_for(self._ws.receive(), timeout=(self._keep_alive + 10))
-                if msg.type == WSMsgType.TEXT:
-                    await self.received_response(response=str(msg.data))
-                elif msg.type == WSMsgType.CLOSED:
-                    _logger.error('WebSocket connection closed by the server')
-                    close_code = self._ws.close_code
-                    if close_code == 4004:
-                        raise WebsocketClosed(
-                            'Failed to reconnect to a new WebSocket within the specified time (30 seconds).')
-                    elif close_code == 4007:
-                        raise WebsocketClosed(
-                            'Failed to reconnect to a new WebSocket. The reconnect URL provided is invalid.')
-                    elif close_code in [4000, 4001, 4002, 4003, 4005, 4006]:
-                        raise WebSocketError(f'WebSocket connection closed by the server. Close code: {close_code}')
-                    else:
-                        raise WebSocketError(f'WebSocket connection closed by the server. Close code: {close_code}')
-                elif msg.type == WSMsgType.ERROR:
-                    exception = self._ws.exception()
-                    error_message = str(exception) if exception else 'Unknown error occurred'
-                    raise WebSocketError('WebSocket connection closed with error: %s' % error_message)
-            except TimeoutError:
-                raise
+            msg = await asyncio.wait_for(self._ws.receive(), timeout=(self._keep_alive + 10))
+            if msg.type == WSMsgType.TEXT:
+                await self.received_response(response=str(msg.data))
+            elif msg.type == WSMsgType.CLOSED:
+                _logger.error('WebSocket connection closed by the server')
+                close_code = self._ws.close_code
+                if close_code == 4004:
+                    raise WebsocketClosed('Failed to reconnect to a new WebSocket within'
+                                          ' the specified time.')
+                elif close_code == 4007:
+                    raise WebsocketClosed('Failed to reconnect to a new WebSocket.'
+                                          ' The reconnect URL provided is invalid.')
+                elif close_code in [4000, 4001, 4002, 4003, 4005, 4006]:
+                    raise WebSocketError(
+                        f'WebSocket connection closed by the server. Close code:{close_code}')
+                else:
+                    raise WebSocketError(
+                        f'WebSocket connection closed by the server. Close code:{close_code}')
+            elif msg.type == WSMsgType.ERROR:
+                exception = self._ws.exception()
+                error_message = str(exception) if exception else 'Unknown error occurred'
+                raise WebSocketError(f'WebSocket connection closed with error:{error_message}')
 
     async def received_response(self, response: str) -> None:
         """
         Process the received response.
 
-       :param response:
-        The response received from the WebSocket.
-       """
+        :param response: The response received from the WebSocket.
+        """
         try:
             response: dict = to_json(text=response)
         except (UnicodeDecodeError, JSONDecodeError) as error:
             _logger.error('Failed to parse response as JSON: %s. Response: %s', error, response)
+            raise  # Re-raise the original error
         else:
             if response.get('metadata') is not None:
                 metadata = response['metadata']
                 # ====> Session Keepalive <====
                 if metadata['message_type'] == 'session_keepalive':
-                    _logger.debug('Received a keepalive message. The WebSocket connection is healthy.')
+                    _logger.debug(
+                        'Received a keepalive message. The WebSocket connection is healthy.')
                 # ====> Session Welcome <====
                 elif metadata['message_type'] == 'session_welcome':
                     _session: Session = response['payload']['session']
                     _logger.debug('Connected to WebSocket. Session ID: %s', _session['id'])
-                    # Close the old connection until the new reconnect websocket receive a Welcome message.
+                    # Close the old connection until the new reconnect websocket receive a
+                    # Welcome message.
                     if self._ws_switch is not None and not self._ws_switch.closed:
                         # Closing the old connection.
                         await self._ws_switch.close()
                         self._ws_switch = None
                     else:
                         # Subscribing to events.
-                        task = self._http.subscribe(user_id=self.__connection.broadcaster.id,
-                                                    session_id=_session['id'],
-                                                    subscriptions=self.subscriptions)
+                        task = self.__http.subscribe(user_id=self.__connection.broadcaster.id,
+                                                     session_id=_session['id'],
+                                                     subscriptions=self.subscriptions)
                         self.__loop.create_task(task, name='Twitchify:Subscriptions')
                     if _session['id'] != self.session_id:
                         if self.session_id is not None:
-                            _logger.debug('A new WebSocket Session has been detected ID: %s', _session['id'])
+                            _logger.debug('A new WebSocket Session has been detected ID: %s',
+                                          _session['id'])
                         self.session_id = _session['id']
                     # KeepAlive timeout.
                     self._keep_alive = _session['keepalive_timeout_seconds']
 
                 # ====> Session Reconnect <====
                 elif metadata['message_type'] == 'session_reconnect':
                     _session: Session = response['payload']['session']
@@ -220,16 +208,16 @@
 
                 # ====> Subscription Revocation <====
                 elif metadata['message_type'] == 'revocation':
                     _subscription: Subscription = response['payload']['subscription']
                     _status = _subscription['status']
                     # Revoked the authorization token that the subscription relied on.
                     if _status == 'authorization_revoked':
-                        raise Forbidden(
-                            'The user has revoked authorization for the `%s` subscription.' % _subscription['type'])
+                        raise Forbidden(f'The user has revoked authorization for the'
+                                        f' `{_subscription["type"]}` subscription.')
                     # The user mentioned in the subscription no longer exists.
                     elif _status == 'user_removed':
                         raise NotFound(
                             'The user mentioned in the subscription no longer exists.'
                         )
                     # Subscription type and version is no longer supported.
                     elif _status == 'version_removed':
```

### Comparing `twitchify-1.0.5/twitch/http.py` & `twitchify-1.1.0/twitch/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,54 +20,48 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
-from .errors import (UnknownError, TwitchServerError, BadRequest, Unauthorized,
-                     Forbidden, HTTPException, SubscriptionError)
-from . import __version__, __github__
-from .utils import format_seconds
-from .user import Broadcaster
-
-# Libraries
-from aiohttp import (ClientSession, helpers)
-from asyncio import Lock, sleep
+from aiohttp import ClientSession, helpers
+from asyncio import Lock, sleep, Task
 from time import time
+from typing import TYPE_CHECKING, Optional, List, Callable, Any
+
+from .errors import (
+    UnknownError, TwitchServerError, BadRequest, Unauthorized,
+    Forbidden, HTTPException, SubscriptionError, NotFound)
+from .utils import format_seconds
 
-from typing import TYPE_CHECKING
 if TYPE_CHECKING:
+    from .types.stream import Stream
+    from .types.user import UserType
+    from .types.channel import Channel
     from .types.eventsub.subscriptions import SubscriptionPayload
     from aiohttp import ClientWebSocketResponse
     from .types.http import Validate, Refresh
-    from .state import ConnectionState
-    from typing import Optional, List
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class Route:
     BASE_ROUTE: str = 'https://api.twitch.tv/helix/'
 
     __slots__ = ('method', 'url')
 
     def __init__(self, method: str, path: Optional[str] = None, url: Optional[str] = None) -> None:
         """
         Initialize a Route object.
 
-        :param method:
-         The HTTP method of the route.
-        :param path:
-         The path of the route.
-
-        :param url:
-         The complete URL of the route (overrides BASE_ROUTE + path). Defaults to None.
+        :param method: The HTTP method of the route.
+        :param path: The path of the route.
+        :param url: The complete URL of the route (overrides BASE_ROUTE + path). Defaults to None.
         """
         self.method: str = method
         if path is None and url is None:
             raise TypeError
         else:
             if url is not None:
                 self.url = url
@@ -76,47 +70,44 @@
 
     def __repr__(self) -> str:
         return f'<Route method={self.method} url={self.url}>'
 
 
 class HTTPClient:
     """Serves as an HTTP client responsible for sending HTTP requests to the Twitch API."""
+    __slots__ = ('_dispatch', '_client_id', '_client_secret', '__session', '_session_lock',
+                 '_user_agent', '_refresh_token')
 
-    __slots__ = ('__connection', '_client_id', '_client_secret', '__session', '_session_lock', '_user_agent',
-                 '_refresh_token')
-
-    def __init__(self, *, connection: ConnectionState, client_id: str, client_secret: Optional[str]) -> None:
+    def __init__(self, dispatcher: Callable[..., Any], client: str, secret: Optional[str]) -> None:
         """
         Initialize the HTTPClient object.
         """
-        self.__connection = connection
-        self._client_id = client_id
-        self._client_secret = client_secret
+        self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
+        self._client_id = client
+        self._client_secret = secret
         self.__session: Optional[ClientSession] = None
         self._session_lock: Lock = Lock()
-
-        self._user_agent: str = f'Twitchify/{__version__} (GitHub: {__github__})'
+        github = 'https://github.com/Rapptz/discord.py/blob/master/discord/http.py'
+        self._user_agent: str = f'Twitchify/1.1.0 (GitHub: {github})'
         self._refresh_token: Optional[str] = None
 
     @property
     def is_open(self) -> bool:
         """
         Checks if the HTTP session is open.
 
-        :return:
-         True if the session is open, False otherwise.
+        :return: True if the session is open, False otherwise.
         """
         return self.__session is not None and not self.__session.closed
 
     async def _open(self, *, access_token: str) -> None:
         """
         Opens an HTTP session.
 
-        :param access_token:
-         The access token to use for authentication.
+        :param access_token: The access token to use for authentication.
         """
         async with self._session_lock:
             if not self.is_open:
                 headers = {
                     'Client-ID': self._client_id,
                     'Authorization': f'Bearer {access_token}',
                     'Content-Type': 'application/json'
@@ -134,35 +125,37 @@
         async with self._session_lock:
             if self.is_open:
                 await self.__session.close()
                 self.__session = None
                 _logger.debug('HTTP session has been closed.')
         return not self.is_open
 
-    async def open_session(self, access_token: str, refresh_token: Optional[str] = None) -> Validate:
+    async def open_session(self, token: str, refresh_token: Optional[str] = None) -> Validate:
         """
         Verifies the access token and opens a new session with it.
 
-        :param access_token:
+        :param token:
          The access token for authentication.
 
         :param refresh_token:
          (Optional) The refresh token for refreshing the access token.
 
         :return: A validation response.
         """
         # Opening a session.
-        await self._open(access_token=access_token)
+        await self._open(access_token=token)
         self._refresh_token: Optional[str] = refresh_token
         validation: Validate = await self._validate_token(generate=True)
         if validation['expires_in'] == 0:
-            _logger.debug('Old application detected, exempt from expiration rules. Investigation needed.')
+            _logger.debug('Old application detected, exempt from expiration rules.'
+                          ' Investigation needed.')
             if self._refresh_token is not None:
                 _logger.warning(
-                    'The refresh token has been removed due to the access token returning an expire time of 0.')
+                    'The refresh token has been removed due to the access token returning an'
+                    ' expire time of 0.')
         else:
             self._refresh_token = refresh_token
 
         return validation
 
     async def ws_connect(self, *, url: str) -> ClientWebSocketResponse:
         """
@@ -196,49 +189,54 @@
         method = route.method
         url = route.url
         for retry_count in range(1, 4):
             try:
                 async with self.__session.request(method, url, **kwargs) as response:
                     if response.status in [200, 202]:
                         return await response.json()
-                    elif response.status == 400:
+                    if response.status == 400:
                         raise BadRequest
                     elif response.status == 401:
                         raise Unauthorized
                     elif response.status == 403:
                         raise Forbidden
+                    elif response.status == 404:
+                        raise NotFound
                     elif 500 <= response.status < 600:
                         raise TwitchServerError
-                    else:
-                        raise UnknownError
-            except OSError:
+                    raise UnknownError
+            except OSError as exc:
                 if 3 >= retry_count:
-                    _logger.info(f'Request failed: %s. Retrying in %s seconds...', route, (5 * retry_count))
+                    _logger.info('Request failed: %s. Retrying in %s seconds...',
+                                 Route, (5 * retry_count))
                     await sleep(5 * retry_count)
-        else:
-            raise HTTPException
+                raise HTTPException from exc
 
     async def _generate_token(self) -> Optional[Refresh]:
         if self._refresh_token and self._client_secret:
-            # There is a chance that both the task and the normal request can refresh the token at the same time.
+            # There is a chance that both the task and the normal
+            # request can refresh the token at the same time.
             if not self._session_lock.locked():
                 async with self._session_lock:
                     # Encoding the client secret.
                     encoded_secret = helpers.quote(self._refresh_token)
                     params = {'grant_type': 'refresh_token',
                               'refresh_token': encoded_secret,
                               'client_id': self._client_id,
                               'client_secret': self._client_secret}
                     _logger.debug('Generating a new access token to refresh the existing one.')
                     route = Route(method='POST', url='https://id.twitch.tv/oauth2/token')
                     refresh: Refresh = await self.request(route=route, params=params)
                     # Updating the session headers.
-                    self.__session.headers.update({'Authorization': f'Bearer {refresh["access_token"]}'})
-                    _logger.debug('Session headers have been successfully updated with the new access token.')
-                    await self.__connection.parse(event='refresh_token', data=refresh)
+                    self.__session.headers.update({
+                        'Authorization': f'Bearer {refresh["access_token"]}'
+                    })
+                    _logger.debug('Session headers have been successfully updated with'
+                                  ' the new access token.')
+                    self._dispatch('refresh_token', refresh['access_token'])
                     return refresh
         return None
 
     async def _validate_token(self, *, generate: bool = False) -> Validate:
         """
         Validating access token.
 
@@ -250,57 +248,62 @@
         """
         while True:
             try:
                 route = Route(method='GET', url='https://id.twitch.tv/oauth2/validate')
                 validation: Validate = await self._request(route=route)
                 _logger.debug('Access token successfully validated.')
                 return validation
-            except Unauthorized:
+            except Unauthorized as exc:
                 if generate and (self._client_secret and self._refresh_token):
                     try:
                         # Generating a new access token.
                         await self._generate_token()
+                        continue
                     except (BadRequest, Forbidden):
-                        raise Unauthorized(message='Invalid refresh token or client secret.')
+                        raise Unauthorized(message='Invalid refresh token or client secret.'
+                                           ) from exc
                 else:
                     raise
 
     async def Refresher(self, *, expires_in: int) -> None:
         """
         Refresher task to refresh the current access token.
 
         :param expires_in:
          The expiration time of the current access token.
         """
         start_time = time()
         # If the refresh_token or client_secret is missing,
         if self._refresh_token and self._client_secret:
-            _logger.debug("A new token will be generated in %s.", format_seconds(expires_in - 300))
+            _logger.debug('A new token will be generated in %s.', format_seconds(expires_in - 300))
         else:
             # Set expires_in to a default value of 3540 seconds (59 minutes).
             expires_in = 3540 + 300
-            _logger.debug('Access token generation disabled due to missing refresh token or client secret.')
+            _logger.debug('Access token generation disabled due to'
+                          ' missing refresh token or client secret.')
         while True:
-            # Create a new access token approximately 5 minutes before the current token's expiration.
+            # Create a new access token approximately 5 minutes before the
+            # current token's expiration.
             await sleep(min((expires_in - 300), 3540))
             current_time = time()
             elapsed_time = current_time - start_time
             try:
                 if elapsed_time >= expires_in - 300:
                     # Reset the refresh token timer
                     start_time = time()
                     await self._generate_token()
-                    _logger.debug("A new token will be generated in %s.", format_seconds(expires_in - 300))
-
+                    _logger.debug('A new token will be generated in %s.',
+                                  format_seconds(expires_in - 300))
                 # ==> Validating the access token <==
                 validation: Validate = await self._validate_token()
-                # Update the expiration time of the access token. Update the expiration time of the access token.
+                # Update the expiration time of the access token.
                 expires_in = validation['expires_in']
             except BadRequest:
-                _logger.warning('Invalid Refresh Token. The automatic generation feature has been disabled.')
+                _logger.warning('Invalid Refresh Token.'
+                                ' The automatic generation feature has been disabled.')
                 self._refresh_token = None
 
     async def request(self, *, route: Route, **kwargs) -> _request:
         """
         Sends an HTTP request to the specified route.
 
         :param route:
@@ -310,26 +313,29 @@
          Additional parameters to pass to the request.
 
         :return:
          The response from the API.
         """
         while True:
             try:
-                _logger.debug(f'Sending request: %s %s, kwargs: %s.', route.method, route.url, kwargs)
+                _logger.debug('Sending request: %s kwargs: %s.', route, kwargs)
                 data: dict = await self._request(route=route, **kwargs)
-                _logger.debug(f'Received response: %s', data)
+                _logger.debug('Received response: %s', data)
                 return data
             except Unauthorized:
                 try:
-                    _logger.error(f'Unable to make the request to URL: %s. Unauthorized access.', route.url)
+                    _logger.error('Unable to make the request to URL: %s Unauthorized access.',
+                                  route.url)
                     await self._validate_token(generate=True)
+                    continue
                 except (Unauthorized, BadRequest):
                     raise
 
-    async def subscribe(self, *, user_id: str, session_id: str, subscriptions: List[SubscriptionPayload]) -> None:
+    async def subscribe(self, *, user_id: str, session_id: str,
+                        subscriptions: List[SubscriptionPayload]) -> None:
         """
         Subscribes to multiple events with the specified subscriptions.
 
         :param user_id:
          The user ID.
 
         :param session_id:
@@ -350,26 +356,46 @@
                         'to_broadcaster_user_id': user_id
                     },
                     'transport': {
                         'method': 'websocket',
                         'session_id': session_id
                     }
                 }
-                _logger.debug(f'Subscribing to `%s` event version %s.', subscription['name'], subscription['version'])
+                _logger.debug('Subscribing to `%s` event version %s.',
+                              subscription['name'], subscription['version'])
                 route = Route(method='POST', path='eventsub/subscriptions')
                 await self.request(route=route, json=data)
-            except Forbidden:
-                raise Forbidden('Subscription `%s` is missing proper authorization' % subscription['name'])
-            except BadRequest:
+            except Forbidden as exc:
+                raise Forbidden(f'Subscription `{subscription["name"]}`'
+                                f' is missing proper authorization') from exc
+            except BadRequest as exc:
                 raise SubscriptionError(subscription=subscription['name'],
-                                        version=subscription['version'])
-        await self.__connection.parse(event='ready')
+                                        version=subscription['version']) from exc
+        self._dispatch('ready')
 
-    async def get_client(self) -> Broadcaster:
+    async def get_client(self) -> UserType:
         """
-        Retrieves the user with the associated access token.
-
-        :return:
-         The Broadcaster.
+        Retrieves the broadcaster with the associated access token.
         """
         data = await self.request(route=Route(method='GET', path='users'))
-        return Broadcaster(data=data['data'][0])
+        return data['data'][0]
+
+    async def get_channel(self, broadcaster_id: str) -> Channel:
+        """
+        Retrieves the channel information.
+        """
+        _route = Route(method='GET', path=f'channels?broadcaster_id={broadcaster_id}')
+        data = await self.request(route=_route)
+        return data['data'][0]
+
+    async def get_stream(self, user_id: str) -> Optional[Stream]:
+        """
+        Retrieves the stream.
+        """
+        try:
+            _route = Route(method='GET', path=f'streams?user_id={user_id}')
+            data = await self.request(route=_route)
+            if len(data['data']) == 1:
+                return data['data'][0]
+        except NotFound:
+            pass
+        return None
```

### Comparing `twitchify-1.0.5/twitch/message.py` & `twitchify-1.1.0/twitch/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,50 +21,57 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .types import message as msg
-    from typing import List, Optional
+    from typing import List
 
 
 class Emote:
     """
     Represents a message emote.
+
+    :param emote: A dictionary representing the emote with 'id', 'begin', and 'end' keys.
     """
+
     __slots__ = ('id', 'begin', 'end')
 
     def __init__(self, *, emote: msg.Emote) -> None:
         self.id: str = emote['id']
         self.begin: int = emote['begin']
         self.end: int = emote['end']
 
     def __repr__(self) -> str:
         return f'<Emote id={self.id} begin={self.begin} end={self.end}>'
 
 
 class Message:
     """
     Represents a chat message.
+
+    :param message: A dictionary representing the message with 'text' and 'emotes' keys.
     """
+
     __slots__ = ('content', '_emotes')
 
     def __init__(self, *, message: msg.Message) -> None:
         self.content: str = message['text']
         self._emotes: List[msg.Emote] = message['emotes']
 
     def __repr__(self) -> str:
         return f'<Message message={self.content}>'
 
     def __str__(self) -> str:
         return self.content
 
     @property
-    def emotes(self) -> Optional[List[Emote]]:
-        if len(self._emotes) != 0:
-            return [Emote(emote=emote) for emote in self._emotes]
-
-        return None
+    def emotes(self) -> List[Emote]:
+        """
+        Retrieve the list of emotes in the message, if any.
+
+        :return: List of Emote objects.
+        """
+        return [Emote(emote=emote) for emote in self._emotes]
```

### Comparing `twitchify-1.0.5/twitch/moderation.py` & `twitchify-1.1.0/twitch/moderation.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     @property
     def ends_at(self) -> Optional[datetime]:
         if self._ends_at:
             return parse_rfc3339_timestamp(timestamp=self._ends_at)
         return None
 
     def __repr__(self) -> str:
-        return f'<Ban user={self.user.__repr__()} moderator={self.moderator.__repr__()} reason={self.reason}>'
+        return f'<Ban user={self.user.__repr__()} moderator={self.moderator.__repr__()}>'
 
 
 class UnBan:
     """
     Represents a channel unban.
     """
     __slots__ = ('user', 'moderator')
@@ -81,15 +81,16 @@
 
     def __init__(self, mode: Union[md.ShieldModeBegin, md.ShieldModeEnd]) -> None:
         self.moderator: User = User(user=mode, prefix='moderator_user')
         self._started_at: Optional[str] = mode.get('started_at')
         self._ended_at: Optional[str] = mode.get('ended_at')
 
     def __repr__(self) -> str:
-        return f'<UnBan moderator={self.moderator} _started_at={self._started_at} _ended_at={self._ended_at}>'
+        return f'<UnBan moderator={self.moderator} _started_at={self._started_at}' \
+               f' _ended_at={self._ended_at}>'
 
     @property
     def is_enabled(self) -> bool:
         return self._started_at is not None
 
     @property
     def started_at(self) -> Optional[datetime]:
```

### Comparing `twitchify-1.0.5/twitch/reward.py` & `twitchify-1.1.0/twitch/reward.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 
 
 class _Appearance:
     """
     Represents the appearance settings for a reward.
     """
 
-    __slots__ = ('title', 'description', 'is_in_stock', 'background_color', 'image', 'default_image')
+    __slots__ = ('title', 'description', 'is_in_stock', 'background_color', 'image',
+                 'default_image')
 
     def __init__(self, *, reward: rd.Reward) -> None:
         self.title: str = reward['title']
         self.description: str = reward['prompt']
         self.background_color: str = reward['background_color']
         self.image: _OptionalImage = _OptionalImage(image=reward['image'])
         self.default_image: _Image = _Image(image=reward['default_image'])
@@ -146,27 +147,28 @@
         return None
 
 
 class Reward:
     """
     Represents a channel reward.
     """
-    __slots__ = ('id', 'cost', 'status', 'appearance', 'options', 'cooldown', 'redeemed_current_stream')
+    __slots__ = ('id', 'cost', 'status', 'appearance', 'options', 'cooldown',
+                 'redeemed_current_stream')
 
     def __init__(self, *, reward: rd.Reward) -> None:
         self.id: str = reward['id']
         self.cost: int = reward['cost']
         self.status: _Status = _Status(reward=reward)
         self.appearance: _Appearance = _Appearance(reward=reward)
         self.options: _Options = _Options(reward=reward)
         self.cooldown: _Cooldown = _Cooldown(reward=reward)
         self.redeemed_current_stream: Optional[int] = reward['redemptions_redeemed_current_stream']
 
     def __repr__(self) -> str:
-        return f'<Reward id={self.id} cost={self.cost} redeemed_current_stream={self.redeemed_current_stream}>'
+        return f'<Reward id={self.id} redeemed_current_stream={self.redeemed_current_stream}>'
 
 
 class _Reward:
     """
     Represents a base reward.
     """
     __slots__ = ('id', 'title', 'cost', 'description')
@@ -191,8 +193,8 @@
         self.id: str = redemption['id']
         self.user: User = User(user=redemption)
         self.status: str = redemption['status']
         self.reward: _Reward = _Reward(reward=redemption['reward'])
         self.redeemed_at: datetime = parse_rfc3339_timestamp(timestamp=redemption['redeemed_at'])
 
     def __repr__(self) -> str:
-        return f'<Redemption id={self.id} user={self.user} reward={self.reward.__repr__()} status={self.status}>'
+        return f'<Redemption id={self.id} user={self.user} reward={self.reward.__repr__()}>'
```

### Comparing `twitchify-1.0.5/twitch/state.py` & `twitchify-1.1.0/twitch/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,81 +21,91 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 # Core
-from .channel import Channel, Subscription, SubscriptionGift, SubscriptionMessage, Cheer, Raid
+from .channel import Update, Subscription, SubscriptionGift, SubscriptionMessage, Cheer, Raid
 from .goals import Donation, Charity, Goal, HyperTrain
-from .user import Broadcaster, Follower, User, Update
+from .user import Follower, User, UserUpdate
+from .broadcaster import Broadcaster
 from .moderation import Ban, UnBan, ShieldMode
 from .stream import Online, Offline, Shoutout
 from .reward import Reward, Redemption
 from .survey import Poll, Prediction
+from asyncio import Task
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
-    from typing import Optional, Dict, Callable, Any
-    from .types.http import Refresh
+    from typing import Optional, Dict, Callable, Any, List
+    from .http import HTTPClient
+    from .types.eventsub.reward import Redemption as Rp
     from .types.eventsub import (
         channel as chl,
         moderation as md,
         reward as rd,
         poll as pl,
         prediction as pd,
         charity as ch,
         goal as gl,
         hypertrain as ht,
         stream as sm,
         user as us)
 
 import logging
+
 _logger = logging.getLogger(__name__)
 
 
 class ConnectionState:
     """
     Represents the state of the connection.
     """
+    __slots__ = ('_http', 'broadcaster', '_dispatch', 'is_streaming', 'events')
 
-    def __init__(self, dispatcher: Callable[..., Any]) -> None:
+    def __init__(self, dispatcher: Callable[..., Any], http: HTTPClient, ev: List[str]) -> None:
+        self._http: HTTPClient = http
+        self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
         self.broadcaster: Optional[Broadcaster] = None
-        self._dispatch: Callable[..., Any] = dispatcher
+        self.events: List[str] = ev
+
+    async def get_client(self) -> None:
+        """
+        Retrieves the broadcaster's data from the connection's HTTP client and initializes the
+        Broadcaster object.
+        """
+        _data = await self._http.get_client()
+        self.broadcaster = Broadcaster(http=self._http, user=_data)
 
-    async def parse(self, event: str, data: Optional[Dict[str, Any]] = None) -> None:
+    async def parse(self, method: str, data: Optional[Dict[str, Any]] = None) -> None:
         """
         Parse an event and dispatch it to the appropriate handler.
         """
         try:
-            parse = self.__getattribute__('parse_' + event.replace('.', '_'))
+            parse = getattr(self, 'parse_' + method.replace('.', '_'))
             if data is None:
                 await parse()
             else:
                 await parse(data)
         except Exception as error:
-            _logger.error(f'Failed to parse event: {event}, {error}')
+            _logger.error('Failed to parse event: %s, %s', method, error)
 
     async def parse_ready(self) -> None:
         """
         Parse ready event.
         """
         self._dispatch('ready')
 
-    async def parse_refresh_token(self, data: Refresh) -> None:
-        """
-        Parse a refresh token event.
-        """
-        self._dispatch('refresh_token', data['access_token'])
-
     async def parse_channel_update(self, data: chl.Update) -> None:
         """
         Parse a channel update event.
         """
-        _channel = Channel(channel=data)
+        _channel = Update(channel=data)
         self._dispatch('channel_update', _channel)
 
     async def parse_channel_follow(self, data: chl.Follow) -> None:
         """
         Parse a channel follow event.
         """
         _user = Follower(channel=data)
@@ -190,22 +200,22 @@
     async def parse_channel_channel_points_custom_reward_remove(self, data: rd.Reward):
         """
         Parse a channel custom reward remove event for channel points.
         """
         _reward = Reward(reward=data)
         self._dispatch('points_reward_remove', _reward)
 
-    async def parse_channel_channel_points_custom_reward_redemption_add(self, data: rd.Redemption) -> None:
+    async def parse_channel_channel_points_custom_reward_redemption_add(self, data: Rp) -> None:
         """
         Parse a channel custom reward redemption add event for channel points.
         """
         _redemption = Redemption(redemption=data)
         self._dispatch('points_reward_redemption', _redemption)
 
-    async def parse_channel_channel_points_custom_reward_redemption_update(self, data: rd.Redemption) -> None:
+    async def parse_channel_channel_points_custom_reward_redemption_update(self, data: Rp) -> None:
         """
         Parse a channel custom reward redemption update event for channel points.
         """
         _redemption = Redemption(redemption=data)
         self._dispatch('points_reward_redemption_update', _redemption)
 
     # ========================> Survey <========================
@@ -376,14 +386,15 @@
         _stream = Offline(stream=data)
         self._dispatch('stream_offline', _stream)
 
     async def parse_user_update(self, data: us.Update) -> None:
         """
         Parse a user update event.
         """
-        _update = Update(update=data)
+        _update = UserUpdate(update=data)
         # Updating the broadcaster
         self.broadcaster.name = _update.name
         self.broadcaster.display_name = _update.display_name
-        self.broadcaster._description = _update.description
+        self.broadcaster.description = _update.description
         self.broadcaster.email = _update.email
-        self._dispatch('user_update', _update)
+        if 'user_update' in self.events:
+            self._dispatch('user_update', _update)
```

### Comparing `twitchify-1.0.5/twitch/stream.py` & `twitchify-1.1.0/twitch/stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,27 +23,45 @@
 """
 
 from __future__ import annotations
 
 # Core
 from .utils import parse_rfc3339_timestamp
 from .user import User
-
+from datetime import datetime
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from .types.eventsub import stream as sm
-    from typing import Optional, Union
-    from datetime import datetime
+    from typing import Optional, Union, List
+    from .types import stream as mst
+
+
+class Stream:
+    __slots__ = ('id', 'language', 'viewers', 'thumbnail_url', 'is_mature', 'started_at')
+
+    def __init__(self, stream: mst.Stream) -> None:
+        self.id: str = stream['id']
+        self.language: str = stream['language']
+        self.viewers: int = stream['viewer_count']
+        self.thumbnail_url: str = stream['thumbnail_url']
+        self.is_mature: bool = stream['is_mature']
+        self.started_at: datetime = parse_rfc3339_timestamp(timestamp=stream['started_at'])
+
+    def __repr__(self) -> str:
+        return f'<Stream id={self.id} viewers={self.viewers} language={self.language}>'
 
 
 class Shoutout:
     """
     Represents a stream shoutout.
     """
-    __slots__ = ('__shoutout', 'viewer_count', 'started_at', '_cooldown_ends_at', '_target_cooldown_ends_at')
+    __slots__ = (
+        '__shoutout', 'viewer_count', 'started_at', '_cooldown_ends_at',
+        '_target_cooldown_ends_at')
 
     def __init__(self, shoutout: Union[sm.ShoutoutCreate, sm.ShoutoutReceived]) -> None:
 
         self.__shoutout = shoutout
         self.viewer_count: int = shoutout['viewer_count']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=shoutout['started_at'])
         self._cooldown_ends_at: Optional[str] = shoutout.get('cooldown_ends_at')
@@ -52,23 +70,21 @@
     def __repr__(self) -> str:
         return f'<Shoutout sender={self.sender.__repr__()} Receiver={self.receiver.__repr__()}>'
 
     @property
     def sender(self) -> User:
         if self._cooldown_ends_at:
             return User(user=self.__shoutout, prefix='broadcaster_user')
-        else:
-            return User(user=self.__shoutout, prefix='from_broadcaster_user')
+        return User(user=self.__shoutout, prefix='from_broadcaster_user')
 
     @property
     def receiver(self):
         if self._cooldown_ends_at is None:
             return User(user=self.__shoutout, prefix='broadcaster_user')
-        else:
-            return User(user=self.__shoutout, prefix='to_broadcaster_user')
+        return User(user=self.__shoutout, prefix='to_broadcaster_user')
 
     @property
     def cooldown_ends_at(self) -> Optional[datetime]:
         if self._cooldown_ends_at:
             return parse_rfc3339_timestamp(timestamp=self._cooldown_ends_at)
         return None
 
@@ -88,21 +104,21 @@
     def __init__(self, stream: sm.Online) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
         self.id: str = stream['id']
         self.type: str = stream['type']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=stream['started_at'])
 
     def __repr__(self) -> str:
-        return f'<Online user={self.user} id={self.id} type={self.type} started_at={self.started_at}>'
+        return f'<Online user={self.user} id={self.id} started_at={self.started_at}>'
 
 
 class Offline:
     """
     Represents an offline stream.
     """
-    __slots__ = 'user'
+    __slots__ = ('user',)
 
     def __init__(self, stream: sm.Offline) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
 
     def __repr__(self) -> str:
         return f'<Offline user={self.user}>'
```

### Comparing `twitchify-1.0.5/twitch/survey.py` & `twitchify-1.1.0/twitch/survey.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 from __future__ import annotations
 
 # Core
 from .utils import parse_rfc3339_timestamp
 from .user import User
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from typing import Optional, List, Union, Literal
     from .types.eventsub import poll as pl
     from .types.eventsub import prediction as pd
     from datetime import datetime
 
 
-
 class _Voting:
     """
     Represents voting settings for a poll.
     """
 
     __slots__ = ('enabled', 'amount_per_vote')
 
@@ -68,16 +68,16 @@
         return f'<Choice id={self.id} title={self.title}>'
 
 
 class Poll:
     """
     Represents a channel poll.
     """
-    __slots__ = ('id', 'title', '_choices', 'bits_voting', 'points_voting', 'started_at', '_ends_at', '_ended_at',
-                 '_status')
+    __slots__ = ('id', 'title', '_choices', 'bits_voting', 'points_voting', 'started_at',
+                 '_ends_at', '_ended_at', '_status')
 
     def __init__(self, poll: Union[pl.Begin, pl.Progress, pl.End]):
         self.id: str = poll['id']
         self.title: str = poll['title']
         self._choices: List[Union[pl.Choice, pl.ChoicesCount]] = poll['choices']
         self.bits_voting: _Voting = _Voting(vote=poll['bits_voting'])
         self.points_voting: _Voting = _Voting(vote=poll['channel_points_voting'])
@@ -97,23 +97,21 @@
     def is_ended(self):
         return self._ended_at is not None
 
     @property
     def status(self) -> Literal['active', 'completed', 'archived', 'terminated']:
         if self._ended_at:
             return self._status
-        else:
-            return 'active'
+        return 'active'
 
     @property
     def end_at(self) -> datetime:
         if self._ended_at is not None:
             return parse_rfc3339_timestamp(timestamp=self._ended_at)
-        else:
-            return parse_rfc3339_timestamp(timestamp=self._ends_at)
+        return parse_rfc3339_timestamp(timestamp=self._ends_at)
 
 
 class _Predictor:
     """
     Represents a predictor in a prediction.
     """
 
@@ -149,29 +147,29 @@
     def __repr__(self):
         return f'<Outcome user={self.id} title={self.title} color={self.color}>'
 
     @property
     def users(self) -> int:
         if self._top_predictors is None:
             return self._users
-        else:
-            return len(self._top_predictors)
+        return len(self._top_predictors)
 
     @property
     def top_predictors(self) -> List[_Predictor]:
         if self._top_predictors:
             return [_Predictor(predictor=p) for p in self._top_predictors]
         return []
 
 
 class Prediction:
     """
     Represents a channel prediction.
     """
-    __slots__ = ('id', 'title', '_outcomes', 'started_at', '_locks_at', '_locked_at', '_ended_at', '_status')
+    __slots__ = ('id', 'title', '_outcomes', 'started_at', '_locks_at', '_locked_at', '_ended_at',
+                 '_status')
 
     def __init__(self, *, prediction: Union[pd.Begin, pd.Progress, pd.Lock, pd.End]):
         self.id: str = prediction['id']
         self.title: str = prediction['title']
         self._outcomes: List[Union[pd.Outcome, pd.BaseOutcome]] = prediction['outcomes']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=prediction['started_at'])
         self._locks_at: Optional[str] = prediction.get('locks_at')
@@ -186,18 +184,17 @@
     def outcomes(self) -> List[_Outcome]:
         return [_Outcome(outcome=o) for o in self._outcomes]
 
     @property
     def status(self) -> Literal['open', 'locked', 'resolved', 'canceled']:
         if self._locks_at:
             return 'open'
-        elif self._locked_at:
+        if self._locked_at:
             return 'locked'
-        else:
-            return self._status
+        return self._status
 
     @property
     def is_locked(self) -> bool:
         if self._locked_at or self._ended_at:
             return True
         return False
 
@@ -207,15 +204,15 @@
             return True
         return False
 
     @property
     def lock_at(self) -> Optional[datetime]:
         if self._locks_at:
             return parse_rfc3339_timestamp(timestamp=self._locks_at)
-        elif self._locked_at:
+        if self._locked_at:
             return parse_rfc3339_timestamp(timestamp=self._locked_at)
         return None
 
     @property
     def ended_at(self) -> Optional[datetime]:
         if self._ended_at:
             return parse_rfc3339_timestamp(timestamp=self._ended_at)
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/channel.py` & `twitchify-1.1.0/twitch/types/eventsub/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 # Core
-from ..user import SpecificBroadcaster, SpecificUser, SpecificAnonymous, ToSpecificBroadcaster, FromSpecificBroadcaster
+from ..user import SpecificBroadcaster, SpecificUser, SpecificAnonymous, ToSpecificBroadcaster,\
+    FromSpecificBroadcaster
 from ..message import Message
 
 # Libraries
 from typing import Optional
 
 
 class Update(SpecificBroadcaster):
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/charity.py` & `twitchify-1.1.0/twitch/types/eventsub/charity.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,13 +80,7 @@
     Type: Charity Campaign Stop
     Name: `channel.charity_campaign.stop`
     Version: 1
     """
     current_amount: Amount
     target_amount: Amount
     stopped_at: str
-
-
-
-
-
-
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/goal.py` & `twitchify-1.1.0/twitch/types/eventsub/goal.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 # Core
 from ..user import SpecificBroadcaster
 # Libraries
 from typing import TypedDict, Literal
 
 
 class Goal(TypedDict):
-    type: Literal['follow', 'subscription', 'subscription_count', 'new_subscription', 'new_subscription_count']
+    type: Literal['follow', 'subscription', 'subscription_count', 'new_subscription',
+                  'new_subscription_count']
     current_amount: int
 
 
 class _GoalBase(SpecificBroadcaster, Goal):
     id: str
     description: str
     started_at: str
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/hypertrain.py` & `twitchify-1.1.0/twitch/types/eventsub/hypertrain.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/eventsub/moderation.py` & `twitchify-1.1.0/twitch/types/eventsub/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/eventsub/poll.py` & `twitchify-1.1.0/twitch/types/eventsub/poll.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/eventsub/prediction.py` & `twitchify-1.1.0/twitch/types/eventsub/prediction.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/eventsub/reward.py` & `twitchify-1.1.0/twitch/types/eventsub/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/eventsub/stream.py` & `twitchify-1.1.0/twitch/types/eventsub/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 # Core
-from ..user import SpecificBroadcaster, SpecificModerator, ToSpecificBroadcaster, FromSpecificBroadcaster
+from ..user import SpecificBroadcaster, SpecificModerator, ToSpecificBroadcaster,\
+    FromSpecificBroadcaster
 # Libraries
 from typing import Literal
 
 
 class BaseShoutout(SpecificBroadcaster):
     viewer_count: int
     started_at: str
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/subscriptions.py` & `twitchify-1.1.0/twitch/types/eventsub/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,49 +31,87 @@
     Represents a subscription with a name and a version.
     """
     name: str
     version: str
 
 
 Subscriptions: Dict[str, SubscriptionPayload] = {
-    'channel_update': {'name': 'channel.update', 'version': '1'},
-    'follow': {'name': 'channel.follow', 'version': '2'},
-    'subscribe': {'name': 'channel.subscribe', 'version': '1'},
-    'subscription_end': {'name': 'channel.subscription.end', 'version': '1'},
-    'subscription_gift': {'name': 'channel.subscription.gift', 'version': '1'},
-    'subscription_message': {'name': 'channel.subscription.message', 'version': '1'},
-    'cheer': {'name': 'channel.cheer', 'version': '1'},
-    'raid': {'name': 'channel.raid', 'version': '1'},
-    'ban': {'name': 'channel.ban', 'version': '1'},
-    'unban': {'name': 'channel.unban', 'version': '1'},
-    'moderator_add': {'name': 'channel.moderator.add', 'version': '1'},
-    'moderator_remove': {'name': 'channel.moderator.remove', 'version': '1'},
-    'points_reward_add': {'name': 'channel.channel_points_custom_reward.add', 'version': '1'},
-    'points_reward_update': {'name': 'channel.channel_points_custom_reward.update', 'version': '1'},
-    'points_reward_remove': {'name': 'channel.channel_points_custom_reward.remove', 'version': '1'},
-    'points_reward_redemption': {'name': 'channel.channel_points_custom_reward_redemption.add', 'version': '1'},
-    'points_reward_redemption_update': {'name': 'channel.channel_points_custom_reward_redemption.update',
-                                        'version': '1'},
-    'poll_begin': {'name': 'channel.poll.begin', 'version': '1'},
-    'poll_progress': {'name': 'channel.poll.progress', 'version': '1'},
-    'poll_end': {'name': 'channel.poll.end', 'version': '1'},
-    'prediction_begin': {'name': 'channel.prediction.begin', 'version': '1'},
-    'prediction_progress': {'name': 'channel.prediction.progress', 'version': '1'},
-    'prediction_lock': {'name': 'channel.prediction.lock', 'version': '1'},
-    'prediction_end': {'name': 'channel.prediction.end', 'version': '1'},
-    'charity_campaign_donate': {'name': 'channel.charity_campaign.donate', 'version': '1'},
-    'charity_campaign_start': {'name': 'channel.charity_campaign.start', 'version': '1'},
-    'charity_campaign_progress': {'name': 'channel.charity_campaign.progress', 'version': '1'},
-    'charity_campaign_stop': {'name': 'channel.charity_campaign.stop', 'version': '1'},
-    'goal_begin': {'name': 'channel.goal.begin', 'version': '1'},
-    'goal_progress': {'name': 'channel.goal.progress', 'version': '1'},
-    'goal_end': {'name': 'channel.goal.end', 'version': '1'},
-    'hype_train_begin': {'name': 'channel.hype_train.begin', 'version': '1'},
-    'hype_train_progress': {'name': 'channel.hype_train.progress', 'version': '1'},
-    'hype_train_end': {'name': 'channel.hype_train.end', 'version': '1'},
-    'shield_mode_begin': {'name': 'channel.shield_mode.begin', 'version': '1'},
-    'shield_mode_end': {'name': 'channel.shield_mode.end', 'version': '1'},
-    'shoutout_create': {'name': 'channel.shoutout.create', 'version': '1'},
-    'shoutout_receive': {'name': 'channel.shoutout.receive', 'version': '1'},
-    'stream_online': {'name': 'stream.online', 'version': '1'},
-    'stream_offline': {'name': 'stream.offline', 'version': '1'},
-    'user_update': {'name': 'user.update', 'version': '1'}}
+    'channel_update':
+        {'name': 'channel.update', 'version': '1'},
+    'follow':
+        {'name': 'channel.follow', 'version': '2'},
+    'subscribe':
+        {'name': 'channel.subscribe', 'version': '1'},
+    'subscription_end':
+        {'name': 'channel.subscription.end', 'version': '1'},
+    'subscription_gift':
+        {'name': 'channel.subscription.gift', 'version': '1'},
+    'subscription_message':
+        {'name': 'channel.subscription.message', 'version': '1'},
+    'cheer':
+        {'name': 'channel.cheer', 'version': '1'},
+    'raid':
+        {'name': 'channel.raid', 'version': '1'},
+    'ban':
+        {'name': 'channel.ban', 'version': '1'},
+    'unban':
+        {'name': 'channel.unban', 'version': '1'},
+    'moderator_add':
+        {'name': 'channel.moderator.add', 'version': '1'},
+    'moderator_remove':
+        {'name': 'channel.moderator.remove', 'version': '1'},
+    'points_reward_add':
+        {'name': 'channel.channel_points_custom_reward.add', 'version': '1'},
+    'points_reward_update':
+        {'name': 'channel.channel_points_custom_reward.update', 'version': '1'},
+    'points_reward_remove':
+        {'name': 'channel.channel_points_custom_reward.remove', 'version': '1'},
+    'points_reward_redemption':
+        {'name': 'channel.channel_points_custom_reward_redemption.add', 'version': '1'},
+    'points_reward_redemption_update':
+        {'name': 'channel.channel_points_custom_reward_redemption.update', 'version': '1'},
+    'poll_begin':
+        {'name': 'channel.poll.begin', 'version': '1'},
+    'poll_progress':
+        {'name': 'channel.poll.progress', 'version': '1'},
+    'poll_end':
+        {'name': 'channel.poll.end', 'version': '1'},
+    'prediction_begin':
+        {'name': 'channel.prediction.begin', 'version': '1'},
+    'prediction_progress':
+        {'name': 'channel.prediction.progress', 'version': '1'},
+    'prediction_lock':
+        {'name': 'channel.prediction.lock', 'version': '1'},
+    'prediction_end':
+        {'name': 'channel.prediction.end', 'version': '1'},
+    'charity_campaign_donate':
+        {'name': 'channel.charity_campaign.donate', 'version': '1'},
+    'charity_campaign_start':
+        {'name': 'channel.charity_campaign.start', 'version': '1'},
+    'charity_campaign_progress':
+        {'name': 'channel.charity_campaign.progress', 'version': '1'},
+    'charity_campaign_stop':
+        {'name': 'channel.charity_campaign.stop', 'version': '1'},
+    'goal_begin':
+        {'name': 'channel.goal.begin', 'version': '1'},
+    'goal_progress':
+        {'name': 'channel.goal.progress', 'version': '1'},
+    'goal_end':
+        {'name': 'channel.goal.end', 'version': '1'},
+    'hype_train_begin':
+        {'name': 'channel.hype_train.begin', 'version': '1'},
+    'hype_train_progress':
+        {'name': 'channel.hype_train.progress', 'version': '1'},
+    'hype_train_end':
+        {'name': 'channel.hype_train.end', 'version': '1'},
+    'shield_mode_begin':
+        {'name': 'channel.shield_mode.begin', 'version': '1'},
+    'shield_mode_end':
+        {'name': 'channel.shield_mode.end', 'version': '1'},
+    'shoutout_create':
+        {'name': 'channel.shoutout.create', 'version': '1'},
+    'shoutout_receive':
+        {'name': 'channel.shoutout.receive', 'version': '1'},
+    'stream_online':
+        {'name': 'stream.online', 'version': '1'},
+    'stream_offline':
+        {'name': 'stream.offline', 'version': '1'}}
```

### Comparing `twitchify-1.0.5/twitch/types/eventsub/user.py` & `twitchify-1.1.0/twitch/types/eventsub/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/gateway.py` & `twitchify-1.1.0/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/http.py` & `twitchify-1.1.0/twitch/types/http.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/message.py` & `twitchify-1.1.0/twitch/types/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.5/twitch/types/user.py` & `twitchify-1.1.0/twitch/types/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,33 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 # Libraries
 from typing import TypedDict, Literal, Optional
 
+Types = Literal['admin', 'global_mod', 'staff', '']
+Tier = Literal['affiliate', 'partner', '']
+
+
+class UserImages(TypedDict):
+    profile_image_url: str
+    offline_image_url: str
+
+
+class UserType(UserImages):
+    id: str
+    login: str
+    display_name: str
+    email: str
+    type: Types
+    broadcaster_type: Tier
+    description: str
+    created_at: str
+
 
 class Broadcaster(TypedDict):
     broadcaster_id: str
     broadcaster_login: str
     broadcaster_name: str
 
 
@@ -62,40 +81,7 @@
     user_name: Optional[str]
 
 
 class SpecificUser(TypedDict):
     user_id: str
     user_login: str
     user_name: str
-
-
-class BaseUser(TypedDict):
-    """
-    Base user.
-    """
-    id: str
-    login: str
-    display_name: str
-
-
-_user_type = Literal['admin', 'global_mod', 'staff', '']
-_broadcaster_type = Literal['affiliate', 'partner', '']
-
-
-class UserPayload(BaseUser):
-    """
-    Represents a user.
-    """
-    type: _user_type
-    broadcaster_type: _broadcaster_type
-    description: str
-    profile_image_url: str
-    offline_image_url: str
-    view_count: int
-    created_at: str
-
-
-class UserPayloadWithEmail(UserPayload):
-    """
-    Represents a user with email.
-    """
-    email: str
```

### Comparing `twitchify-1.0.5/twitch/utils.py` & `twitchify-1.1.0/twitch/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,28 +25,69 @@
 from __future__ import annotations
 
 # Core
 from .types.eventsub.subscriptions import Subscriptions
 
 # Libraries
 from datetime import datetime
-import json
+from functools import wraps
 import logging
+import json
+import time
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionPayload
-    from typing import Optional, List
+    from typing import Optional, List, Callable, Awaitable, Any
 try:
     # noinspection PyPackageRequirements
     import orjson
 except ImportError:
     orjson = None
 
 
+def cache_decorator(expiry_seconds: int) -> Callable:
+    """
+    Cache decorator that caches the result of a function with a specified expiry time.
+
+    :param expiry_seconds: The number of seconds to cache the result.
+    :return: The decorated function.
+    """
+    cache = {}
+    cache_expiry = {}
+
+    def decorator(func: Callable[..., Awaitable[Any]]) -> Callable[..., Awaitable[Any]]:
+        """
+        Decorator function that wraps the original function with caching logic.
+
+        :param func: The original function to be decorated.
+        :return: The wrapped function.
+        """
+        @wraps(func)
+        async def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
+            """
+            Wrapper function that performs the caching logic before calling the original function.
+
+            :param self: The instance object.
+            :param args: The positional arguments passed to the function.
+            :param kwargs: The keyword arguments passed to the function.
+            :return: The result of the original function.
+            """
+            cache_key = (func.__name__, self, *args, frozenset(kwargs.items()))
+            if cache_key in cache and time.time() < cache_expiry[cache_key]:
+                return cache[cache_key]
+            result = await func(self, *args, **kwargs)
+            cache[cache_key] = result
+            cache_expiry[cache_key] = time.time() + expiry_seconds
+            return result
+        return wrapper
+
+    return decorator
+
+
 def to_json(text: str, encoding='utf-8') -> dict:
     """
     Converts the given text to a JSON object (dict) using the specified encoding.
 
     :param text:
      The text to convert to JSON.
 
@@ -58,21 +99,21 @@
 
     :raises UnicodeDecodeError: If the text cannot be decoded using the specified encoding.
     :raises json.JSONDecodeError: If the text is not valid JSON.
     """
     if orjson is not None:
         encoded_text = text.encode(encoding)
         return orjson.loads(encoded_text)  # type: ignore
-    else:
-        return json.loads(text)
+    return json.loads(text)
 
 
 def format_seconds(seconds: int) -> str:
     """
-    Formats the given number of seconds into a string representation of days, hours, minutes, and seconds.
+    Formats the given number of seconds into a string representation of days, hours, minutes,
+    and seconds.
 
     :param seconds:
      The number of seconds.
 
     :return:
      The formatted time string.
     """
@@ -105,19 +146,18 @@
 
     :return:
      The input text if it is not empty, or None if it is empty.
     """
 
     if text and text != '':
         return text
-    else:
-        return None
+    return None
 
 
-def parse_rfc3339_timestamp(*, timestamp: str) -> datetime:
+def parse_rfc3339_timestamp(timestamp: str) -> datetime:
     """
     Parses a string representing a timestamp in RFC3339 format and returns a datetime object.
 
     :param timestamp:
      The timestamp in RFC3339 format to be parsed.
 
     :return:
```

### Comparing `twitchify-1.0.5/twitchify.egg-info/PKG-INFO` & `twitchify-1.1.0/twitchify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.0.5/twitchify.egg-info/SOURCES.txt` & `twitchify-1.1.0/twitchify.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 twitch/__init__.py
+twitch/broadcaster.py
 twitch/channel.py
 twitch/client.py
 twitch/errors.py
 twitch/gateway.py
 twitch/goals.py
 twitch/http.py
 twitch/message.py
@@ -13,17 +14,19 @@
 twitch/reward.py
 twitch/state.py
 twitch/stream.py
 twitch/survey.py
 twitch/user.py
 twitch/utils.py
 twitch/types/__init__.py
+twitch/types/channel.py
 twitch/types/gateway.py
 twitch/types/http.py
 twitch/types/message.py
+twitch/types/stream.py
 twitch/types/user.py
 twitch/types/eventsub/__init__.py
 twitch/types/eventsub/channel.py
 twitch/types/eventsub/charity.py
 twitch/types/eventsub/goal.py
 twitch/types/eventsub/hypertrain.py
 twitch/types/eventsub/moderation.py
```

