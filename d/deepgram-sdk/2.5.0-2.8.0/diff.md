# Comparing `tmp/deepgram-sdk-2.5.0.tar.gz` & `tmp/deepgram-sdk-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-2.5.0.tar", last modified: Thu May 18 22:22:10 2023, max compression
+gzip compressed data, was "deepgram-sdk-2.8.0.tar", last modified: Fri Jun 23 16:46:06 2023, max compression
```

## Comparing `deepgram-sdk-2.5.0.tar` & `deepgram-sdk-2.8.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/deepgram/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/deepgram/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 22:22:10.000000 deepgram-sdk-2.5.0/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 22:22:10.513366 deepgram-sdk-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-18 22:21:52.000000 deepgram-sdk-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/mock_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/test_extra.py
```

### Comparing `deepgram-sdk-2.5.0/LICENSE` & `deepgram-sdk-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/PKG-INFO` & `deepgram-sdk-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.5.0
+Version: 2.8.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -12,20 +12,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Deepgram Python SDK
 
 [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/deepgram/deepgram-python-sdk/CI)](https://github.com/deepgram/deepgram-python-sdk/actions/workflows/CI.yml) [![PyPI](https://img.shields.io/pypi/v/deepgram-sdk)](https://pypi.org/project/deepgram-sdk/) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-rounded)](./.github/CODE_OF_CONDUCT.md)
 
-Official Python SDK for [Deepgram](https://www.deepgram.com/?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk)'s automated speech recognition APIs.
+Official Python SDK for [Deepgram](https://www.deepgram.com/). Start building with our powerful transcription & speech understanding API.
 
-To access the API you will need a Deepgram account. Sign up for free at
-[console.deepgram.com](https://console.deepgram.com/signup?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk).
+> This SDK only supports hosted usage of api.deepgram.com.
+## Getting an API Key
 
-You can learn more about the full Deepgram API at [developers.deepgram.com](https://developers.deepgram.com).
+🔑 To access the Deepgram API you will need a [free Deepgram API Key](https://console.deepgram.com/signup?jump=keys).
+## Documentation
+
+Complete documentation of the Python SDK can be found at [Deepgram Docs](https://developers.deepgram.com/docs/python-sdk).
+
+You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
 ## Getting Started
 
 ```sh
 pip install deepgram-sdk
 ```
 
@@ -105,15 +110,15 @@
     return
 
 # Listen for the connection to close
   deepgramLive.registerHandler(deepgramLive.event.CLOSE, lambda c: print(f'Connection closed with code {c}.'))
 
   # Listen for any transcripts received from Deepgram and write them to the console
   deepgramLive.registerHandler(deepgramLive.event.TRANSCRIPT_RECEIVED, print)
-  
+
   # Listen for the connection to open and send streaming audio from the URL to Deepgram
   async with aiohttp.ClientSession() as session:
     async with session.get(URL) as audio:
       while True:
         data = await audio.content.readany()
         deepgramLive.send(data)
 
@@ -148,28 +153,25 @@
 In the `sample-projects` folder, there are examples from four different Python web frameworks of how to do live streaming audio transcription with Deepgram. These include:
 
 - Flask 2.0
 - FastAPI
 - Django
 - Quart
 
-Each of the examples has a README file you can follow to set up and run your project. If you get stuck, please feel free to Tweet us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
 ## Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](./.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](./.github/CONTRIBUTING.md) guidelines for more information.
 
 ## Getting Help
 
 We love to hear from you so if you have questions, comments or find a bug in the
 project, let us know! You can either:
 
-- [Open an issue](https://github.com/deepgram/deepgram-python-sdk/issues/new) on this repository
-- Tweet at us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
-## Further Reading
+- [Open an issue in this repository](https://github.com/deepgram/deepgram-python-sdk/issues/new)
+- [Join the Deepgram Github Discussions Community](https://github.com/orgs/deepgram/discussions)
+- [Join the Deepgram Discord Community](https://discord.gg/xWRaCDBtW4)
 
-Check out the Developer Documentation at [https://developers.deepgram.com/](https://developers.deepgram.com/)
+[license]: LICENSE.txt
```

### Comparing `deepgram-sdk-2.5.0/README.md` & `deepgram-sdk-2.8.0/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,36 @@
+Metadata-Version: 2.1
+Name: deepgram-sdk
+Version: 2.8.0
+Summary: The official Python SDK for the Deepgram automated speech recognition platform.
+Home-page: https://github.com/deepgram/deepgram-python-sdk
+Author: Luca Todd
+Author-email: luca.todd@deepgram.com
+License: MIT
+Keywords: deepgram speech-to-text
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Deepgram Python SDK
 
 [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/deepgram/deepgram-python-sdk/CI)](https://github.com/deepgram/deepgram-python-sdk/actions/workflows/CI.yml) [![PyPI](https://img.shields.io/pypi/v/deepgram-sdk)](https://pypi.org/project/deepgram-sdk/) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-rounded)](./.github/CODE_OF_CONDUCT.md)
 
-Official Python SDK for [Deepgram](https://www.deepgram.com/?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk)'s automated speech recognition APIs.
+Official Python SDK for [Deepgram](https://www.deepgram.com/). Start building with our powerful transcription & speech understanding API.
+
+> This SDK only supports hosted usage of api.deepgram.com.
+## Getting an API Key
+
+🔑 To access the Deepgram API you will need a [free Deepgram API Key](https://console.deepgram.com/signup?jump=keys).
+## Documentation
 
-To access the API you will need a Deepgram account. Sign up for free at
-[console.deepgram.com](https://console.deepgram.com/signup?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk).
+Complete documentation of the Python SDK can be found at [Deepgram Docs](https://developers.deepgram.com/docs/python-sdk).
 
-You can learn more about the full Deepgram API at [developers.deepgram.com](https://developers.deepgram.com).
+You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
 ## Getting Started
 
 ```sh
 pip install deepgram-sdk
 ```
 
@@ -91,15 +110,15 @@
     return
 
 # Listen for the connection to close
   deepgramLive.registerHandler(deepgramLive.event.CLOSE, lambda c: print(f'Connection closed with code {c}.'))
 
   # Listen for any transcripts received from Deepgram and write them to the console
   deepgramLive.registerHandler(deepgramLive.event.TRANSCRIPT_RECEIVED, print)
-  
+
   # Listen for the connection to open and send streaming audio from the URL to Deepgram
   async with aiohttp.ClientSession() as session:
     async with session.get(URL) as audio:
       while True:
         data = await audio.content.readany()
         deepgramLive.send(data)
 
@@ -134,28 +153,25 @@
 In the `sample-projects` folder, there are examples from four different Python web frameworks of how to do live streaming audio transcription with Deepgram. These include:
 
 - Flask 2.0
 - FastAPI
 - Django
 - Quart
 
-Each of the examples has a README file you can follow to set up and run your project. If you get stuck, please feel free to Tweet us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
 ## Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](./.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](./.github/CONTRIBUTING.md) guidelines for more information.
 
 ## Getting Help
 
 We love to hear from you so if you have questions, comments or find a bug in the
 project, let us know! You can either:
 
-- [Open an issue](https://github.com/deepgram/deepgram-python-sdk/issues/new) on this repository
-- Tweet at us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
-## Further Reading
+- [Open an issue in this repository](https://github.com/deepgram/deepgram-python-sdk/issues/new)
+- [Join the Deepgram Github Discussions Community](https://github.com/orgs/deepgram/discussions)
+- [Join the Deepgram Discord Community](https://discord.gg/xWRaCDBtW4)
 
-Check out the Developer Documentation at [https://developers.deepgram.com/](https://developers.deepgram.com/)
+[license]: LICENSE.txt
```

### Comparing `deepgram-sdk-2.5.0/deepgram/__init__.py` & `deepgram-sdk-2.8.0/deepgram/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .transcription import Transcription
 from .projects import Projects
 from .usage import Usage
 from .billing import Billing
 from .members import Members
 from .scopes import Scopes
 from .invitations import Invitations
+from .extra import Extra
 
 
 class Deepgram:
     def __init__(self, options: Union[str, Options]) -> None:
         if not isinstance(options, str) and not options.get('api_url'):
             raise ValueError("DG: API URL must be valid or omitted")
         t_options: Options = {
@@ -49,10 +50,13 @@
     def scopes(self) -> Scopes:
         return Scopes(self.options)
 
     @property
     def invitations(self) -> Invitations:
         return Invitations(self.options)
 
+    @property
+    def extra(self) -> Extra:
+        return Extra(self.options)
 
 
 __all__ = ["Deepgram"]
```

### Comparing `deepgram-sdk-2.5.0/deepgram/_types.py` & `deepgram-sdk-2.8.0/deepgram/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     # numerals will be deprecated in the future
     numerals: bool
     numbers: bool
     numbers_spaces: bool
     search: List[str]
     callback: str
     keywords: List[str]
+    keyword_boost: str
     ner: str
     tier: str
     dates: bool
     date_format: str
     times: bool
     dictation: bool
     measurements: bool
@@ -84,15 +85,15 @@
 class PrerecordedOptions(TranscriptionOptions, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
     # https://developers.deepgram.com/documentation/features/
     utterances: bool
     utt_split: float
     detect_entities: bool
-    summarize: bool
+    summarize: Union[bool, str] 
     paragraphs: bool
     detect_language: bool
     detect_topics: bool
     translate: List[str]
     analyze_sentiment: bool
     sentiment: bool
     sentiment_threshold: float
@@ -203,27 +204,32 @@
     transcript: str
     words: List[WordBase]
     speaker: Optional[int]
     speaker_confidence: Optional[float]
     id: str
 
 
+class SummaryV2(TypedDict):
+    short: str
+
 class Metadata(TypedDict):
     request_id: str
     transaction_key: str
     sha256: str
     created: str
     duration: float
     channels: int
     models: List[str]
+    model_info: Dict[str, Any]
 
 
 TranscriptionResults = TypedDict('TranscriptionResults', {
     'channels': List[Channel],
-    'utterances': Optional[List[Utterance]]
+    'utterances': Optional[List[Utterance]],
+    'summary': Optional[SummaryV2],
 })
 
 
 class PrerecordedTranscriptionResponse(TypedDict, total=False):
     request_id: str
     metadata: Metadata
     results: TranscriptionResults
@@ -360,15 +366,15 @@
     diarize: bool
     detect_language: bool
     search: bool
     redact: bool
     alternatives: bool
     numerals: bool
     detect_entities: bool
-    summarize: bool
+    summarize: Union[bool, str] 
     paragraphs: bool
     detect_language: bool
     detect_topics: bool
     translate: bool
     analyze_sentiment: bool
     sentiment_threshold: float
```

### Comparing `deepgram-sdk-2.5.0/deepgram/_utils.py` & `deepgram-sdk-2.8.0/deepgram/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,26 +76,32 @@
     flattened: List[Tuple[str, str]] = sum(unflattened, [])
     return ('?' if flattened else '') + urllib.parse.urlencode(flattened)
 
 
 async def _request(
     path: str, options: Options,
     method: str = 'GET', payload: Payload = None,
-    headers: Optional[Mapping[str, str]] = None
+    headers: Optional[Mapping[str, str]] = None,
+    timeout: float = None,
 ) -> Any:
     if headers is None:
         headers = {}
     destination = cast(str, options.get('api_url', DEFAULT_ENDPOINT)) + path
     updated_headers = _prepare_headers(options, headers)
 
+    if timeout is None:
+        timeout = aiohttp.client.DEFAULT_TIMEOUT
+    else:
+        timeout = aiohttp.ClientTimeout(total=timeout)
+
     async def attempt():
         try:
             async with aiohttp.request(
                 method, destination, data=_normalize_payload(payload),
-                headers=updated_headers, raise_for_status=True
+                headers=updated_headers, raise_for_status=True, timeout=timeout
             ) as resp:
                 content = (await resp.text()).strip()
                 if not content:
                     return None
                 body = json.loads(content)
                 if body.get('error'):
                     raise Exception(f'DG: {content}')
@@ -118,29 +124,30 @@
             continue
     return await attempt()
 
 
 def _sync_request(
     path: str, options: Options,
     method: str = 'GET', payload: Payload = None,
-    headers: Optional[Mapping[str, str]] = None
+    headers: Optional[Mapping[str, str]] = None,
+    timeout: float = None
 ) -> Any:
     if headers is None:
         headers = {}
     destination = cast(str, options.get('api_url', DEFAULT_ENDPOINT)) + path
     updated_headers = _prepare_headers(options, headers)
 
     def attempt():
         req = urllib.request.Request(
             destination, 
             data=_normalize_payload(payload), 
             headers=updated_headers, 
             method=method)
         try:
-            with urllib.request.urlopen(req) as resp:
+            with urllib.request.urlopen(req, timeout=timeout) as resp:
                 content = resp.read().strip()
                 if not content:
                     return None
                 body = json.loads(content)
                 if body.get('error'):
                     raise Exception(f'DG: {content}')
                 return body
```

### Comparing `deepgram-sdk-2.5.0/deepgram/billing.py` & `deepgram-sdk-2.8.0/deepgram/billing.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/invitations.py` & `deepgram-sdk-2.8.0/deepgram/invitations.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/keys.py` & `deepgram-sdk-2.8.0/deepgram/keys.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/members.py` & `deepgram-sdk-2.8.0/deepgram/members.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/projects.py` & `deepgram-sdk-2.8.0/deepgram/projects.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/scopes.py` & `deepgram-sdk-2.8.0/deepgram/scopes.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram/transcription.py` & `deepgram-sdk-2.8.0/deepgram/transcription.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,40 +14,42 @@
 
 class PrerecordedTranscription:
     """This class provides an interface for doing transcription asynchronously on prerecorded audio files."""
 
     _root = "/listen"
 
     def __init__(self, options: Options,
-                 transcription_options: PrerecordedOptions) -> None:
+                 transcription_options: PrerecordedOptions, endpoint) -> None:
         """
         This function initializes the options and transcription_options for the PrerecordedTranscription class.
 
         :param options:Options: Used to Pass in the options for the transcription.
         :param transcription_options:PrerecordedOptions: Used to Specify the transcription options for a prerecorded audio file.
         :return: Nothing.
 
         """
-
         self.options = options
+        if endpoint is not None:
+            self._root = endpoint
         self.transcription_options = transcription_options
 
     async def __call__(
-        self, source: TranscriptionSource
+        self, source: TranscriptionSource, timeout: float = None
     ) -> PrerecordedTranscriptionResponse:
         """
         The __call__ function is a special method that allows the class to be called
         as a function. This is useful for creating instances of the class, where we can
         call `PrerecordedTranscription()` and pass in arguments to set up an instance of
         the class. For example:
         
             prerecorded_transcription = PrerecordedTranscription(...)
         
         :param source:TranscriptionSource: Used to Pass in the audio file.
-        :return: A `prerecordedtranscriptionresponse` object, which contains the transcription results.
+        :param timeout:float: (optional) The request timeout (if not set, defaults to `aiohttp`'s default timeout)
+        :return: A `PrerecordedTranscriptionResponse` object, which contains the transcription results.
         
         """
 
         if 'buffer' in source and 'mimetype' not in source:
             raise Exception(
                 'DG: Mimetype must be provided if the source is bytes'
             )
@@ -55,50 +57,54 @@
             Union[bytes, Dict],
             source.get('buffer', {'url': source.get('url')})
         )
         content_type = cast(str, source.get('mimetype', 'application/json'))
         return await _request(
             f'{self._root}{_make_query_string(self.transcription_options)}',
             self.options, method='POST', payload=payload,
-            headers={'Content-Type': content_type}
+            headers={'Content-Type': content_type},
+            timeout=timeout
         )
 
 
 class SyncPrerecordedTranscription:
     """This class provides an interface for doing transcription synchronously on prerecorded audio files."""
 
     _root = "/listen"
 
     def __init__(self, options: Options,
-                 transcription_options: PrerecordedOptions) -> None:
+                 transcription_options: PrerecordedOptions, endpoint) -> None:
         """
         This function initializes the options and transcription_options for the PrerecordedTranscription class.
 
         :param options:Options: Used to Pass in the options for the transcription.
         :param transcription_options:PrerecordedOptions: Used to Specify the transcription options for a prerecorded audio file.
         :return: Nothing.
 
         """
 
         self.options = options
+        if endpoint is not None:
+            self._root = endpoint
         self.transcription_options = transcription_options
 
     def __call__(
-        self, source: TranscriptionSource
+        self, source: TranscriptionSource, timeout: float = None
     ) -> PrerecordedTranscriptionResponse:
 
         """
         The __call__ function is a special method that allows the class to be called
         as a function. This is useful for creating instances of the class, where we can
         call `SyncPrerecordedTranscription()` and pass in arguments to set up an instance of
         the class. For example:
         
             sync_prerecorded_transcription = SyncPrerecordedTranscription(...)
         
         :param source:TranscriptionSource: Used to Pass in the audio file.
+        :param timeout:float: (optional) The request timeout, excluding the upload time of the audio file.
         :return: A `prerecordedtranscriptionresponse` object, which contains the transcription results.
         
         """
     
         if 'buffer' in source and 'mimetype' not in source:
             raise Exception(
                 'DG: Mimetype must be provided if the source is bytes'
@@ -107,43 +113,46 @@
             Union[bytes, Dict],
             source.get('buffer', {'url': source.get('url')})
         )
         content_type = cast(str, source.get('mimetype', 'application/json'))
         return _sync_request(
             f'{self._root}{_make_query_string(self.transcription_options)}',
             self.options, method='POST', payload=payload,
-            headers={'Content-Type': content_type}
+            headers={'Content-Type': content_type},
+            timeout=timeout
         )
 
 
 class LiveTranscription:
     """
     This class allows you to perform live transcription by connecting to Deepgram's Transcribe Streaming API.
     It takes in options for the transcription job, and a callback function to handle events.
 
     """
 
     _root = "/listen"
     MESSAGE_TIMEOUT = 1.0
 
     def __init__(self, options: Options,
-                 transcription_options: LiveOptions) -> None:
+                 transcription_options: LiveOptions, endpoint) -> None:
         """
         The __init__ function is called when an instance of the class is created.
         It initializes all of the attributes that are part of the object, and can be
         accessed using "self." notation. In this case, it sets up a list to store any
         messages received from Transcribe Streaming.
         
         :param options:Options: Used to Pass the options for the transcription job.
         :param transcription_options:LiveOptions: Used to Pass in the configuration for the transcription job.
         :return: None.
         
         """
 
         self.options = options
+        if endpoint is not None:
+            self._root = endpoint
         self.transcription_options = transcription_options
         self.handlers: List[Tuple[LiveTranscriptionEvent, EventHandler]] = []
         # all received messages
         self.received: List[Union[LiveTranscriptionResponse, Metadata]] = []
         # is the transcription job done?
         self.done = False
         self._socket = cast(websockets.client.WebSocketClientProtocol, None)
@@ -327,43 +336,49 @@
     """
     
     def __init__(self, options: Options) -> None:
         self.options = options
 
     async def prerecorded(
         self, source: TranscriptionSource,
-        options: PrerecordedOptions = None, **kwargs
+        options: PrerecordedOptions = None,
+        endpoint = "/listen",
+        timeout: float = None,
+        **kwargs
     ) -> PrerecordedTranscriptionResponse:
         """Retrieves a transcription for an already-existing audio file,
         local or web-hosted."""
         if options is None:
             options = {}
         full_options = cast(PrerecordedOptions, {**options, **kwargs})
         return await PrerecordedTranscription(
-            self.options, full_options
-        )(source)
+            self.options, full_options, endpoint
+        )(source, timeout=timeout)
 
 
     def sync_prerecorded(
         self, source: TranscriptionSource,
-        options: PrerecordedOptions = None, **kwargs
+        options: PrerecordedOptions = None,
+        endpoint = "/listen",
+        timeout: float = None,
+        **kwargs
     ) -> PrerecordedTranscriptionResponse:
         """Retrieves a transcription for an already-existing audio file,
         local or web-hosted."""
         if options is None:
             options = {}
         full_options = cast(PrerecordedOptions, {**options, **kwargs})
         return SyncPrerecordedTranscription(
-            self.options, full_options
-        )(source)
+            self.options, full_options, endpoint
+        )(source, timeout=timeout)
 
 
     async def live(
-        self, options: LiveOptions = None, **kwargs
+        self, options: LiveOptions = None, endpoint = "/listen", **kwargs
     ) -> LiveTranscription:
         """Provides a client to send raw audio data to be transcribed."""
         if options is None:
             options = {}
         full_options = cast(LiveOptions, {**options, **kwargs})
         return await LiveTranscription(
-            self.options, full_options
+            self.options, full_options, endpoint
         )()
```

### Comparing `deepgram-sdk-2.5.0/deepgram/usage.py` & `deepgram-sdk-2.8.0/deepgram/usage.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.5.0/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-2.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-Metadata-Version: 2.1
-Name: deepgram-sdk
-Version: 2.5.0
-Summary: The official Python SDK for the Deepgram automated speech recognition platform.
-Home-page: https://github.com/deepgram/deepgram-python-sdk
-Author: Luca Todd
-Author-email: luca.todd@deepgram.com
-License: MIT
-Keywords: deepgram speech-to-text
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Deepgram Python SDK
 
 [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/deepgram/deepgram-python-sdk/CI)](https://github.com/deepgram/deepgram-python-sdk/actions/workflows/CI.yml) [![PyPI](https://img.shields.io/pypi/v/deepgram-sdk)](https://pypi.org/project/deepgram-sdk/) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg?style=flat-rounded)](./.github/CODE_OF_CONDUCT.md)
 
-Official Python SDK for [Deepgram](https://www.deepgram.com/?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk)'s automated speech recognition APIs.
+Official Python SDK for [Deepgram](https://www.deepgram.com/). Start building with our powerful transcription & speech understanding API.
+
+> This SDK only supports hosted usage of api.deepgram.com.
+## Getting an API Key
+
+🔑 To access the Deepgram API you will need a [free Deepgram API Key](https://console.deepgram.com/signup?jump=keys).
+## Documentation
 
-To access the API you will need a Deepgram account. Sign up for free at
-[console.deepgram.com](https://console.deepgram.com/signup?utm_medium=github&utm_source=devrel&utm_content=deepgram-python-sdk).
+Complete documentation of the Python SDK can be found at [Deepgram Docs](https://developers.deepgram.com/docs/python-sdk).
 
-You can learn more about the full Deepgram API at [developers.deepgram.com](https://developers.deepgram.com).
+You can learn more about the Deepgram API at [developers.deepgram.com](https://developers.deepgram.com/docs).
 
 ## Getting Started
 
 ```sh
 pip install deepgram-sdk
 ```
 
@@ -105,15 +96,15 @@
     return
 
 # Listen for the connection to close
   deepgramLive.registerHandler(deepgramLive.event.CLOSE, lambda c: print(f'Connection closed with code {c}.'))
 
   # Listen for any transcripts received from Deepgram and write them to the console
   deepgramLive.registerHandler(deepgramLive.event.TRANSCRIPT_RECEIVED, print)
-  
+
   # Listen for the connection to open and send streaming audio from the URL to Deepgram
   async with aiohttp.ClientSession() as session:
     async with session.get(URL) as audio:
       while True:
         data = await audio.content.readany()
         deepgramLive.send(data)
 
@@ -148,28 +139,25 @@
 In the `sample-projects` folder, there are examples from four different Python web frameworks of how to do live streaming audio transcription with Deepgram. These include:
 
 - Flask 2.0
 - FastAPI
 - Django
 - Quart
 
-Each of the examples has a README file you can follow to set up and run your project. If you get stuck, please feel free to Tweet us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
 ## Development and Contributing
 
 Interested in contributing? We ❤️ pull requests!
 
 To make sure our community is safe for all, be sure to review and agree to our
 [Code of Conduct](./.github/CODE_OF_CONDUCT.md). Then see the
 [Contribution](./.github/CONTRIBUTING.md) guidelines for more information.
 
 ## Getting Help
 
 We love to hear from you so if you have questions, comments or find a bug in the
 project, let us know! You can either:
 
-- [Open an issue](https://github.com/deepgram/deepgram-python-sdk/issues/new) on this repository
-- Tweet at us! We're [@DeepgramAI on Twitter](https://twitter.com/DeepgramAI)
-
-## Further Reading
+- [Open an issue in this repository](https://github.com/deepgram/deepgram-python-sdk/issues/new)
+- [Join the Deepgram Github Discussions Community](https://github.com/orgs/deepgram/discussions)
+- [Join the Deepgram Discord Community](https://discord.gg/xWRaCDBtW4)
 
-Check out the Developer Documentation at [https://developers.deepgram.com/](https://developers.deepgram.com/)
+[license]: LICENSE.txt
```

### Comparing `deepgram-sdk-2.5.0/setup.py` & `deepgram-sdk-2.8.0/setup.py`

 * *Files identical despite different names*

