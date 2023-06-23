# Comparing `tmp/patreon-archiver-0.0.5.tar.gz` & `tmp/patreon_archiver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patreon-archiver-0.0.5.tar", last modified: Thu Jan 27 00:13:55 2022, max compression
+gzip compressed data, was "patreon_archiver-0.0.6.tar", max compression
```

## Comparing `patreon-archiver-0.0.5.tar` & `patreon_archiver-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,10 @@
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.326533 patreon-archiver-0.0.5/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      291 2022-01-24 23:32:51.000000 patreon-archiver-0.0.5/.gitignore
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      111 2022-01-24 20:21:48.000000 patreon-archiver-0.0.5/.isort.cfg
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       26 2022-01-24 20:21:53.000000 patreon-archiver-0.0.5/.prettierrc
--rw-r-----   0 tatsh     (1000) tatsh     (1000)    18283 2022-01-24 20:21:55.000000 patreon-archiver-0.0.5/.pylintrc
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      169 2022-01-24 20:22:01.000000 patreon-archiver-0.0.5/.readthedocs.yaml
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.324533 patreon-archiver-0.0.5/.stubs/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1282 2022-01-26 23:55:38.000000 patreon-archiver-0.0.5/.stubs/setuptools.pyi
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.324533 patreon-archiver-0.0.5/.stubs/yt_dlp/
--rwxr-xr-x   0 tatsh     (1000) tatsh     (1000)        0 2022-01-24 17:14:16.000000 patreon-archiver-0.0.5/.stubs/yt_dlp/__init__.pyi
--rwxr-xr-x   0 tatsh     (1000) tatsh     (1000)      339 2022-01-24 17:24:08.000000 patreon-archiver-0.0.5/.stubs/yt_dlp/cookies.pyi
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     7921 2022-01-24 20:21:58.000000 patreon-archiver-0.0.5/.style.yapf
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.324533 patreon-archiver-0.0.5/.vscode/
--rwxr-xr-x   0 tatsh     (1000) tatsh     (1000)      197 2022-01-24 20:06:17.000000 patreon-archiver-0.0.5/.vscode/settings.json
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1080 2022-01-27 00:00:54.000000 patreon-archiver-0.0.5/LICENSE.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1876 2022-01-27 00:13:55.326533 patreon-archiver-0.0.5/PKG-INFO
--rwxr-xr-x   0 tatsh     (1000) tatsh     (1000)     1532 2022-01-27 00:10:49.000000 patreon-archiver-0.0.5/README.md
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      925 2022-01-24 20:22:11.000000 patreon-archiver-0.0.5/mypy.ini
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.326533 patreon-archiver-0.0.5/patreon_archiver/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       44 2022-01-24 23:21:16.000000 patreon-archiver-0.0.5/patreon_archiver/__init__.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     2500 2022-01-26 23:43:21.000000 patreon-archiver-0.0.5/patreon_archiver/constants.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     4784 2022-01-26 23:46:48.000000 patreon-archiver-0.0.5/patreon_archiver/main.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      679 2022-01-26 23:41:51.000000 patreon-archiver-0.0.5/patreon_archiver/patreon_typing.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     2642 2022-01-26 23:43:07.000000 patreon-archiver-0.0.5/patreon_archiver/utils.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2022-01-27 00:13:55.326533 patreon-archiver-0.0.5/patreon_archiver.egg-info/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1876 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/PKG-INFO
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      608 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/SOURCES.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)        1 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/dependency_links.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       60 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/entry_points.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      106 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/requires.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       17 2022-01-27 00:13:55.000000 patreon-archiver-0.0.5/patreon_archiver.egg-info/top_level.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       43 2022-01-24 20:22:16.000000 patreon-archiver-0.0.5/pytest.ini
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       38 2022-01-27 00:13:55.326533 patreon-archiver-0.0.5/setup.cfg
--rwxr-xr-x   0 tatsh     (1000) tatsh     (1000)      924 2022-01-27 00:13:39.000000 patreon-archiver-0.0.5/setup.py
+-rw-r--r--   0        0        0     1080 2022-01-27 00:00:54.869085 patreon_archiver-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1609 2022-04-23 03:06:40.808397 patreon_archiver-0.0.6/README.md
+-rw-r--r--   0        0        0       44 2022-01-24 23:21:16.437539 patreon_archiver-0.0.6/patreon_archiver/__init__.py
+-rw-r--r--   0        0        0     2415 2023-04-26 06:28:41.963593 patreon_archiver-0.0.6/patreon_archiver/constants.py
+-rw-r--r--   0        0        0     6366 2023-06-23 05:08:45.488206 patreon_archiver-0.0.6/patreon_archiver/main.py
+-rw-r--r--   0        0        0     1286 2023-05-23 12:34:09.364870 patreon_archiver-0.0.6/patreon_archiver/patreon_typing.py
+-rw-r--r--   0        0        0      695 2023-04-26 06:19:47.794664 patreon_archiver-0.0.6/patreon_archiver/patreon_typing.ts
+-rw-r--r--   0        0        0     3284 2023-04-26 06:28:41.749593 patreon_archiver-0.0.6/patreon_archiver/utils.py
+-rw-r--r--   0        0        0      731 2023-06-23 05:11:05.917988 patreon_archiver-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 patreon_archiver-0.0.6/PKG-INFO
```

### Comparing `patreon-archiver-0.0.5/LICENSE.txt` & `patreon_archiver-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patreon-archiver-0.0.5/PKG-INFO` & `patreon_archiver-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: patreon-archiver
-Version: 0.0.5
-Summary: Archive Patreon content.
-Home-page: https://github.com/Tatsh/patreon-archiver
-Author: Andrew Udvare
-Author-email: audvare@gmail.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # Patreon Archiver
 
 Download Patreon content. Video content will be saved using yt-dlp. You
 should ensure that you are logged into Patreon in the appropriate browser
 profile.
 
 Recommendations in `~/.config/yt-dlp/config` or equivalent file:
