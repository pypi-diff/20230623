# Comparing `tmp/google-chad-3.6.tar.gz` & `tmp/google-chad-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-3.6.tar", last modified: Thu May 25 10:39:58 2023, max compression
+gzip compressed data, was "google-chad-3.7.tar", last modified: Fri Jun 23 08:48:41 2023, max compression
```

## Comparing `google-chad-3.6.tar` & `google-chad-3.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.779649 google-chad-3.6/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-05-25 09:39:19.000000 google-chad-3.6/LICENSE
--rwxrwx---   0 root         (0) root         (0)      111 2023-05-25 09:39:19.000000 google-chad-3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10626 2023-05-25 10:39:58.775647 google-chad-3.6/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    10523 2023-05-25 09:55:01.000000 google-chad-3.6/README.md
--rwxrwx---   0 root         (0) root         (0)      912 2023-05-25 09:54:31.000000 google-chad-3.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:39:58.779649 google-chad-3.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/chad/
--rwxrwx---   0 root         (0) root         (0)        0 2023-05-25 09:39:19.000000 google-chad-3.6/src/chad/__init__.py
--rwxrwx---   0 root         (0) root         (0)    20062 2023-05-25 09:54:20.000000 google-chad-3.6/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/chad_extractor/
--rwxrwx---   0 root         (0) root         (0)        0 2023-05-25 09:39:19.000000 google-chad-3.6/src/chad_extractor/__init__.py
--rwxrwx---   0 root         (0) root         (0)    23026 2023-05-25 10:37:05.000000 google-chad-3.6/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/dorks/
--rwxrwx---   0 root         (0) root         (0)      237 2023-05-25 09:39:19.000000 google-chad-3.6/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/google_chad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10626 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-25 10:39:58.000000 google-chad-3.6/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:39:58.775647 google-chad-3.6/src/templates/
--rwxrwx---   0 root         (0) root         (0)     1747 2023-05-25 09:55:11.000000 google-chad-3.6/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-23 08:45:56.000000 google-chad-3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-23 08:45:56.000000 google-chad-3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11112 2023-06-23 08:48:41.139303 google-chad-3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-06-23 08:45:56.000000 google-chad-3.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      882 2023-06-23 08:45:56.000000 google-chad-3.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 08:48:41.139303 google-chad-3.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/chad/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 08:45:56.000000 google-chad-3.7/src/chad/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19486 2023-06-23 08:45:56.000000 google-chad-3.7/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/chad_extractor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 08:45:56.000000 google-chad-3.7/src/chad_extractor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23333 2023-06-23 08:45:56.000000 google-chad-3.7/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/dorks/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-23 08:45:56.000000 google-chad-3.7/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/google_chad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11112 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-23 08:48:41.000000 google-chad-3.7/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 08:48:41.139303 google-chad-3.7/src/templates/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-23 08:45:56.000000 google-chad-3.7/src/templates/social_media_template.json
```

### Comparing `google-chad-3.6/PKG-INFO` & `google-chad-3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.6
+Version: 3.7
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
-At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported on it. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
+At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
@@ -52,15 +52,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.7-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -83,72 +83,78 @@
 
 ## Chad Extractor
 
 Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
 
 ### Extracting and Validating Data
 
-Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag.
+Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag - where plaintext files will be treated as server responses and extraction logic will be immediately applied.
 
 ## Advanced Example: Social Media Takover
 
 Prepare Google Dorks as `social_media_dorks.txt` file:
 
 ```fundamental
 intext:"t.me/"
-intext:"discord.com/invite/"
+intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
 intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
 intext:"twitter.com/"
-intext:"instagram.com/"
 intext:"facebook.com/"
+intext:"instagram.com/"
+intext:"tiktok.com/"
 intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
 ```
 
 Prepare a template as `social_media_template.json` file:
 
 ```json
 {
    "telegram":{
-      "extract":"t\\.me\\/[\\w\\d\\-\\+]+",
+      "extract":"t\\.me\\/(?:(?!(?:share)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
    },
    "discord":{
-      "extract":"discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"discord\\.(?:com|gg)\\/invite\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"Invite Invalid"
    },
    "youtube":{
-      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available\\."
    },
    "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:explore|hashtag|home|i|intent|personalization|search|share|tos|widgets\\.js|[\\w]+\\/(?:privacy|tos))(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
+   "facebook":{
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer|share\\.php|terms\\.php)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available"
+   },
    "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"instagram\\.com\\/(?:(?!(?:about|accounts|ar|explore|p)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
-   "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available"
+   "tiktok":{
+      "extract":"(?<!vt\\.)tiktok\\.com\\/\\@[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://www.",
+      "validate":"Couldn't find this account"
    },
    "linkedin-company":{
-      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"Page not found"
    },
    "linkedin-user":{
-      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"An exact match for .+ could not be found\\."
    }
 }
 ```
 
 **Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