@@ -52,20 +38,19 @@
   -o, --output-dir TEXT           Output directory
   -b, --browser TEXT              Browser to read cookies from
   -p, --profile TEXT              Browser profile
   -x, --fail                      Do not continue processing after a failed
                                   yt-dlp command.
   -L, --yt-dlp-arg-limit INTEGER  Number of media URIs to pass to yt-dlp at a
                                   time.
+  -S, --sleep-time INTEGER        Number of seconds to wait between requests
   -d, --debug                     Enable debug output
   --help                          Show this message and exit.
 ```
 
 ## How to get the campaign ID
 
 1. Go to the content creator's main page.
 2. View the source and search for `patreon-media/p/campaign/`.
 3. After the `/` there should be a number, as in
    `patreon-media/p/campaign/12345678`. In that case the campaign ID is
    `12345678`.
-
-
```

### Comparing `patreon-archiver-0.0.5/README.md` & `patreon_archiver-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: patreon-archiver
+Version: 0.0.6
+Summary: Save Patreon content you have access to.
+License: MIT
+Author: Andrew Udvare
+Author-email: audvare@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: mutagen (>=1.46.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: yt-dlp (>=2023.6.22,<2024.0.0)
+Description-Content-Type: text/markdown
+
 # Patreon Archiver
 
 Download Patreon content. Video content will be saved using yt-dlp. You
 should ensure that you are logged into Patreon in the appropriate browser
 profile.
 
 Recommendations in `~/.config/yt-dlp/config` or equivalent file:
@@ -38,18 +57,20 @@
   -o, --output-dir TEXT           Output directory
   -b, --browser TEXT              Browser to read cookies from
   -p, --profile TEXT              Browser profile
   -x, --fail                      Do not continue processing after a failed
                                   yt-dlp command.
   -L, --yt-dlp-arg-limit INTEGER  Number of media URIs to pass to yt-dlp at a
                                   time.
+  -S, --sleep-time INTEGER        Number of seconds to wait between requests
   -d, --debug                     Enable debug output
   --help                          Show this message and exit.
 ```
 
 ## How to get the campaign ID
 
 1. Go to the content creator's main page.
 2. View the source and search for `patreon-media/p/campaign/`.
 3. After the `/` there should be a number, as in
    `patreon-media/p/campaign/12345678`. In that case the campaign ID is
    `12345678`.
+
```

### Comparing `patreon-archiver-0.0.5/patreon_archiver/constants.py` & `patreon_archiver-0.0.6/patreon_archiver/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 from typing import Final, Mapping
 
 __all__ = ('FIELDS', 'MEDIA_URI', 'PATREON_API_URI', 'POSTS_URI',
-           'SHARED_HEADERS', 'USER_AGENT')
+           'SHARED_HEADERS', 'SHARED_PARAMS', 'USER_AGENT')
 
 PATREON_API_URI: Final[str] = 'https://www.patreon.com/api'
 MEDIA_URI: Final[str] = f'{PATREON_API_URI}/media'
 POSTS_URI: Final[str] = f'{PATREON_API_URI}/posts'
+USER_AGENT: Final[str] = 'Patreon/7.6.28 (Android; Android 11; Scale/2.10)'
+SHARED_HEADERS: Final[Mapping[str, str]] = {
+    'accept': '*/*',
+    'accept-language': 'en,en-GB;q=0.9,en-US;q=0.8',
+    'authority': 'www.patreon.com',
+    'cache-control': 'no-cache',
+    'content-type': 'application/vnd.api+json',
+    'dnt': '1',
+    'pragma': 'no-cache',
+    'referer': 'https://www.patreon.com/home',
+    'user-agent': USER_AGENT,
+}
 FIELDS: Final[Mapping[str, str]] = dict(
     campaign=','.join(
         ('avatar_photo_url', 'currency', 'earnings_visibility', 'is_monthly',
          'is_nsfw', 'name', 'show_audio_post_download_links', 'url')),
     post=','.join(
         ('change_visibility_at', 'comment_count', 'content',
          'current_user_can_comment', 'current_user_can_delete',
@@ -22,28 +34,14 @@
     post_tag=','.join(('tag_type', 'value')),
     user=','.join(('image_url', 'full_name', 'url')),
     access_rule=','.join(('access_rule_type', 'amount_cents')),
     media=','.join(
         ('download_url', 'file_name', 'id', 'image_urls', 'metadata')),
     contains_exclusive_posts='true',
     is_draft='false')
-USER_AGENT: Final[str] = ('Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 '
-                          '(KHTML, like Gecko) Chrome/100.0.4758.54 '
-                          'Safari/537.36')
-SHARED_HEADERS: Final[Mapping[str, str]] = {
-    'accept': '*/*',
-    'accept-language': 'en,en-GB;q=0.9,en-US;q=0.8',
-    'authority': 'www.patreon.com',
-    'cache-control': 'no-cache',
-    'content-type': 'application/vnd.api+json',
-    'dnt': '1',
-    'pragma': 'no-cache',
-    'referer': 'https://www.patreon.com/home',
-    'user-agent': USER_AGENT,
-}
 SHARED_PARAMS: Final[Mapping[str, str]] = {
     **dict(include=','.join((
         'access_rules',
         'attachments',
         'audio',
         'campaign',
         'images',
@@ -56,10 +54,12 @@
         'user',
         'user_defined_tags',
     )),
            sort='-published_at'),
     **{
         'json-api-version': '1.0',
     },
-    **{f'fields[{x}]': y
-       for x, y in FIELDS.items()}
+    **{
+        f'fields[{x}]': y
+        for x, y in FIELDS.items()
+    }
 }
```

### Comparing `patreon-archiver-0.0.5/patreon_archiver/main.py` & `patreon_archiver-0.0.6/patreon_archiver/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 from os import chdir, makedirs
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Iterator, TypedDict
 import json
-import subprocess as sp
+import sys
 
 from loguru import logger
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 from yt_dlp.cookies import extract_cookies_from_browser
 import click
 import requests
+import yt_dlp
 
 from .constants import MEDIA_URI, POSTS_URI, SHARED_HEADERS
-from .patreon_typing import PostDataDict, PostDataImageDict, PostsDict
-from .utils import (chunks, get_extension, get_shared_params, setup_logging,
-                    write_if_new)
+from .patreon_typing import MediaData, Posts, PostsData
+from .utils import (YoutubeDLLogger, chunks, get_extension, get_shared_params,
+                    setup_logging, unique_iter, write_if_new)
 
 __all__ = ('main',)
 
 
-def save_images(session: requests.Session, pdd: PostDataDict) -> None:
-    click.secho(f"Image file: {pdd['attributes']['url']}")
+class SaveInfo(TypedDict):
+    post_data_dict: PostsData
+    target_dir: Path
+
+
+def save_images(session: requests.Session, pdd: PostsData) -> SaveInfo:
+    click.secho(f'Image file: {pdd["attributes"]["url"]}')
     target_dir = Path('.', 'images', pdd['id'])
     makedirs(target_dir, exist_ok=True)
     write_if_new(target_dir.joinpath('post.json'),
                  f'{json.dumps(pdd, sort_keys=True, indent=2)}\n')
-    for index, id_ in enumerate(
-            pdd['attributes']['post_metadata']['image_order'], start=1):
-        with session.get(f'{MEDIA_URI}/{id_}') as r:
-            data: PostDataImageDict = r.json()['data']
-            with session.get(
-                    data['attributes']['image_urls']['original']) as r:
-                write_if_new(
-                    target_dir.joinpath(
-                        f'{index:02d}-{data["id"]}.' +
-                        get_extension(data["attributes"]["mimetype"])),
-                    r.content, 'wb')
+    assert pdd['attributes']['post_type'] == 'image_file'
+    if pdd['attributes']['post_metadata']:
+        for index, id_ in enumerate(
+                pdd['attributes']['post_metadata']['image_order'], start=1):
+            with session.get(f'{MEDIA_URI}/{id_}') as req:
+                data: MediaData = req.json()['data']
+                with session.get(
+                        data['attributes']['image_urls']['original']) as req:
+                    write_if_new(
+                        target_dir.joinpath(
+                            f'{index:02d}-{data["id"]}.' +
+                            get_extension(data['attributes']['mimetype'])),
+                        req.content, 'wb')
+    return SaveInfo(post_data_dict=pdd, target_dir=target_dir)
 
 
-def save_other(pdd: PostDataDict) -> None:
-    click.secho(f"{pdd['attributes']['post_type'].title()}: " +
+def save_other(pdd: PostsData) -> SaveInfo:
+    click.secho(f'{pdd["attributes"]["post_type"].title()}: ' +
                 pdd['attributes']['url'])
     other = Path('.', 'other')
     makedirs(other, exist_ok=True)
     write_if_new(
-        other.joinpath(f"{pdd['attributes']['post_type']}-{pdd['id']}.json"),
+        other.joinpath(f'{pdd["attributes"]["post_type"]}-{pdd["id"]}.json'),
         f'{json.dumps(pdd, sort_keys=True, indent=2)}\n')
+    return SaveInfo(post_data_dict=pdd, target_dir=other)
 
 
-def process_posts(posts: PostsDict, media_uris: List[str],
-                  session: requests.Session) -> None:
+def process_posts(posts: Posts,
+                  session: requests.Session) -> Iterator[str | SaveInfo]:
     for post in posts['data']:
         if (post['attributes']['post_type']
-                in ('audio_file', 'audio_embed', 'video_embed')):
-            media_uris.append(post['attributes']['url'])
+                in ('audio_file', 'audio_embed', 'video_embed',
+                    'video_external_file')):
+            yield post['attributes']['url']
         elif post['attributes']['post_type'] == 'image_file':
-            save_images(session, post)
+            yield from save_images(session, post)
         else:
-            save_other(post)
+            yield save_other(post)
 
 
 @click.command()
 @click.option('-o', '--output-dir', default=None, help='Output directory')
 @click.option('-b',
               '--browser',
               default='chrome',
@@ -71,52 +84,79 @@
               help=('Do not continue processing after a failed '
                     'yt-dlp command.'))
 @click.option('-L',
               '--yt-dlp-arg-limit',
               default=20,
               type=int,
               help='Number of media URIs to pass to yt-dlp at a time.')
+@click.option('-S',
+              '--sleep-time',
+              default=1,
+              type=int,
+              help='Number of seconds to wait between requests')
 @click.option('-d', '--debug', is_flag=True, help='Enable debug output')
 @click.argument('campaign_id')
-def main(output_dir: Optional[Union[Path, str]],
+def main(output_dir: Path | str | None,
          browser: str,
          profile: str,
          campaign_id: str,
          fail: bool = False,
          yt_dlp_arg_limit: int = 20,
+         sleep_time: int = 1,
          debug: bool = False) -> None:
     setup_logging(debug)
     if output_dir is None:
         output_dir = Path('.', campaign_id)
         makedirs(output_dir, exist_ok=True)
     chdir(output_dir)
     with requests.Session() as session:
-        session.headers.update({
-            **SHARED_HEADERS,
-            **dict(cookie='; '.join(f'{c.name}={c.value}' \
-                for c in extract_cookies_from_browser(browser, profile)
-                    if 'patreon.com' in c.domain))
-        })
-        with session.get(POSTS_URI,
-                         params=get_shared_params(campaign_id)) as r:
-            r.raise_for_status()
-            media_uris: List[str] = []
-            posts: PostsDict = r.json()
-            process_posts(posts, media_uris, session)
-            next_uri: Optional[str] = posts['links']['next']
-            logger.debug(f'Next URI: {next_uri}')
-            while next_uri:
-                with session.get(next_uri) as r:
-                    r.raise_for_status()
-                    posts = r.json()
-                    process_posts(posts, media_uris, session)
-                    try:
-                        next_uri = posts['links']['next']
-                        logger.debug(f'Next URI: {next_uri}')
-                    except KeyError:
-                        next_uri = None
-            for chunk in chunks(list(set(media_uris)), yt_dlp_arg_limit):
+        session.mount(
+            'https://',
+            HTTPAdapter(
+                max_retries=Retry(backoff_factor=2.5,
+                                  status_forcelist=[429, 500, 502, 503, 504])))
+        headers = dict(**SHARED_HEADERS)
+        cookies = '; '.join(f'{cookie.name}={cookie.value}' \
+                for cookie in extract_cookies_from_browser(browser, profile)
+                    if 'patreon.com' in cookie.domain)
+        session.headers.update({**headers, 'cookie': cookies})
+        try:
+            with session.get(POSTS_URI,
+                             params=get_shared_params(campaign_id)) as req:
+                req.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            logger.debug(f'JSON: {e.response.content}')
+            click.echo(
+                'Go to patreon.com and perform the verification, wait 30 seconds and try again.',
+                err=True)
+            raise click.Abort() from e
+        posts: Posts = req.json()
+        media_uris = list(
+            x for x in process_posts(posts, session) if isinstance(x, str))
+        next_uri = posts['links']['next']
+        logger.debug(f'Next URI: {next_uri}')
+        while next_uri:
+            with session.get(next_uri) as req:
+                req.raise_for_status()
+                posts = req.json()
+                media_uris.extend(x for x in process_posts(posts, session)
+                                  if isinstance(x, str))
                 try:
-                    sp.run(['yt-dlp'] + list(chunk), check=True)
-                except sp.CalledProcessError as e:
-                    if fail:
-                        raise click.Abort() from e
+                    next_uri = posts['links']['next']
+                    logger.debug(f'Next URI: {next_uri}')
+                except KeyError:
+                    next_uri = None
+        sys.argv = [sys.argv[0]]
+        ydl_opts = yt_dlp.parse_options()[-1]
+        ydl = yt_dlp.YoutubeDL({
+            **ydl_opts,
+            **dict(logger=YoutubeDLLogger(),
+                   sleep_interval_requests=sleep_time,
+                   verbose=debug)
+        })
+        for chunk in (list(x) for x in chunks(list(unique_iter(media_uris)),
+                                              yt_dlp_arg_limit)):
+            try:
+                ydl.download(chunk)
+            except Exception as e:  # pylint: disable=broad-except
+                if fail:
+                    raise click.Abort() from e
```

### Comparing `patreon-archiver-0.0.5/patreon_archiver/utils.py` & `patreon_archiver-0.0.6/patreon_archiver/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,116 @@
 from os.path import isfile
 from pathlib import Path
 from types import FrameType
-from typing import (Iterator, Literal, Mapping, Optional, Sequence, TypeVar,
-                    Union)
+from typing import (AnyStr, Iterable, Iterator, Literal as L, Mapping,
+                    Sequence, Set, TypeVar)
 import logging
 import sys
 
 from loguru import logger
 import click
 
 from .constants import FIELDS, SHARED_PARAMS
 
-__all__ = ('UnknownMimetypeError', 'chunks', 'get_extension',
-           'get_shared_params', 'write_if_new')
+__all__ = ('UnknownMimetypeError', 'YoutubeDLLogger', 'chunks',
+           'get_extension', 'get_shared_params', 'setup_logging',
+           'unique_iter', 'write_if_new')
 
 
-def write_if_new(target: Union[Path, str],
-                 content: Union[str, bytes],
-                 mode: str = 'w') -> None:
+def write_if_new(target: Path | str, content: AnyStr, mode: str = 'w') -> None:
     if not isfile(target):
         with click.open_file(str(target), mode) as f:
             f.write(content)
 
 
 class UnknownMimetypeError(Exception):
     pass
 
 
-def get_extension(mimetype: str) -> Literal['png', 'jpg']:
+def get_extension(mimetype: str) -> L['png', 'jpg']:
     if mimetype == 'image/jpeg':
         return 'jpg'
     if mimetype == 'image/png':
         return 'png'
     raise UnknownMimetypeError(mimetype)
 
 
 def get_shared_params(campaign_id: str) -> Mapping[str, str]:
     return {
         **SHARED_PARAMS,
-        **{f'fields[{x}]': y
-           for x, y in FIELDS.items()},
+        **{
+            f'fields[{x}]': y
+            for x, y in FIELDS.items()
+        },
         **{
             'filter[campaign_id]': campaign_id,
         },
     }
 
 
 T = TypeVar('T')
 
 
-def chunks(l: Sequence[T], n: int) -> Iterator[Iterator[T]]:
-    for i in range(0, len(l), n):
-        yield iter(l[i:i + n])
+def chunks(seq: Sequence[T], n: int) -> Iterator[Iterator[T]]:
+    for i in range(0, len(seq), n):
+        yield iter(seq[i:i + n])
 
 
 class InterceptHandler(logging.Handler):  # pragma: no cover
     """Intercept handler taken from Loguru's documentation."""
     def emit(self, record: logging.LogRecord) -> None:
-        level: Union[str, int]
+        level: str | int
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
         # Find caller from where originated the logged message
-        frame: Optional[FrameType] = logging.currentframe()
+        frame: FrameType | None = logging.currentframe()
         depth = 2
         while frame and frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage())
 
 
 def setup_log_intercept_handler() -> None:  # pragma: no cover
     """Sets up Loguru to intercept records from the logging module."""
     logging.basicConfig(handlers=(InterceptHandler(),), level=0)
 
 
-def setup_logging(debug: Optional[bool] = False) -> None:
+def setup_logging(debug: bool | None = False) -> None:
     """Shared function to enable logging."""
     if debug:  # pragma: no cover
         setup_log_intercept_handler()
         logger.enable('')
     else:
         logger.configure(handlers=(dict(
             format='<level>{message}</level>',
             level='INFO',
             sink=sys.stderr,
         ),))
+
+
+def unique_iter(seq: Iterable[T]) -> Iterator[T]:
+    """https://stackoverflow.com/a/480227/374110"""
+    seen: Set[T] = set()
+    seen_add = seen.add
+    return (x for x in seq if not (x in seen or seen_add(x)))
+
+
+class YoutubeDLLogger:
+    def debug(self, message: str) -> None:
+        if message.startswith('[debug] '):
+            logger.debug(message)
+        else:
+            logger.info(message)
+
+    def info(self, _: str) -> None:
+        pass
+
+    def warning(self, message: str) -> None:
+        logger.warning(message)
+
+    def error(self, message: str) -> None:
+        logger.error(message)
```