@@ -201,15 +207,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.6 ( github.com/ivan-sincek/chad )
+Chad v3.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -268,15 +274,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.6/README.md` & `google-chad-3.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,303 +1,309 @@
-# Chad
-
-Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
-
-At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported on it. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
-
-Tested on Kali Linux v2023.1 (64-bit).
-
-Made for educational purposes. I hope it will help!
-
-## Table of Contents
-
-* [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
-* [Shortest Possible](#shortest-possible)
-* [Basic Example: File Download](#basic-example-file-download)
-* [Chad Extractor](#chad-extractor)
-    * [Extracting and Validating Data)](#extracting-and-validating-data)
-* [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
-    * [Basic Use (Single Domain)](#basic-use-single-domain)
-    * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
-* [Rate Limiting](#rate-limiting)
-* [Usage](#usage)
-
-## How to Install
-
-```bash
-pip3 install google-chad
-
-pip3 install --upgrade google-chad
-
-playwright install chromium
-```
-
-## How to Build and Install Manually
-
-Run the following commands:
-
-```bash
-git clone https://github.com/ivan-sincek/chad && cd chad
-
-python3 -m pip install --upgrade build
-
-python3 -m build
-
-python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
-
-playwright install chromium
-```
-
-## Shortest Possible
-
-```bash
-chad -q 'intitle:"index of /" intext:"parent directory"'
-```
-
-## Basic Example: File Download
-
-Did you say Metagoofil?!
-
-```bash
-mkdir downloads
-
-chad -q "ext:pdf OR ext:docx OR ext:xlsx OR ext:pptx" -s *.example.com -tr 200 -d downloads -sos no
-```
-
-`-s <site>` is optional. For more information, see [Usage](#usage).
-
-Chad's file download feature is based on Python Requests library.
-
-## Chad Extractor
-
-Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
-
-### Extracting and Validating Data
-
-Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag.
-
-## Advanced Example: Social Media Takover
-
-Prepare Google Dorks as `social_media_dorks.txt` file:
-
-```fundamental
-intext:"t.me/"
-intext:"discord.com/invite/"
-intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
-intext:"twitter.com/"
-intext:"instagram.com/"
-intext:"facebook.com/"
-intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
-```
-
-Prepare a template as `social_media_template.json` file:
-
-```json
-{
-   "telegram":{
-      "extract":"t\\.me\\/[\\w\\d\\-\\+]+",
-      "extract_prepend":"https://",
-      "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
-   },
-   "discord":{
-      "extract":"discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"Invite Invalid"
-   },
-   "youtube":{
-      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available\\."
-   },
-   "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
-      "extract_prepend":"https://",
-      "validate":"This account doesn.?t exist"
-   },
-   "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "extract_append":"/",
-      "validate":"Sorry, this page isn't available\\."
-   },
-   "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available"
-   },
-   "linkedin-company":{
-      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://hr.",
-      "validate":"Page not found"
-   },
-   "linkedin-user":{
-      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://hr.",
-      "validate":"An exact match for .+ could not be found\\."
-   }
-}
-```
-
-**Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
-
-Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
-
-All regular expression searches are case-insensitive.
-
-Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
-
-To extract data without validating it, omit `validate` attributes from the template file as necessary.
-
-### Basic Use (Single Domain)
-
-```bash
-chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json -sos no
-
-chad-extractor -t social_media_template.json -res results.json -o results_report.json
-```
-
-### Advanced Use (Multiple Domains)
-
-Prepare sites/domains as `sites.txt` file:
-
-```fundamental
-*.example.com
-*.example.com -www
-```
-
-Prepare bot-safe User-Agents as `user_agents.txt` file, where `<your-api-key>` is your API key from [scrapeops.io](https://scrapeops.io):
-
-```python
-python3 -c 'import json, requests; open("user_agents.txt", "w").write(("\n").join(requests.get("http://headers.scrapeops.io/v1/user-agents?api_key=<your-api-key>&num_results=100", verify = False).json()["result"]))'
-```
-
-Automate:
-
-```bash
-mkdir results
-
-IFS=$'\n'; count=0; for site in $(cat sites.txt); do count=$((count+1)); echo "#${count} | ${site}"; chad -q social_media_dorks.txt -s "${site}" -tr 200 -a user_agents.txt -o "results/results_${count}.json"; done
-
-chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
-```
-
-## Rate Limiting
-
-Google's cooling-off period can be from a few hours to a whole day.
-
-To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
-
-Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
-
-## Usage
-
-```fundamental
-Chad v3.6 ( github.com/ivan-sincek/chad )
-
-Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
-Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
-
-DESCRIPTION
-    Search Google Dorks like Chad
-QUERIES
-    File with Google Dorks or a single query to use
-    -q <queries> - queries.txt | intext:password | "ext:tar OR ext:zip" | etc.
-SITE
-    Domain[s] to search
-    -s <site> - example.com | sub.example.com | *.example.com | "*.example.com -www" | etc.
-TIME
-    Get results not older than the specified time in months
-    -t <time> - 6 | 12 | 24 | etc.
-TOTAL RESULTS
-    Total number of unique results
-    Default: 100
-    -tr <total-results> - 200 | etc.
-PAGE RESULTS
-    Number of results per page - capped at 100 by Google
-    Default: randint(75, 100) per page
-    -pr <page-results> - 50 | etc.
-MINIMUM QUERIES
-    Minimum sleep between Google queries
-    Default: 75
-    -min-q <minimum-queries> - 120 | etc.
-MAXIMUM QUERIES
-    Maximum sleep between Google queries
-    Default: minimum + 50
-    -max-q <maximum-queries> - 180 | etc.
-MINIMUM PAGES
-    Minimum sleep between Google pages
-    Default: 15
-    -min-p <minimum-pages> - 30 | etc.
-MAXIMUM PAGES
-    Maximum sleep between Google pages
-    Default: minimum + 10
-    -max-p <maximum-pages> - 60 | etc.
-AGENTS
-    File with user agents to use
-    Default: nagooglesearch user agents
-    -a <agents> - user_agents.txt | etc.
-PROXIES
-    File with proxies to use
-    -p <proxies> - proxies.txt | etc.
-DIRECTORY
-    Downloads directory
-    All downloaded files will be saved in this directory
-    -d <directory> - downloads | etc.
-THREADS
-    Number of parallel files to download
-    Default: 5
-    -th <threads> - 20 | etc.
-OUT
-    Output file
-    -o <out> - results.json | etc.
-SLEEP ON START
-    Safety feature to prevent accidental rate limit triggering
-    -sos <sleep-on-start> - no 
-DEBUG
-    Debug output
-    -dbg <debug> - yes
-```
-
-```fundamental
-Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
-
-Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
-Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
-
-DESCRIPTION
-    Extract and validate data from Chad results or plaintext files
-TEMPLATE
-    JSON template file with extraction and validation information
-    -t <template> - template.json | etc.
-RESULTS DIRECTORY/FILE
-    Directory containing Chad results or plaintext files, or a single file
-    -res <results> - results | results.json | urls.txt | etc.
-PLAINTEXT
-    Parse files as plaintext
-    -pt <plaintext> - yes
-EXCLUDES
-    File with regular expressions or a single expression to exclude the page content
-    -e <excludes> - regexes.txt | "<div id=\"seo\">.+?<\/div>" | etc.
-THREADS
-    Number of parallel headless browsers to run
-    Default: 4
-    -th <threads> - 10 | etc.
-RETRIES
-    Number of retries per URL
-    Default: 2
-    -r <retries> - 5 | etc.
-WAIT
-    Wait before fetching the page content
-    Default: 4
-    -w <wait> - 10 | etc.
-AGENTS
-    File with user agents to use
-    Default: nagooglesearch user agents
-    -a <agents> - user_agents.txt | etc.
-OUT
-    Output file
-    -o <out> - results_report.json | etc.
-VERBOSE
-    Create additional supporting output files
-    -v <verbose> - yes
-```
+# Chad
+
+Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
+
+At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
+
+Tested on Kali Linux v2023.1 (64-bit).
+
+Made for educational purposes. I hope it will help!
+
+## Table of Contents
+
+* [How to Install](#how-to-install)
+* [How to Build and Install Manually](#how-to-build-and-install-manually)
+* [Shortest Possible](#shortest-possible)
+* [Basic Example: File Download](#basic-example-file-download)
+* [Chad Extractor](#chad-extractor)
+    * [Extracting and Validating Data)](#extracting-and-validating-data)
+* [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
+    * [Basic Use (Single Domain)](#basic-use-single-domain)
+    * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
+* [Rate Limiting](#rate-limiting)
+* [Usage](#usage)
+
+## How to Install
+
+```bash
+pip3 install google-chad
+
+pip3 install --upgrade google-chad
+
+playwright install chromium
+```
+
+## How to Build and Install Manually
+
+Run the following commands:
+
+```bash
+git clone https://github.com/ivan-sincek/chad && cd chad
+
+python3 -m pip install --upgrade build
+
+python3 -m build
+
+python3 -m pip install dist/google_chad-3.7-py3-none-any.whl
+
+playwright install chromium
+```
+
+## Shortest Possible
+
+```bash
+chad -q 'intitle:"index of /" intext:"parent directory"'
+```
+
+## Basic Example: File Download
+
+Did you say Metagoofil?!
+
+```bash
+mkdir downloads
+
+chad -q "ext:pdf OR ext:docx OR ext:xlsx OR ext:pptx" -s *.example.com -tr 200 -d downloads -sos no
+```
+
+`-s <site>` is optional. For more information, see [Usage](#usage).
+
+Chad's file download feature is based on Python Requests library.
+
+## Chad Extractor
+
+Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
+
+### Extracting and Validating Data
+
+Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag - where plaintext files will be treated as server responses and extraction logic will be immediately applied.
+
+## Advanced Example: Social Media Takover
+
+Prepare Google Dorks as `social_media_dorks.txt` file:
+
+```fundamental
+intext:"t.me/"
+intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
+intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
+intext:"twitter.com/"
+intext:"facebook.com/"
+intext:"instagram.com/"
+intext:"tiktok.com/"
+intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
+```
+
+Prepare a template as `social_media_template.json` file:
+
+```json
+{
+   "telegram":{
+      "extract":"t\\.me\\/(?:(?!(?:share)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
+   },
+   "discord":{
+      "extract":"discord\\.(?:com|gg)\\/invite\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"Invite Invalid"
+   },
+   "youtube":{
+      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available\\."
+   },
+   "twitter":{
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:explore|hashtag|home|i|intent|personalization|search|share|tos|widgets\\.js|[\\w]+\\/(?:privacy|tos))(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This account doesn.?t exist"
+   },
+   "facebook":{
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer|share\\.php|terms\\.php)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available"
+   },
+   "instagram":{
+      "extract":"instagram\\.com\\/(?:(?!(?:about|accounts|ar|explore|p)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "extract_append":"/",
+      "validate":"Sorry, this page isn't available\\."
+   },
+   "tiktok":{
+      "extract":"(?<!vt\\.)tiktok\\.com\\/\\@[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://www.",
+      "validate":"Couldn't find this account"
+   },
+   "linkedin-company":{
+      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://hr.",
+      "validate":"Page not found"
+   },
+   "linkedin-user":{
+      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://hr.",
+      "validate":"An exact match for .+ could not be found\\."
+   }
+}
+```
+
+**Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
+
+Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
+
+All regular expression searches are case-insensitive.
+
+Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
+
+To extract data without validating it, omit `validate` attributes from the template file as necessary.
+
+### Basic Use (Single Domain)
+
+```bash
+chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json -sos no
+
+chad-extractor -t social_media_template.json -res results.json -o results_report.json
+```
+
+### Advanced Use (Multiple Domains)
+
+Prepare sites/domains as `sites.txt` file:
+
+```fundamental
+*.example.com
+*.example.com -www
+```
+
+Prepare bot-safe User-Agents as `user_agents.txt` file, where `<your-api-key>` is your API key from [scrapeops.io](https://scrapeops.io):
+
+```python
+python3 -c 'import json, requests; open("user_agents.txt", "w").write(("\n").join(requests.get("http://headers.scrapeops.io/v1/user-agents?api_key=<your-api-key>&num_results=100", verify = False).json()["result"]))'
+```
+
+Automate:
+
+```bash
+mkdir results
+
+IFS=$'\n'; count=0; for site in $(cat sites.txt); do count=$((count+1)); echo "#${count} | ${site}"; chad -q social_media_dorks.txt -s "${site}" -tr 200 -a user_agents.txt -o "results/results_${count}.json"; done
+
+chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
+```
+
+## Rate Limiting
+
+Google's cooling-off period can be from a few hours to a whole day.
+
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
+
+Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
+
+## Usage
+
+```fundamental
+Chad v3.7 ( github.com/ivan-sincek/chad )
+
+Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
+Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
+
+DESCRIPTION
+    Search Google Dorks like Chad
+QUERIES
+    File with Google Dorks or a single query to use
+    -q <queries> - queries.txt | intext:password | "ext:tar OR ext:zip" | etc.
+SITE
+    Domain[s] to search
+    -s <site> - example.com | sub.example.com | *.example.com | "*.example.com -www" | etc.
+TIME
+    Get results not older than the specified time in months
+    -t <time> - 6 | 12 | 24 | etc.
+TOTAL RESULTS
+    Total number of unique results
+    Default: 100
+    -tr <total-results> - 200 | etc.
+PAGE RESULTS
+    Number of results per page - capped at 100 by Google
+    Default: randint(75, 100) per page
+    -pr <page-results> - 50 | etc.
+MINIMUM QUERIES
+    Minimum sleep between Google queries
+    Default: 75
+    -min-q <minimum-queries> - 120 | etc.
+MAXIMUM QUERIES
+    Maximum sleep between Google queries
+    Default: minimum + 50
+    -max-q <maximum-queries> - 180 | etc.
+MINIMUM PAGES
+    Minimum sleep between Google pages
+    Default: 15
+    -min-p <minimum-pages> - 30 | etc.
+MAXIMUM PAGES
+    Maximum sleep between Google pages
+    Default: minimum + 10
+    -max-p <maximum-pages> - 60 | etc.
+AGENTS
+    File with user agents to use
+    Default: nagooglesearch user agents
+    -a <agents> - user_agents.txt | etc.
+PROXIES
+    File with proxies to use
+    -p <proxies> - proxies.txt | etc.
+DIRECTORY
+    Downloads directory
+    All downloaded files will be saved in this directory
+    -d <directory> - downloads | etc.
+THREADS
+    Number of parallel files to download
+    Default: 5
+    -th <threads> - 20 | etc.
+OUT
+    Output file
+    -o <out> - results.json | etc.
+SLEEP ON START
+    Safety feature to prevent accidental rate limit triggering
+    -sos <sleep-on-start> - no 
+DEBUG
+    Debug output
+    -dbg <debug> - yes
+```
+
+```fundamental
+Chad Extractor v3.7 ( github.com/ivan-sincek/chad )
+
+Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
+Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
+
+DESCRIPTION
+    Extract and validate data from Chad results or plaintext files
+TEMPLATE
+    JSON template file with extraction and validation information
+    -t <template> - template.json | etc.
+RESULTS DIRECTORY/FILE
+    Directory containing Chad results or plaintext files, or a single file
+    -res <results> - results | results.json | urls.txt | etc.
+PLAINTEXT
+    Parse files as plaintext
+    -pt <plaintext> - yes
+EXCLUDES
+    File with regular expressions or a single expression to exclude the page content
+    -e <excludes> - regexes.txt | "<div id=\"seo\">.+?<\/div>" | etc.
+THREADS
+    Number of parallel headless browsers to run
+    Default: 4
+    -th <threads> - 10 | etc.
+RETRIES
+    Number of retries per URL
+    Default: 2
+    -r <retries> - 5 | etc.
+WAIT
+    Wait before fetching the page content
+    Default: 4
+    -w <wait> - 10 | etc.
+AGENTS
+    File with user agents to use
+    Default: nagooglesearch user agents
+    -a <agents> - user_agents.txt | etc.
+OUT
+    Output file
+    -o <out> - results_report.json | etc.
+VERBOSE
+    Create additional supporting output files
+    -v <verbose> - yes
+```
```

### Comparing `google-chad-3.6/src/google_chad.egg-info/PKG-INFO` & `google-chad-3.7/src/google_chad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.6
+Version: 3.7
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
-At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported on it. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
+At the moment, this tool cannot be installed on Windows OS because Python's `jq` library (required by Chad Extractor) is not supported. Although, [Chad](https://github.com/ivan-sincek/chad/blob/main/src/chad/chad.py) does in fact work on Windows OS - run it as a standalone script.
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
 
 ## Table of Contents
 
@@ -52,15 +52,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.6-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.7-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -83,72 +83,78 @@
 
 ## Chad Extractor
 
 Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
 
 ### Extracting and Validating Data
 
-Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag.
+Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag - where plaintext files will be treated as server responses and extraction logic will be immediately applied.
 
 ## Advanced Example: Social Media Takover
 
 Prepare Google Dorks as `social_media_dorks.txt` file:
 
 ```fundamental
 intext:"t.me/"
-intext:"discord.com/invite/"
+intext:"discord.com/invite/" OR intext:"discord.gg/invite/"
 intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
 intext:"twitter.com/"
-intext:"instagram.com/"
 intext:"facebook.com/"
+intext:"instagram.com/"
+intext:"tiktok.com/"
 intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
 ```
 
 Prepare a template as `social_media_template.json` file:
 
 ```json
 {
    "telegram":{
-      "extract":"t\\.me\\/[\\w\\d\\-\\+]+",
+      "extract":"t\\.me\\/(?:(?!(?:share)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
    },
    "discord":{
-      "extract":"discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"discord\\.(?:com|gg)\\/invite\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"Invite Invalid"
    },
    "youtube":{
-      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This page isn't available\\."
    },
    "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:explore|hashtag|home|i|intent|personalization|search|share|tos|widgets\\.js|[\\w]+\\/(?:privacy|tos))(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "validate":"This account doesn.?t exist"
    },
+   "facebook":{
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer|share\\.php|terms\\.php)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available"
+   },
    "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts|explore)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract":"instagram\\.com\\/(?:(?!(?:about|accounts|ar|explore|p)(?:$|(?:\\/|\\?)[^\\s]))[\\w\\d\\.\\_\\-\\+\\@]+)(?<!\\.)",
       "extract_prepend":"https://",
       "extract_append":"/",
       "validate":"Sorry, this page isn't available\\."
    },
-   "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available"
+   "tiktok":{
+      "extract":"(?<!vt\\.)tiktok\\.com\\/\\@[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
+      "extract_prepend":"https://www.",
+      "validate":"Couldn't find this account"
    },
    "linkedin-company":{
-      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"Page not found"
    },
    "linkedin-user":{
-      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\.\\_\\-\\+\\@]+(?<!\\.)",
       "extract_prepend":"https://hr.",
       "validate":"An exact match for .+ could not be found\\."
    }
 }
 ```
 
 **Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
@@ -201,15 +207,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.6 ( github.com/ivan-sincek/chad )
+Chad v3.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -268,15 +274,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.6 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.7 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

