# Comparing `tmp/eventregistry-9.0.tar.gz` & `tmp/eventregistry-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventregistry-9.0.tar", last modified: Mon May 15 10:33:01 2023, max compression
+gzip compressed data, was "eventregistry-9.1.tar", last modified: Fri Jun 23 08:41:19 2023, max compression
```

## Comparing `eventregistry-9.0.tar` & `eventregistry-9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.441188 eventregistry-9.0/
--rw-rw-rw-   0        0        0     1099 2016-03-26 08:55:17.000000 eventregistry-9.0/LICENSE
--rw-rw-rw-   0        0        0      712 2023-05-15 10:33:01.440187 eventregistry-9.0/PKG-INFO
--rw-rw-rw-   0        0        0     8181 2023-05-15 10:10:31.000000 eventregistry-9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.425172 eventregistry-9.0/eventregistry/
--rw-rw-rw-   0        0        0    10851 2023-04-03 08:02:00.000000 eventregistry-9.0/eventregistry/Analytics.py
--rw-rw-rw-   0        0        0    10060 2023-01-19 14:20:19.000000 eventregistry-9.0/eventregistry/Base.py
--rw-rw-rw-   0        0        0     4052 2023-03-23 11:29:32.000000 eventregistry-9.0/eventregistry/Counts.py
--rw-rw-rw-   0        0        0     2529 2023-01-19 08:55:17.000000 eventregistry-9.0/eventregistry/DailyShares.py
--rw-rw-rw-   0        0        0     2046 2023-01-19 08:56:51.000000 eventregistry-9.0/eventregistry/EventForText.py
--rw-rw-rw-   0        0        0    39635 2023-05-10 09:36:42.000000 eventregistry-9.0/eventregistry/EventRegistry.py
--rw-rw-rw-   0        0        0     3976 2023-01-19 08:59:06.000000 eventregistry-9.0/eventregistry/Info.py
--rw-rw-rw-   0        0        0      255 2022-03-11 10:55:55.000000 eventregistry-9.0/eventregistry/Logger.py
--rw-rw-rw-   0        0        0    16179 2023-05-10 09:57:48.000000 eventregistry-9.0/eventregistry/Query.py
--rw-rw-rw-   0        0        0     5481 2023-01-19 09:19:52.000000 eventregistry-9.0/eventregistry/QueryArticle.py
--rw-rw-rw-   0        0        0    40411 2023-04-04 09:59:02.000000 eventregistry-9.0/eventregistry/QueryArticles.py
--rw-rw-rw-   0        0        0    30185 2023-01-19 10:23:22.000000 eventregistry-9.0/eventregistry/QueryEvent.py
--rw-rw-rw-   0        0        0    35667 2023-03-30 14:36:40.000000 eventregistry-9.0/eventregistry/QueryEvents.py
--rw-rw-rw-   0        0        0    34065 2023-05-09 12:22:22.000000 eventregistry-9.0/eventregistry/QueryMentions.py
--rw-rw-rw-   0        0        0     7235 2023-01-19 13:28:14.000000 eventregistry-9.0/eventregistry/QueryStory.py
--rw-rw-rw-   0        0        0     4420 2023-01-19 13:29:26.000000 eventregistry-9.0/eventregistry/Recent.py
--rw-rw-rw-   0        0        0    24919 2023-05-15 09:21:43.000000 eventregistry-9.0/eventregistry/ReturnInfo.py
--rw-rw-rw-   0        0        0    19605 2023-01-19 13:38:39.000000 eventregistry-9.0/eventregistry/TopicPage.py
--rw-rw-rw-   0        0        0     4461 2023-01-19 13:40:32.000000 eventregistry-9.0/eventregistry/Trends.py
--rw-rw-rw-   0        0        0      755 2021-06-29 08:01:31.000000 eventregistry-9.0/eventregistry/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-15 10:32:18.000000 eventregistry-9.0/eventregistry/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.439194 eventregistry-9.0/eventregistry.egg-info/
--rw-rw-rw-   0        0        0      712 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2017-04-12 20:31:39.000000 eventregistry-9.0/eventregistry.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 10:33:01.441188 eventregistry-9.0/setup.cfg
--rw-rw-rw-   0        0        0     1313 2017-10-14 11:29:58.000000 eventregistry-9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:41:19.828487 eventregistry-9.1/
+-rw-rw-rw-   0        0        0     1099 2016-03-26 08:55:17.000000 eventregistry-9.1/LICENSE
+-rw-rw-rw-   0        0        0      712 2023-06-23 08:41:19.828487 eventregistry-9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8181 2023-05-15 10:10:31.000000 eventregistry-9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 08:41:19.821993 eventregistry-9.1/eventregistry/
+-rw-rw-rw-   0        0        0    10711 2023-06-16 06:13:47.000000 eventregistry-9.1/eventregistry/Analytics.py
+-rw-rw-rw-   0        0        0    10104 2023-06-16 07:25:47.000000 eventregistry-9.1/eventregistry/Base.py
+-rw-rw-rw-   0        0        0     4052 2023-03-23 11:29:32.000000 eventregistry-9.1/eventregistry/Counts.py
+-rw-rw-rw-   0        0        0     2670 2023-06-16 07:57:37.000000 eventregistry-9.1/eventregistry/DailyShares.py
+-rw-rw-rw-   0        0        0     2046 2023-01-19 08:56:51.000000 eventregistry-9.1/eventregistry/EventForText.py
+-rw-rw-rw-   0        0        0    39486 2023-06-16 06:56:43.000000 eventregistry-9.1/eventregistry/EventRegistry.py
+-rw-rw-rw-   0        0        0     3976 2023-01-19 08:59:06.000000 eventregistry-9.1/eventregistry/Info.py
+-rw-rw-rw-   0        0        0      255 2022-03-11 10:55:55.000000 eventregistry-9.1/eventregistry/Logger.py
+-rw-rw-rw-   0        0        0    16457 2023-06-16 07:50:43.000000 eventregistry-9.1/eventregistry/Query.py
+-rw-rw-rw-   0        0        0     5686 2023-06-16 07:32:28.000000 eventregistry-9.1/eventregistry/QueryArticle.py
+-rw-rw-rw-   0        0        0    42019 2023-06-23 08:18:00.000000 eventregistry-9.1/eventregistry/QueryArticles.py
+-rw-rw-rw-   0        0        0    31057 2023-06-23 08:21:04.000000 eventregistry-9.1/eventregistry/QueryEvent.py
+-rw-rw-rw-   0        0        0    37379 2023-06-23 08:19:35.000000 eventregistry-9.1/eventregistry/QueryEvents.py
+-rw-rw-rw-   0        0        0    34861 2023-06-16 07:46:25.000000 eventregistry-9.1/eventregistry/QueryMentions.py
+-rw-rw-rw-   0        0        0     7497 2023-06-16 07:47:55.000000 eventregistry-9.1/eventregistry/QueryStory.py
+-rw-rw-rw-   0        0        0     4440 2023-06-16 07:51:21.000000 eventregistry-9.1/eventregistry/Recent.py
+-rw-rw-rw-   0        0        0    24936 2023-06-16 07:52:28.000000 eventregistry-9.1/eventregistry/ReturnInfo.py
+-rw-rw-rw-   0        0        0    19739 2023-06-16 07:55:08.000000 eventregistry-9.1/eventregistry/TopicPage.py
+-rw-rw-rw-   0        0        0     4441 2023-06-16 07:56:06.000000 eventregistry-9.1/eventregistry/Trends.py
+-rw-rw-rw-   0        0        0      755 2021-06-29 08:01:31.000000 eventregistry-9.1/eventregistry/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-23 08:04:16.000000 eventregistry-9.1/eventregistry/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:41:19.827487 eventregistry-9.1/eventregistry.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-06-23 08:41:19.000000 eventregistry-9.1/eventregistry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2023-06-23 08:41:19.000000 eventregistry-9.1/eventregistry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:41:19.000000 eventregistry-9.1/eventregistry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2017-04-12 20:31:39.000000 eventregistry-9.1/eventregistry.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-06-23 08:41:19.000000 eventregistry-9.1/eventregistry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 08:41:19.000000 eventregistry-9.1/eventregistry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:41:19.829487 eventregistry-9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2017-10-14 11:29:58.000000 eventregistry-9.1/setup.py
```

### Comparing `eventregistry-9.0/LICENSE` & `eventregistry-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/PKG-INFO` & `eventregistry-9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventregistry
-Version: 9.0
+Version: 9.1
 Summary: A package that can be used to query information in Event Registry (http://eventregistry.org/)
 Home-page: https://github.com/EventRegistry/event-registry-python
 Author: Gregor Leban
 Author-email: gregor@eventregistry.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eventregistry-9.0/README.md` & `eventregistry-9.1/README.md`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/eventregistry/Analytics.py` & `eventregistry-9.1/eventregistry/Analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
     def __init__(self, eventRegistry: EventRegistry):
         """
         @param eventRegistry: instance of EventRegistry class
         """
         self._er = eventRegistry
 
 
-    def annotate(self, text: str, lang: str = None, customParams: dict = None):
+    def annotate(self, text: str, lang: Union[str, None] = None, customParams: Union[dict, None] = None):
         """
         identify the list of entities and nonentities mentioned in the text
         @param text: input text to annotate
         @param lang: language of the provided document (can be an ISO2 or ISO3 code). If None is provided, the language will be automatically detected
         @param customParams: None or a dict with custom parameters to send to the annotation service
         @returns: dict
         """
         params = {"lang": lang, "text": text}
         if customParams:
             params.update(customParams)
         return self._er.jsonRequestAnalytics("/api/v1/annotate", params)
 
 
-    def categorize(self, text: str, taxonomy: str = "dmoz", concepts: List[str] = None):
+    def categorize(self, text: str, taxonomy: str = "dmoz", concepts: Union[List[str], None] = None):
         """
         determine the set of up to 5 categories the text is about. Currently, only English text can be categorized!
         @param text: input text to categorize
         @param taxonomy: which taxonomy use for categorization. Options "dmoz" (over 5000 categories in 3 levels, English language only)
             or "news" (general news categorization, 9 categories, any langauge)
         @returns: dict
         """
@@ -82,15 +82,15 @@
         determine the language of the given text
         @param text: input text to analyze
         @returns: dict
         """
         return self._er.jsonRequestAnalytics("/api/v1/detectLanguage", { "text": text })
 
 
-    def extractArticleInfo(self, url: str, proxyUrl: str = None, headers: Union[str, dict] = None, cookies: Union[dict, str] = None):
+    def extractArticleInfo(self, url: str, proxyUrl: Union[str, None] = None, headers: Union[str, dict, None] = None, cookies: Union[dict, str, None] = None):
         """
         extract all available information about an article available at url `url`. Returned information will include
         article title, body, authors, links in the articles, ...
         @param url: article url to extract article information from
         @param proxyUrl: proxy that should be used for downloading article information. format: {schema}://{username}:{pass}@{proxy url/ip}
         @param headers: dict with headers to set in the request (optional)
         @param cookies: dict with cookies to set in the request (optional)
@@ -116,16 +116,16 @@
         @param text: text on wich to extract named entities
         @returns: dict
         """
         return self._er.jsonRequestAnalytics("/api/v1/ner", {"text": text})
 
 
     def trainTopicOnTweets(self, twitterQuery: str, useTweetText: bool = True, useIdfNormalization: bool = True,
-            normalization: bool = "linear", maxTweets: int = 2000, maxUsedLinks: int = 500, ignoreConceptTypes: Union[str, List[str]] = [],
-            maxConcepts: int = 20, maxCategories: int = 10, notifyEmailAddress: str = None):
+            normalization: str = "linear", maxTweets: int = 2000, maxUsedLinks: int = 500, ignoreConceptTypes: Union[str, List[str]] = [],
+            maxConcepts: int = 20, maxCategories: int = 10, notifyEmailAddress: Union[str, None] = None):
         """
         create a new topic and train it using the tweets that match the twitterQuery
         @param twitterQuery: string containing the content to search for. It can be a Twitter user account (using "@" prefix or user's Twitter url),
                 a hash tag (using "#" prefix) or a regular keyword.
         @param useTweetText: do you want to analyze the content of the tweets and extract the concepts mentioned in them? If False, only content shared
             in the articles in the user's tweets will be analyzed
         @param useIdfNormalization: normalize identified concepts by their IDF in the news (punish very common concepts)
@@ -171,19 +171,17 @@
         add the information extracted from the provided "text" to the topic with uri "uri"
         @param uri: uri of the topic (obtained by calling trainTopicCreateTopic method)
         @param text: text to analyze and extract information from
         """
         return self._er.jsonRequestAnalytics("/api/v1/trainTopic", { "action": "addDocument", "uri": uri, "text": text})
 
 
-    def trainTopicGetTrainedTopic(self, uri: str, maxConcepts: int = 20, maxCategories: int = 10,
-            ignoreConceptTypes: Union[str, List[str]] = [], idfNormalization: bool = True):
+    def trainTopicGetTrainedTopic(self, uri: str, maxConcepts: int = 20, maxCategories: int = 10, idfNormalization: bool = True):
         """
         retrieve topic for the topic for which you have already finished training
         @param uri: uri of the topic (obtained by calling trainTopicCreateTopic method)
         @param maxConcepts: number of top concepts to retrieve in the topic
         @param maxCategories: number of top categories to retrieve in the topic
-        @param ignoreConceptTypes: what types of concepts you would like to ignore in the profile. options: person, org, loc, wiki or an array with those
         @param idfNormalization: should the concepts be normalized by punishing the commonly mentioned concepts
         @param returns: returns the trained topic: { concepts: [], categories: [] }
         """
         return self._er.jsonRequestAnalytics("/api/v1/trainTopic", { "action": "getTrainedTopic", "uri": uri, "maxConcepts": maxConcepts, "maxCategories": maxCategories, "idfNormalization": idfNormalization })
```

### Comparing `eventregistry-9.0/eventregistry/Base.py` & `eventregistry-9.1/eventregistry/Base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿"""
 utility classes for Event Registry
 """
 
 import six, warnings, os, sys, re, datetime, time
 from eventregistry.Logger import logger
-from typing import Union, List
+from typing import Union, List, Dict
 
 mainLangs = ["eng", "deu", "zho", "slv", "spa"]
 allLangs = [ "eng", "deu", "spa", "cat", "por", "ita", "fra", "rus", "ara", "tur", "zho", "slv", "hrv", "srp" ]
 conceptTypes = ["loc", "person", "org", "keyword", "wiki", "conceptClass", "conceptFolder"]
 
 
 def deprecated(func):
@@ -119,41 +119,41 @@
     def encodeDate(val: Union[datetime.datetime, datetime.date, str]):
         """encode val that can be a date in different forms as a date that can be sent to Er"""
         if isinstance(val, datetime.datetime):
             return val.date().isoformat()
         elif isinstance(val, datetime.date):
             return val.isoformat()
         elif isinstance(val, six.string_types):
-            assert re.match("^\d{4}-\d{2}-\d{2}$", val), "date value '%s' was not provided in the 'YYYY-MM-DD' format" % (val)
+            assert re.match(r"^\d{4}-\d{2}-\d{2}$", val), f"date value '{val}' was not provided in the 'YYYY-MM-DD' format"
             return val
         raise AssertionError("date was not in the expected format")
 
 
     @staticmethod
     def encodeDateTime(val: Union[datetime.datetime, str]):
         """encode datetime into UTC ISO format which can be sent to ER"""
         if isinstance(val, datetime.datetime):
             # if we have a datetime in some tz, we convert it first to UTC
-            if val.utcoffset() != None:
+            if val.utcoffset() is not None:
                 import pytz
                 val = val.astimezone(pytz.utc)
             return val.isoformat()
         elif isinstance(val, six.string_types):
-            assert re.match("^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}(\.\d+)?$", val), "datetime value '%s' was not provided in the 'YYYY-MM-DDTHH:MM:SS.SSSS' format" % (val)
+            assert re.match(r"^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}(\.\d+)?$", val), f"datetime value '{val}' was not provided in the 'YYYY-MM-DDTHH:MM:SS.SSSS' format"
             return val
         raise AssertionError("datetime was not in the recognizable data type. Use datetime or string in ISO format")
 
 
     def _clearVal(self, propName: str):
         """remove the value of a property propName (if existing)"""
         if propName in self.queryParams:
             del self.queryParams[propName]
 
 
-    def _hasVal(self, propName: str):
+    def _hasVal(self, propName: str) -> bool:
         """do we have in the query property named propName"""
         return propName in self.queryParams
 
 
     def _setVal(self, propName: str, val):
         """set a value of a property in the query"""
         if isinstance(val, six.string_types):
@@ -184,58 +184,58 @@
                 val = val.encode("utf8")
             val = removeInvalidChars(val)
         if propName not in self.queryParams:
             self.queryParams[propName] = []
         self.queryParams[propName].append(val)
 
 
-    def _update(self, object: dict):
+    def _update(self, object: Dict):
         self.queryParams.update(object)
 
 
-    def _getQueryParams(self):
+    def _getQueryParams(self) -> Dict:
         """return the parameters."""
         return dict(self.queryParams)
 
 
-    def _setQueryArrVal(self, value: Union[str, QueryItems, list], propName: str, propOperName: str, defaultOperName: str):
+    def _setQueryArrVal(self, value: Union[str, QueryItems, List, None], propName: str, propOperName: Union[str, None], defaultOperName: str):
         """
         parse the value "value" and use it to set the property propName and the operator with name propOperName
         @param value: None, string, QueryItems or list. Values to be set using property name propName
         @param propOperName: property to set containing the "and" or "or". Relevant only if multiple items are provided in "value". Can be None if only one value is possible
         @param defaultOperName: which operator should be used in case "value" is a list. If a list, we will print also a warning to suggest use of QueryItems
         """
         # by default we have None - so don't do anything
         if value is None or value == "":
             return
         # if we have an instance of QueryItems then apply it
         if isinstance(value, QueryItems):
             self.queryParams[propName] = value.getItems()
             # if we need to specify the operator for the property
-            if propOperName != None:
+            if propOperName is not None:
                 self.queryParams[propOperName] = value.getOper().replace("$", "")
             # if the user specified the QueryItems class but used the invalid operator type then raise an error
-            assert propOperName != None or value.getOper().replace("$", "") == defaultOperName, "An invalid operator type '%s' was used for property '%s'" % (value.getOper().replace("$", ""), propName)
+            assert propOperName is not None or value.getOper().replace("$", "") == defaultOperName, "An invalid operator type '%s' was used for property '%s'" % (value.getOper().replace("$", ""), propName)
 
         # if we have a string value, just use it
         elif isinstance(value, six.string_types):
             self.queryParams[propName] = value
 
         # if we have a list, set it, but also weport
         elif isinstance(value, list):
             self.queryParams[propName] = value
             # if we need to specify the operator for the property
-            if propOperName != None:
+            if propOperName is not None:
                 self.queryParams[propOperName] = defaultOperName
                 if len(value) > 1:
-                    logger.warning("Warning: The value of parameter '%s' was provided as a list and '%s' operator was used implicitly between the items. We suggest specifying the list using the QueryItems.AND() or QueryItems.OR() to ensure the appropriate operator is used." % (propName, defaultOperName))
+                    logger.warning("Warning: The value of parameter '%s' was provided as a list and '%s' operator was used implicitly between the items. We suggest specifying the list using the QueryItems.AND() or QueryItems.OR() to ensure the appropriate operator is used.", propName, defaultOperName)
 
         # there should be no other valid types
         else:
-            assert False, "Parameter '%s' was of unsupported type. It should either be None, a string or an instance of QueryItems" % (propName)
+            assert False, f"Parameter '{propName}' was of unsupported type. It should either be None, a string or an instance of QueryItems"
 
 
 
 class Query(QueryParamsBase):
     def __init__(self):
         QueryParamsBase.__init__(self)
         self.resultTypeList = []
```

### Comparing `eventregistry-9.0/eventregistry/Counts.py` & `eventregistry-9.1/eventregistry/Counts.py`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/eventregistry/DailyShares.py` & `eventregistry-9.1/eventregistry/DailyShares.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 
 
 # get top shared articles for today or any other day
 class GetTopSharedArticles(QueryParamsBase):
     def __init__(self,
-                 date: str = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
+                 date: Union[str, datetime.date, datetime.datetime, None] = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
                  count: int = 20,      # number of top shared articles to return
                  returnInfo: ReturnInfo = ReturnInfo()):
         QueryParamsBase.__init__(self)
         self._setVal("action", "getArticles")
         self._setVal("resultType", "articles")
         self._setVal("articlesCount", count)
         self._setVal("articlesSortBy", "socialScore")
         self._update(returnInfo.getParams("articles"))
 
-        if date == None:
+        if date is None:
             date = datetime.date.today()
         self._setDateVal("dateStart", date)
         self._setDateVal("dateEnd", date)
 
 
     def _getPath(self):
         return "/api/v1/article"
 
 
 # get top shared events for today or any other day
 class GetTopSharedEvents(QueryParamsBase):
     def __init__(self,
-                 date: str = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
-                 count: int = 20,      # number of top shared articles to return
+                 date: Union[str, datetime.date, datetime.datetime, None] = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
+                 count: int = 20,                                                     # number of top shared articles to return
                  returnInfo: ReturnInfo = ReturnInfo()):
         QueryParamsBase.__init__(self)
         self._setVal("action", "getEvents")
         self._setVal("resultType", "events")
         self._setVal("eventsCount", count)
         self._setVal("eventsSortBy", "socialScore")
         self._update(returnInfo.getParams("events"))
 
-        if date == None:
+        if date is None:
             date = datetime.date.today()
         self._setDateVal("dateStart", date)
         self._setDateVal("dateEnd", date)
 
 
     def _getPath(self):
         return "/api/v1/event"
```

### Comparing `eventregistry-9.0/eventregistry/EventForText.py` & `eventregistry-9.1/eventregistry/EventForText.py`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/eventregistry/EventRegistry.py` & `eventregistry-9.1/eventregistry/EventRegistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 ﻿"""
 main class responsible for obtaining results from the Event Registry
 """
 import six, os, sys, traceback, json, re, requests, time, logging, threading
 
-from typing import Union, List
+from typing import Union, List, Tuple
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Logger import logger
 
 
 class EventRegistry(object):
     """
     the core object that is used to access any data in Event Registry
     it is used to send all the requests and queries
     """
     def __init__(self,
-                 apiKey: str = None,
-                 host: str = None,
-                 hostAnalytics: str = None,
+                 apiKey: Union[str, None] = None,
+                 host: Union[str, None] = None,
+                 hostAnalytics: Union[str, None] = None,
                  minDelayBetweenRequests: float = 0.5,
                  repeatFailedRequestCount: int = -1,
                  allowUseOfArchive: bool = True,
                  verboseOutput: bool = False,
-                 settingsFName: str = None):
+                 settingsFName: Union[str, None] = None):
         """
         @param apiKey: API key that should be used to make the requests to the Event Registry. API key is assigned to each user account and can be obtained on
             this page: https://newsapi.ai/dashboard
         @param host: host to use to access the Event Registry backend. Use None to use the default host.
         @param hostAnalytics: the host address to use to perform the analytics api calls
         @param minDelayBetweenRequests: the minimum number of seconds between individual api calls
         @param repeatFailedRequestCount: if a request fails (for example, because ER is down), what is the max number of times the request
@@ -34,16 +34,16 @@
         @param allowUseOfArchive: default is True. Determines if the queries made should potentially be executed on the archive data.
             If False, all queries (regardless how the date conditions are set) will be executed on data from the last 31 days.
             Queries executed on the archive are more expensive so set it to False if you are just interested in recent data
         @param verboseOutput: if True, additional info about errors etc will be printed to console
         @param settingsFName: If provided it should be a full path to 'settings.json' file where apiKey an/or host can be loaded from.
             If None, we will look for the settings file in the eventregistry module folder
         """
-        self._host = host
-        self._hostAnalytics = hostAnalytics
+        self._host = host or "http://eventregistry.org"
+        self._hostAnalytics = hostAnalytics or "http://analytics.eventregistry.org"
         self._lastException = None
         self._logRequests = False
         self._minDelayBetweenRequests = minDelayBetweenRequests
         self._repeatFailedRequestCount = repeatFailedRequestCount
         self._allowUseOfArchive = allowUseOfArchive
         self._verboseOutput = verboseOutput
         self._lastQueryTime = time.time()
@@ -68,24 +68,21 @@
             settings = json.load(open(settFName))
             self._host = host or settings.get("host", "http://eventregistry.org")
             self._hostAnalytics = hostAnalytics or settings.get("hostAnalytics", "http://analytics.eventregistry.org")
             # if api key is set, then use it when making the requests
             if "apiKey" in settings and not apiKey:
                 logger.debug("found apiKey in settings file which will be used for making requests")
                 self._apiKey = settings["apiKey"]
-        else:
-            self._host = host or "http://eventregistry.org"
-            self._hostAnalytics = hostAnalytics or "http://analytics.eventregistry.org"
 
         if self._apiKey == None:
             print("No API key was provided. You will be allowed to perform only a very limited number of requests per day.")
         self._requestLogFName = os.path.join(currPath, "requests_log.txt")
 
-        logger.debug("Event Registry host: %s" % (self._host))
-        logger.debug("Text analytics host: %s" % (self._hostAnalytics))
+        logger.debug("Event Registry host: %s", self._host)
+        logger.debug("Text analytics host: %s", self._hostAnalytics)
 
         # list of status codes - when we get them as a response from the call, we don't want to repeat the query as the response will likely always be the same
         self._stopStatusCodes = set([
             204,        # Information not available. Request succeeded, but the requested information is not available.
             400,        # Bad request. The request was unacceptable, most likely due to invalid or missing parameter.
             401,        # User's limit reached. The user reached the limit of the tokens in his account. The requests are rejected.
             403,        # Invalid account. The user's IP or account is disabled, potentially due to misuse.
@@ -102,15 +99,15 @@
                 return
             latestVersion = respInfo.text.strip()
             import eventregistry._version as _version
             currentVersion = _version.__version__
             for (latest, current) in zip(latestVersion.split("."), currentVersion.split(".")):
                 if int(latest) > int(current):
                     logger.info("==============\nYour version of the module is outdated, please update to the latest version")
-                    logger.info("Your version is %s while the latest is %s" % (currentVersion, latestVersion))
+                    logger.info("Your version is %s while the latest is %s", currentVersion, latestVersion)
                     logger.info("Update by calling: pip install --upgrade eventregistry\n==============")
                     return
                 # in case the server mistakenly has a lower version that the user has, don't report an error
                 elif int(latest) < int(current):
                     return
         except:
             pass
@@ -118,15 +115,15 @@
 
     def setLogging(self, val: bool):
         """should all requests be logged to a file or not?"""
         self._logRequests = val
 
 
     def setExtraParams(self, params: dict):
-        if params != None:
+        if params is not None:
             assert(isinstance(params, dict))
         self._extraParams = params
 
 
     def getHost(self):
         return self._host
 
@@ -171,18 +168,15 @@
         @param query: instance of Query class
         """
         assert isinstance(query, QueryParamsBase), "query parameter should be an instance of a class that has Query as a base class, such as QueryArticles or QueryEvents"
         import urllib
         # don't modify original query params
         allParams = query._getQueryParams()
         # make the url
-        try:
-            url = self._host + query._getPath() + "?" + urllib.urlencode(allParams, doseq=True)
-        except:
-            url = self._host + query._getPath() + "?" + urllib.parse.urlencode(allParams, doseq=True)
+        url = self._host + query._getPath() + "?" + urllib.parse.urlencode(allParams, doseq=True)
         return url
 
 
     def getLastHeaders(self):
         """
         return the headers returned in the response object of the last executed request
         """
@@ -196,27 +190,27 @@
         return self._headers.get(headerName, default)
 
 
     def printLastReqStats(self):
         """
         print some statistics about the last executed request
         """
-        print("Tokens used by the request: " + self.getLastHeader("req-tokens"))
-        print("Performed action: " + self.getLastHeader("req-action"))
+        print("Tokens used by the request: " + str(self.getLastHeader("req-tokens")))
+        print("Performed action: " + str(self.getLastHeader("req-action")))
         print("Was archive used for the query: " + (self.getLastHeader("req-archive") == "1" and "Yes" or "No"))
 
 
     def getLastReqArchiveUse(self):
         """
         return True or False depending on whether the last request used the archive or not
         """
         return self.getLastHeader("req-archive", "0") == "1"
 
 
-    def execQuery(self, query:QueryParamsBase, allowUseOfArchive: bool = None):
+    def execQuery(self, query:QueryParamsBase, allowUseOfArchive: Union[bool, None] = None):
         """
         main method for executing the search queries.
         @param query: instance of Query class
         @param allowUseOfArchive: potentially override the value set when constructing EventRegistry class.
             If not None set it to boolean to determine if the request can be executed on the archive data or not
             If left to None then the value set in the EventRegistry constructor will be used
         """
@@ -224,15 +218,15 @@
         # don't modify original query params
         allParams = query._getQueryParams()
         # make the request
         respInfo = self.jsonRequest(query._getPath(), allParams, allowUseOfArchive = allowUseOfArchive)
         return respInfo
 
 
-    def jsonRequest(self, methodUrl: str, paramDict: dict, customLogFName: str = None, allowUseOfArchive: bool = None):
+    def jsonRequest(self, methodUrl: str, paramDict: dict, customLogFName: Union[str, None] = None, allowUseOfArchive: Union[bool, None] = None):
         """
         make a request for json data. repeat it _repeatFailedRequestCount times, if they fail (indefinitely if _repeatFailedRequestCount = -1)
         @param methodUrl: url on er (e.g. "/api/v1/article")
         @param paramDict: optional object containing the parameters to include in the request (e.g. { "articleUri": "123412342" }).
         @param customLogFName: potentially a file name where the request information can be logged into
         @param allowUseOfArchive: potentially override the value set when constructing EventRegistry class.
             If not None set it to boolean to determine if the request can be executed on the archive data or not
@@ -240,32 +234,32 @@
         """
         self._sleepIfNecessary()
         self._lastException = None
 
         self._lock.acquire()
         if self._logRequests:
             try:
-                with open(customLogFName or self._requestLogFName, "a") as log:
-                    if paramDict != None:
+                with open(customLogFName or self._requestLogFName, "a", encoding="utf-8") as log:
+                    if isinstance(paramDict, dict):
                         log.write("# " + json.dumps(paramDict) + "\n")
                     log.write(methodUrl + "\n\n")
             except Exception as ex:
                 self._lastException = ex
 
-        if paramDict == None:
+        if paramDict is None:
             paramDict = {}
         # if we have api key then add it to the paramDict
         if self._apiKey:
             paramDict["apiKey"] = self._apiKey
         # if we want to ignore the archive, set the flag
-        if allowUseOfArchive != None:
+        if isinstance(allowUseOfArchive, bool):
             if not allowUseOfArchive:
                 paramDict["forceMaxDataTimeWindow"] = 31
         # if we didn't override the parameter then check what we've set when constructing the EventRegistry class
-        elif self._allowUseOfArchive == False:
+        elif self._allowUseOfArchive is False:
             paramDict["forceMaxDataTimeWindow"] = 31
         # if we also have some extra parameters, then set those too
         if self._extraParams:
             paramDict.update(self._extraParams)
 
         tryCount = 0
         self._headers = {}  # reset any past data
@@ -280,35 +274,35 @@
                 # remember the returned headers
                 self._headers = respInfo.headers
                 # if we got some error codes print the error and repeat the request after a short time period
                 if respInfo.status_code != 200:
                     raise Exception(respInfo.text)
                 # did we get a warning. if yes, print it
                 if self.getLastHeader("warning"):
-                    logger.warning("=========== WARNING ===========\n%s\n===============================" % (self.getLastHeader("warning")))
+                    logger.warning("=========== WARNING ===========\n%s\n===============================", self.getLastHeader("warning"))
                 # remember the available requests
                 self._dailyAvailableRequests = tryParseInt(self.getLastHeader("x-ratelimit-limit", ""), val = -1)
                 self._remainingAvailableRequests = tryParseInt(self.getLastHeader("x-ratelimit-remaining", ""), val = -1)
 
                 returnData = respInfo.json()
                 break
             except Exception as ex:
                 self._lastException = ex
                 if self._verboseOutput:
                     logger.error("Event Registry exception while executing the request:")
-                    logger.error("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
+                    logger.error("endpoint: %s\nParams: %s", url, json.dumps(paramDict, indent=4))
                     self.printLastException()
                 # in case of invalid input parameters, don't try to repeat the search but we simply raise the same exception again
-                if respInfo != None and respInfo.status_code in self._stopStatusCodes:
+                if respInfo is not None and respInfo.status_code in self._stopStatusCodes:
                     break
                 # in case of the other exceptions (maybe the service is temporarily unavailable) we try to repeat the query
                 logger.info("The request will be automatically repeated in 3 seconds...")
                 time.sleep(5)   # sleep for X seconds on error
         self._lock.release()
-        if returnData == None:
+        if returnData is None:
             raise self._lastException or Exception("No valid return data provided")
         return returnData
 
 
     def jsonRequestAnalytics(self, methodUrl: str, paramDict: dict):
         """
         call the analytics service to execute a method like annotation, categorization, etc.
@@ -330,30 +324,29 @@
                 # make the request
                 respInfo = self._reqSession.post(url, json = paramDict, timeout=60)
                 # remember the returned headers
                 self._headers = respInfo.headers
                 # if we got some error codes print the error and repeat the request after a short time period
                 if respInfo.status_code != 200:
                     raise Exception(respInfo.text)
-
                 returnData = respInfo.json()
                 break
             except Exception as ex:
                 self._lastException = ex
                 if self._verboseOutput:
                     logger.error("Event Registry Analytics exception while executing the request:")
-                    logger.error("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
+                    logger.error("endpoint: %s\nParams: %s", url, json.dumps(paramDict, indent=4))
                     self.printLastException()
                 # in case of invalid input parameters, don't try to repeat the search but we simply raise the same exception again
-                if respInfo != None and respInfo.status_code in self._stopStatusCodes:
+                if respInfo is not None and respInfo.status_code in self._stopStatusCodes:
                     break
                 logger.info("The request will be automatically repeated in 3 seconds...")
                 time.sleep(5)   # sleep for X seconds on error
         self._lock.release()
-        if returnData == None:
+        if returnData is None:
             raise self._lastException or Exception("No valid return data provided")
         return returnData
 
     #
     # suggestion methods - return type is a list of matching items
 
     def suggestConcepts(self, prefix: str, sources: Union[str, list] = ["concepts"], lang: str = "eng", conceptLang: str = "eng", page: int = 1, count: int = 20, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
@@ -413,15 +406,15 @@
         """
         assert page > 0, "page parameter should be above 0"
         params = { "prefix": prefix, "page": page, "count": count }
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestSourceGroups", params)
 
 
-    def suggestLocations(self, prefix: str, sources: Union[str, list] = ["place", "country"], lang: str = "eng", count: int = 20, countryUri: str = None, sortByDistanceTo: bool = None, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
+    def suggestLocations(self, prefix: str, sources: Union[str, list] = ["place", "country"], lang: str = "eng", count: int = 20, countryUri: Union[str, None] = None, sortByDistanceTo: Union[List, Tuple, None] = None, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of geo locations (cities or countries) that contain the prefix
         @param prefix: input text that should be contained in the location name
         @param source: what types of locations are we interested in. Possible options are "place" and "country"
         @param lang: language in which the prefix is specified
         @param count: number of returned suggestions
         @param countryUri: if provided, then return only those locations that are inside the specified country
@@ -435,24 +428,23 @@
             assert isinstance(sortByDistanceTo, (tuple, list)), "sortByDistanceTo has to contain a tuple with latitude and longitude of the location"
             assert len(sortByDistanceTo) == 2, "The sortByDistanceTo should contain two float numbers"
             params["closeToLat"] = sortByDistanceTo[0]
             params["closeToLon"] = sortByDistanceTo[1]
         return self.jsonRequest("/api/v1/suggestLocationsFast", params)
 
 
-    def suggestLocationsAtCoordinate(self, latitude: Union[int, float], longitude: Union[int, float], radiusKm: Union[int, float], limitToCities: bool = False, lang: str = "eng", count: int = 20, ignoreNonWiki: bool = True, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
+    def suggestLocationsAtCoordinate(self, latitude: Union[int, float], longitude: Union[int, float], radiusKm: Union[int, float], limitToCities: bool = False, lang: str = "eng", count: int = 20, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of geo locations (cities or places) that are close to the provided (lat, long) values
         @param latitude: latitude part of the coordinate
         @param longitude: longitude part of the coordinate
         @param radiusKm: radius in kilometres around the coordinates inside which the locations should be returned
         @param limitToCities: limit the set of results only to cities (True) or also to general places (False)
         @param lang: language in which the location label should be returned
         @param count: number of returned suggestions
-        @param ignoreNonWiki: ignore locations that don't have a wiki page and can not be used for concept search
         @param returnInfo: what details about locations should be included in the returned information
         """
         assert isinstance(latitude, (int, float)), "The 'latitude' should be a number"
         assert isinstance(longitude, (int, float)), "The 'longitude' should be a number"
         params = { "action": "getLocationsAtCoordinate", "lat": latitude, "lon": longitude, "radius": radiusKm, "limitToCities": limitToCities, "count": count, "lang": lang }
         params.update(returnInfo.getParams())
         params.update(kwargs)
@@ -570,15 +562,15 @@
         """
         matches = self.suggestConcepts(conceptLabel, lang = lang, sources = sources)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getLocationUri(self, locationLabel: str, lang: str = "eng", sources: Union[str, List[str]] = ["place", "country"], countryUri: str = None, sortByDistanceTo: str = None):
+    def getLocationUri(self, locationLabel: str, lang: str = "eng", sources: Union[str, List[str]] = ["place", "country"], countryUri: Union[str, None] = None, sortByDistanceTo: Union[List, Tuple, None] = None):
         """
         return a location uri that is the best match for the given location label
         @param locationLabel: partial or full location name for which to return the location uri
         @param sources: what types of locations are we interested in. Possible options are "place" and "country"
         @param countryUri: if set, then filter the possible locatiosn to the locations from that country
         @param sortByDistanceTo: sort candidates by distance to the given (lat, long) pair
         """
@@ -620,26 +612,26 @@
 
     def getSourceGroupUri(self, sourceGroupName: str):
         """
         return the URI of the source group that best matches the name
         @param sourceGroupName: partial or full name of the source group
         """
         matches = self.suggestSourceGroups(sourceGroupName)
-        if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
+        if matches is not None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
     def getConceptClassUri(self, classLabel: str, lang: str = "eng"):
         """
         return a uri of the concept class that is the best match for the given label
         @param classLabel: partial or full name of the concept class for which to return class uri
         """
         matches = self.suggestConceptClasses(classLabel, lang = lang)
-        if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
+        if matches is not None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
     def getConceptInfo(self, conceptUri: str,
                        returnInfo: ReturnInfo = ReturnInfo(conceptInfo = ConceptInfoFlags(synonyms = True, image = True, description = True))):
         """
@@ -655,26 +647,26 @@
     def getAuthorUri(self, authorName: str):
         """
         return author uri that is the best match for the given author name (and potentially source url)
         if there are multiple matches for the given author name, they are sorted based on the number of articles they have written (from most to least frequent)
         @param authorName: partial or full name of the author, potentially also containing the source url (e.g. "george brown nytimes")
         """
         matches = self.suggestAuthors(authorName)
-        if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
+        if matches is not None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
     def getEventTypeUri(self, eventTypeLabel: str):
         """
         return event type uri that is the best match for the given label
         @param eventTypeLabel: partial or full name of the event type for which we want to retrieve uri
         """
         matches = self.suggestEventTypes(eventTypeLabel)
-        if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
+        if matches is not None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
     @staticmethod
     def getUriFromUriWgt(uriWgtList: List[str]):
         """
```

### Comparing `eventregistry-9.0/eventregistry/Info.py` & `eventregistry-9.1/eventregistry/Info.py`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/eventregistry/Query.py` & `eventregistry-9.1/eventregistry/Query.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,37 +20,37 @@
         if value != defVal:
             self._queryObj[propName] = value
 
 
 
 class BaseQuery(_QueryCore):
     def __init__(self,
-                 keyword: Union[str, QueryItems] = None,
-                 conceptUri: Union[str, QueryItems] = None,
-                 categoryUri: Union[str, QueryItems] = None,
-                 sourceUri: Union[str, QueryItems] = None,
-                 locationUri: Union[str, QueryItems] = None,
-                 lang: Union[str, QueryItems] = None,
-                 dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                 dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-                 sourceLocationUri: Union[str, List[str]] = None,
-                 sourceGroupUri: Union[str, List[str]] = None,
+                 keyword: Union[str, QueryItems, None] = None,
+                 conceptUri: Union[str, QueryItems, None] = None,
+                 categoryUri: Union[str, QueryItems, None] = None,
+                 sourceUri: Union[str, QueryItems, None] = None,
+                 locationUri: Union[str, QueryItems, None] = None,
+                 lang: Union[str, QueryItems, None] = None,
+                 dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                 dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+                 sourceLocationUri: Union[str, List[str], None] = None,
+                 sourceGroupUri: Union[str, List[str], None] = None,
                  # article or event search only:
-                 dateMention: Union[datetime.datetime, datetime.date, str] = None,
-                 authorUri: Union[str, List[str]] = None,
+                 dateMention: Union[datetime.datetime, datetime.date, str, None] = None,
+                 authorUri: Union[str, List[str], None] = None,
                  keywordLoc: str = "body",
                  # event search only:
                  minMaxArticlesInEvent = None,
                  # mention search only:
-                 industryUri: Union[str, QueryItems] = None,
-                 sdgUri: Union[str, QueryItems] = None,
-                 sasbUri: Union[str, QueryItems] = None,
-                 esgUri: Union[str, QueryItems] = None,
+                 industryUri: Union[str, QueryItems, None] = None,
+                 sdgUri: Union[str, QueryItems, None] = None,
+                 sasbUri: Union[str, QueryItems, None] = None,
+                 esgUri: Union[str, QueryItems, None] = None,
                  # universal:
-                 exclude: Union["BaseQuery", "CombinedQuery"] = None):
+                 exclude: Union["BaseQuery", "CombinedQuery", None] = None):
         """
         @param keyword: keyword(s) to query. Either None, string or QueryItems instance
         @param conceptUri: concept(s) to query. Either None, string or QueryItems instance
         @param sourceUri: source(s) to query. Either None, string or QueryItems instance
         @param locationUri: location(s) to query. Either None, string or QueryItems instance
         @param categoryUri: categories to query. Either None, string or QueryItems instance
         @param lang: language(s) to query. Either None, string or QueryItems instance
@@ -70,22 +70,22 @@
         self._setQueryArrVal("conceptUri", conceptUri)
         self._setQueryArrVal("categoryUri", categoryUri)
         self._setQueryArrVal("sourceUri", sourceUri)
         self._setQueryArrVal("locationUri", locationUri)
         self._setQueryArrVal("lang", lang)
 
         # starting date of the published articles (e.g. 2014-05-02)
-        if dateStart != None:
+        if dateStart is not None:
             self._queryObj["dateStart"] = QueryParamsBase.encodeDate(dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
-        if dateEnd != None:
+        if dateEnd is not None:
             self._queryObj["dateEnd"] = QueryParamsBase.encodeDate(dateEnd)
 
         # mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMention != None:
+        if dateMention is not None:
             if isinstance(dateMention, list):
                 self._queryObj["dateMention"] = [QueryParamsBase.encodeDate(d) for d in dateMention]
             else:
                 self._queryObj["dateMention"] = QueryParamsBase.encodeDate(dateMention)
 
         self._setQueryArrVal("sourceLocationUri", sourceLocationUri)
         self._setQueryArrVal("sourceGroupUri", sourceGroupUri)
@@ -95,20 +95,20 @@
         self._setQueryArrVal("sdgUri", sdgUri)
         self._setQueryArrVal("sasbUri", sasbUri)
         self._setQueryArrVal("esgUri", esgUri)
 
         if keywordLoc != "body":
             self._queryObj["keywordLoc"] = keywordLoc
 
-        if minMaxArticlesInEvent != None:
+        if minMaxArticlesInEvent is not None:
             assert isinstance(minMaxArticlesInEvent, tuple), "minMaxArticlesInEvent parameter should either be None or a tuple with two integer values"
             self._queryObj["minArticlesInEvent"] = minMaxArticlesInEvent[0]
             self._queryObj["maxArticlesInEvent"] = minMaxArticlesInEvent[1]
 
-        if exclude != None:
+        if exclude is not None:
             assert isinstance(exclude, (CombinedQuery, BaseQuery)), "exclude parameter was not a CombinedQuery or BaseQuery instance"
             self._queryObj["$not"] = exclude.getQuery()
 
 
     def _setQueryArrVal(self, propName: str, value):
         # by default we have None - so don't do anything
         if value is None:
@@ -129,61 +129,61 @@
 class CombinedQuery(_QueryCore):
     def __init__(self):
         super(CombinedQuery, self).__init__()
 
 
     @staticmethod
     def AND(queryArr: List[Union["BaseQuery", "CombinedQuery"]],
-            exclude: Union["BaseQuery", "CombinedQuery"] = None):
+            exclude: Union["BaseQuery", "CombinedQuery", None] = None):
         """
         create a combined query with multiple items on which to perform an AND operation
         @param queryArr: a list of items on which to perform an AND operation. Items can be either a CombinedQuery or BaseQuery instances.
         @param exclude: a instance of BaseQuery, CombinedQuery or None. Used to filter out results matching the other criteria specified in this query
         """
         assert isinstance(queryArr, list), "provided argument as not a list"
         assert len(queryArr) > 0, "queryArr had an empty list"
         q = CombinedQuery()
         q.setQueryParam("$and", [])
         for item in queryArr:
             assert isinstance(item, (CombinedQuery, BaseQuery)), "item in the list was not a CombinedQuery or BaseQuery instance"
             q.getQuery()["$and"].append(item.getQuery())
-        if exclude != None:
+        if exclude is not None:
             assert isinstance(exclude, (CombinedQuery, BaseQuery)), "exclude parameter was not a CombinedQuery or BaseQuery instance"
             q.setQueryParam("$not", exclude.getQuery())
         return q
 
 
     @staticmethod
     def OR(queryArr: List[Union["BaseQuery", "CombinedQuery"]],
-           exclude: Union["BaseQuery", "CombinedQuery"] = None):
+           exclude: Union["BaseQuery", "CombinedQuery", None] = None):
         """
         create a combined query with multiple items on which to perform an OR operation
         @param queryArr: a list of items on which to perform an OR operation. Items can be either a CombinedQuery or BaseQuery instances.
         @param exclude: a instance of BaseQuery, CombinedQuery or None. Used to filter out results matching the other criteria specified in this query
         """
         assert isinstance(queryArr, list), "provided argument as not a list"
         assert len(queryArr) > 0, "queryArr had an empty list"
         q = CombinedQuery()
         q.setQueryParam("$or", [])
         for item in queryArr:
             assert isinstance(item, (CombinedQuery, BaseQuery)), "item in the list was not a CombinedQuery or BaseQuery instance"
             q.getQuery()["$or"].append(item.getQuery())
-        if exclude != None:
+        if exclude is not None:
             assert isinstance(exclude, (CombinedQuery, BaseQuery)), "exclude parameter was not a CombinedQuery or BaseQuery instance"
             q.setQueryParam("$not", exclude.getQuery())
         return q
 
 
 
 class ComplexArticleQuery(_QueryCore):
     def __init__(self,
                  query: Union["BaseQuery", "CombinedQuery"],
                  dataType: Union[str, List[str]] = "news",
-                 minSentiment: float = None,
-                 maxSentiment: float = None,
+                 minSentiment: Union[float, None] = None,
+                 maxSentiment: Union[float, None] = None,
                  minSocialScore: int = 0,
                  minFacebookShares: int = 0,
                  startSourceRankPercentile: int = 0,
                  endSourceRankPercentile: int = 100,
                  isDuplicateFilter: str = "keepAll",
                  hasDuplicateFilter: str = "keepAll",
                  eventFilter: str = "keepAll"):
@@ -216,17 +216,17 @@
 
         assert isinstance(query, (CombinedQuery, BaseQuery)), "query parameter was not a CombinedQuery or BaseQuery instance"
         self._queryObj["$query"] = query.getQuery()
         filter = {}
         if dataType != "news":
             filter["dataType"] = dataType
 
-        if minSentiment != None:
+        if minSentiment is not None:
             filter["minSentiment"] = minSentiment
-        if maxSentiment != None:
+        if maxSentiment is not None:
             filter["maxSentiment"] = maxSentiment
 
         if minSocialScore > 0:
             filter["minSocialScore"] = minSocialScore
         if minFacebookShares > 0:
             filter["minFacebookShares"] = minFacebookShares
         if startSourceRankPercentile != 0:
@@ -245,63 +245,63 @@
             self._queryObj["$filter"] = filter
 
 
 
 class ComplexEventQuery(_QueryCore):
     def __init__(self,
                 query: Union["BaseQuery", "CombinedQuery"],
-                minSentiment: float = None,
-                maxSentiment: float = None):
+                minSentiment: Union[float, None] = None,
+                maxSentiment: Union[float, None] = None):
         """
         create an event query using a complex query
         @param query: an instance of CombinedQuery or BaseQuery to use to find events that match the conditions
         """
         super(ComplexEventQuery, self).__init__()
 
         assert isinstance(query, (CombinedQuery, BaseQuery)), "query parameter was not a CombinedQuery or BaseQuery instance"
         filter = {}
-        if minSentiment != None:
+        if minSentiment is not None:
             filter["minSentiment"] = minSentiment
-        if maxSentiment != None:
+        if maxSentiment is not None:
             filter["maxSentiment"] = maxSentiment
 
         if len(filter) > 0:
             self._queryObj["$filter"] = filter
         self._queryObj["$query"] = query.getQuery()
 
 
 
 class ComplexMentionQuery(_QueryCore):
     def __init__(self,
                 query: Union["BaseQuery", "CombinedQuery"],
-                minSentiment: float = None,
-                maxSentiment: float = None,
-                minSentenceIndex: int = None,
-                maxSentenceIndex: int = None,
+                minSentiment: Union[float, None] = None,
+                maxSentiment: Union[float, None] = None,
+                minSentenceIndex: Union[int, None] = None,
+                maxSentenceIndex: Union[int, None] = None,
                 showDuplicates: bool = False):
         """
         create a mention query using a complex query
         @param query: an instance of CombinedQuery or BaseQuery to use to find events that match the conditions
         @param minSentiment: the minimum sentiment of the mentions to return
         @param maxSentiment: the maximum sentiment of the mentions to return
         @param minSentenceIndex: the minimum sentence index of the mentions to return
         @param maxSentenceIndex: the maximum sentence index of the mentions to return
         """
         super(ComplexMentionQuery, self).__init__()
 
         assert isinstance(query, (CombinedQuery, BaseQuery)), "query parameter was not a CombinedQuery or BaseQuery instance"
         filter = {}
-        if minSentiment != None:
+        if minSentiment is not None:
             filter["minSentiment"] = minSentiment
-        if maxSentiment != None:
+        if maxSentiment is not None:
             filter["maxSentiment"] = maxSentiment
 
-        if minSentenceIndex != None:
+        if minSentenceIndex is not None:
             filter["minSentenceIndex"] = minSentenceIndex
-        if maxSentenceIndex != None:
+        if maxSentenceIndex is not None:
             filter["maxSentenceIndex"] = maxSentenceIndex
         if showDuplicates:
             filter["showDuplicates"] = showDuplicates
 
         if len(filter) > 0:
             self._queryObj["$filter"] = filter
         self._queryObj["$query"] = query.getQuery()
```

### Comparing `eventregistry-9.0/eventregistry/QueryArticle.py` & `eventregistry-9.1/eventregistry/QueryArticle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from typing import List, Union
 
 class QueryArticle(Query):
     def __init__(self,
                  articleUriOrUriList: Union[str, List[str]],
-                 requestedResult: "RequestArticle" = None):
+                 requestedResult: Union["RequestArticle", None] = None):
         """
         Class for obtaining available info for one or more articles in the Event Registry
         @param articleUriOrUriList: a single article uri or a list of article uris
         @param requestedResult: the information to return as the result of the query. By default return the information about the article
         """
         super(QueryArticle, self).__init__()
         self._setVal("articleUri", articleUriOrUriList)
@@ -54,14 +54,15 @@
 
 class RequestArticleInfo(RequestArticle):
     def __init__(self, returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return details about the article
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticle, self).__init__()
         self.resultType = "info"
         self.__dict__.update(returnInfo.getParams("info"))
 
 
 
 class RequestArticleSimilarArticles(RequestArticle):
     def __init__(self,
@@ -74,14 +75,15 @@
         return a list of similar articles based on the CCA
         @param page: page of the articles
         @param count: number of articles to return (at most 200)
         @param lang: in which language(s) should be the similar articles
         @param limitPerLang: max number of articles per language to return (-1 for no limit)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticle, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 200, "at most 200 articles can be returned per call"
         self.resultType = "similarArticles"
         self.similarArticlesPage = page
         self.similarArticlesCount = count
         self.similarArticlesLang = lang
         self.similarArticlesLimitPerLang = limitPerLang
@@ -99,14 +101,15 @@
         return a list of duplicated articles of the current article
         @param page: page of the articles
         @param count: number of articles to return (at most 200)
         @param sortBy: how are the articles sorted. Options: id, date, cosSim, fq, socialScore, facebookShares, twitterShares
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticle, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 200, "at most 200 articles can be returned per call"
         self.resultType = "duplicatedArticles"
         self.duplicatedArticlesPage = page
         self.duplicatedArticlesCount = count
         self.duplicatedArticlesSortBy = sortBy
         self.duplicatedArticlesSortByAsc = sortByAsc
@@ -117,9 +120,10 @@
 class RequestArticleOriginalArticle(RequestArticle):
     def __init__(self,
                  returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return the article that is the original of the given article (the current article is a duplicate)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticle, self).__init__()
         self.resultType = "originalArticle"
         self.__dict__.update(returnInfo.getParams("originalArticle"))
```

### Comparing `eventregistry-9.0/eventregistry/QueryArticles.py` & `eventregistry-9.1/eventregistry/QueryArticles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Query import *
 from eventregistry.Logger import logger
 from eventregistry.EventRegistry import EventRegistry
-from typing import Union, List
+from typing import Union, List, Literal
 
 
 class QueryArticles(Query):
     def __init__(self,
-                keywords: Union[str, QueryItems] = None,
-                conceptUri: Union[str, QueryItems] = None,
-                categoryUri: Union[str, QueryItems] = None,
-                sourceUri: Union[str, QueryItems] = None,
-                sourceLocationUri: Union[str, QueryItems] = None,
-                sourceGroupUri: Union[str, QueryItems] = None,
-                authorUri: Union[str, QueryItems] = None,
-                locationUri: Union[str, QueryItems] = None,
-                lang: Union[str, QueryItems] = None,
-                dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                keywords: Union[str, QueryItems, None] = None,
+                conceptUri: Union[str, QueryItems, None] = None,
+                categoryUri: Union[str, QueryItems, None] = None,
+                sourceUri: Union[str, QueryItems, None] = None,
+                sourceLocationUri: Union[str, QueryItems, None] = None,
+                sourceGroupUri: Union[str, QueryItems, None] = None,
+                authorUri: Union[str, QueryItems, None] = None,
+                locationUri: Union[str, QueryItems, None] = None,
+                lang: Union[str, QueryItems, None] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str, None] = None,
                 keywordsLoc: str = "body",
+                keywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
 
-                ignoreKeywords: Union[str, QueryItems] = None,
-                ignoreConceptUri: Union[str, QueryItems] = None,
-                ignoreCategoryUri: Union[str, QueryItems] = None,
-                ignoreSourceUri: Union[str, QueryItems] = None,
-                ignoreSourceLocationUri: Union[str, QueryItems] = None,
-                ignoreSourceGroupUri: Union[str, QueryItems] = None,
-                ignoreAuthorUri: Union[str, QueryItems] = None,
-                ignoreLocationUri: Union[str, QueryItems] = None,
-                ignoreLang: Union[str, QueryItems] = None,
+                ignoreKeywords: Union[str, QueryItems, None] = None,
+                ignoreConceptUri: Union[str, QueryItems, None] = None,
+                ignoreCategoryUri: Union[str, QueryItems, None] = None,
+                ignoreSourceUri: Union[str, QueryItems, None] = None,
+                ignoreSourceLocationUri: Union[str, QueryItems, None] = None,
+                ignoreSourceGroupUri: Union[str, QueryItems, None] = None,
+                ignoreAuthorUri: Union[str, QueryItems, None] = None,
+                ignoreLocationUri: Union[str, QueryItems, None] = None,
+                ignoreLang: Union[str, QueryItems, None] = None,
                 ignoreKeywordsLoc: str = "body",
+                ignoreKeywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
 
                 isDuplicateFilter: str = "keepAll",
                 hasDuplicateFilter: str = "keepAll",
                 eventFilter: str = "keepAll",
                 authorsFilter: str = "keepAll",
                 videosFilter: str = "keepAll",
                 linksFilter: str = "keepAll",
                 startSourceRankPercentile: int = 0,
                 endSourceRankPercentile: int = 100,
                 minSentiment: float = -1,
                 maxSentiment: float = 1,
                 dataType: Union[str, List[str]] = "news",
-                requestedResult: "RequestArticles" = None):
+                requestedResult: Union["RequestArticles", None] = None):
         """
         Query class for searching for individual articles in the Event Registry.
         The resulting articles have to match all specified conditions. If a parameter value equals "" or [], then it is ignored.
         In order for query to be valid, it has to have at least one positive condition (condition that does not start with ignore*).
 
         @param keywords: find articles that mention the specified keywords.
             A single keyword/phrase can be provided as a string, multiple keywords/phrases can be provided as a list of strings.
@@ -81,25 +83,28 @@
         @param lang: find articles that are written in the specified language.
             If more than one language is specified, resulting articles has to be written in *any* of the languages.
         @param dateStart: find articles that were written on or after dateStart. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
         @param dateEnd: find articles that occurred before or on dateEnd. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
         @param dateMentionStart: find articles that explicitly mention a date that is equal or greater than dateMentionStart.
         @param dateMentionEnd: find articles that explicitly mention a date that is lower or equal to dateMentionEnd.
         @param keywordsLoc: where should we look when searching using the keywords provided by "keywords" parameter. "body" (default), "title", or "body,title"
+        @param keywordSearchMode: what search mode to use when specifying keywords. Possible values are: simple, exact, phrase
 
         @param ignoreKeywords: ignore articles that mention all provided keywords
         @param ignoreConceptUri: ignore articles that mention all provided concepts
         @param ignoreCategoryUri: ignore articles that are assigned to a particular category
         @param ignoreSourceUri: ignore articles that have been written by *any* of the specified news sources
         @param ignoreSourceLocationUri: ignore articles that have been written by sources located at *any* of the specified locations
         @param ignoreSourceGroupUri: ignore articles that have been written by sources in *any* of the specified source groups
         @param ignoreAuthorUri: ignore articles that were written by *any* of the specified authors
         @param ignoreLocationUri: ignore articles that occurred in any of the provided locations. A location can be a city or a place
         @param ignoreLang: ignore articles that are written in *any* of the provided languages
         @param ignoreKeywordsLoc: where should we look when data should be used when searching using the keywords provided by "ignoreKeywords" parameter. "body" (default), "title", or "body,title"
+        @param ignoreKeywordSearchMode: what search mode to use when specifying ignoreKeywords. Possible values are: simple, exact, phrase
+
         @param isDuplicateFilter: some articles can be duplicates of other articles. What should be done with them. Possible values are:
                 "skipDuplicates" (skip the resulting articles that are duplicates of other articles)
                 "keepOnlyDuplicates" (return only the duplicate articles)
                 "keepAll" (no filtering, default)
         @param hasDuplicateFilter: some articles are later copied by others. What should be done with such articles. Possible values are:
                 "skipHasDuplicates" (skip the resulting articles that have been later copied by others)
                 "keepOnlyHasDuplicates" (return only the articles that have been later copied by others)
@@ -128,14 +133,15 @@
         @param endSourceRankPercentile: ending percentile of the sources to consider in the results (default: 100). Value should be in range 10-100 and divisible by 10.
         @param minSentiment: minimum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all non-English articles)
         @param maxSentiment: maximum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all non-English articles)
         @param dataType: what data types should we search? "news" (news content, default), "pr" (press releases), or "blog".
                 If you want to use multiple data types, put them in an array (e.g. ["news", "pr"])
+
         @param requestedResult: the information to return as the result of the query. By default return the list of matching articles
         """
         super(QueryArticles, self).__init__()
         self._setVal("action", "getArticles")
 
         self._setQueryArrVal(keywords, "keyword", "keywordOper", "and")
         self._setQueryArrVal(conceptUri, "conceptUri", "conceptOper", "and")
@@ -145,41 +151,44 @@
         self._setQueryArrVal(sourceGroupUri, "sourceGroupUri", "sourceGroupOper", "or")
         self._setQueryArrVal(authorUri, "authorUri", "authorOper", "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
         self._setQueryArrVal(lang, "lang", None, "or")                      # a single lang or list (possible: eng, deu, spa, zho, slv)
 
         # starting date of the published articles (e.g. 2014-05-02)
-        if dateStart != None:
+        if dateStart is not None:
             self._setDateVal("dateStart", dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
-        if dateEnd != None:
+        if dateEnd is not None:
             self._setDateVal("dateEnd", dateEnd)
 
         # first valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionStart != None:
+        if dateMentionStart is not None:
             self._setDateVal("dateMentionStart", dateMentionStart)
         # last valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionEnd != None:
+        if dateMentionEnd is not None:
             self._setDateVal("dateMentionEnd", dateMentionEnd)
 
+        self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
+        self._setValIfNotDefault("keywordSearchMode", keywordSearchMode, "phrase")
+
         # for the negative conditions, only the OR is a valid operator type
         self._setQueryArrVal(ignoreKeywords, "ignoreKeyword", None, "or")
         self._setQueryArrVal(ignoreConceptUri, "ignoreConceptUri", None, "or")
         self._setQueryArrVal(ignoreCategoryUri, "ignoreCategoryUri", None, "or")
         self._setQueryArrVal(ignoreSourceUri, "ignoreSourceUri", None, "or")
         self._setQueryArrVal(ignoreSourceLocationUri, "ignoreSourceLocationUri", None, "or")
         self._setQueryArrVal(ignoreSourceGroupUri, "ignoreSourceGroupUri", None, "or")
         self._setQueryArrVal(ignoreAuthorUri, "ignoreAuthorUri", None, "or")
         self._setQueryArrVal(ignoreLocationUri, "ignoreLocationUri", None, "or")
 
         self._setQueryArrVal(ignoreLang, "ignoreLang", None, "or")
-
-        self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
         self._setValIfNotDefault("ignoreKeywordLoc", ignoreKeywordsLoc, "body")
+        self._setValIfNotDefault("ignoreKeywordSearchMode", ignoreKeywordSearchMode, "phrase")
+
 
         self._setValIfNotDefault("isDuplicateFilter", isDuplicateFilter, "keepAll")
         self._setValIfNotDefault("hasDuplicateFilter", hasDuplicateFilter, "keepAll")
         self._setValIfNotDefault("eventFilter", eventFilter, "keepAll")
         self._setValIfNotDefault("hasAuthorsFilter", authorsFilter, "keepAll")
         self._setValIfNotDefault("hasLinksFilter", linksFilter, "keepAll")
         self._setValIfNotDefault("hasVideosFilter", videosFilter, "keepAll")
@@ -213,27 +222,27 @@
         Result types can be the classes that extend RequestArticles base class (see classes below).
         """
         assert isinstance(requestArticles, RequestArticles), "QueryArticles class can only accept result requests that are of type RequestArticles"
         self.resultTypeList = [requestArticles]
 
 
     @staticmethod
-    def initWithArticleUriList(uriList: Union[str, List[str]], returnInfo: ReturnInfo = None):
+    def initWithArticleUriList(uriList: Union[str, List[str]], returnInfo: Union[ReturnInfo, None] = None):
         """
         instead of making a query, provide a list of article URIs manually, and then produce the desired results on top of them
         """
         # we need to set the dataType parameter here, otherwise users cannot ask for blog or pr articles using this way
-        q = QueryArticles(requestedResult=RequestArticlesInfo(returnInfo=returnInfo))
+        q = QueryArticles(requestedResult=RequestArticlesInfo(returnInfo = returnInfo))
         assert isinstance(uriList, str) or isinstance(uriList, list), "uriList has to be a list of strings or a string that represent article uris"
         q.queryParams = { "action": "getArticles", "articleUri": uriList, "dataType": ["news", "blog", "pr"] }
         return q
 
 
     @staticmethod
-    def initWithArticleUriWgtList(uriWgtList: Union[str, List[str]], returnInfo: ReturnInfo = None):
+    def initWithArticleUriWgtList(uriWgtList: Union[str, List[str]], returnInfo: Union[ReturnInfo, None] = None):
         """
         instead of making a query, provide a list of article URIs manually, and then produce the desired results on top of them
         """
         # we need to set the dataType parameter here, otherwise users cannot ask for blog or pr articles using this way
         q = QueryArticles(requestedResult=RequestArticlesInfo(returnInfo=returnInfo))
         if isinstance(uriWgtList, list):
             q.queryParams = { "action": "getArticles", "articleUriWgtList": ",".join(uriWgtList) }
@@ -285,15 +294,15 @@
         count = res.get("articles", {}).get("totalResults", 0)
         return count
 
 
     def execQuery(self, eventRegistry: EventRegistry,
                   sortBy: str = "rel",
                   sortByAsc: bool = False,
-                  returnInfo: ReturnInfo = None,
+                  returnInfo: Union[ReturnInfo, None] = None,
                   maxItems: int = -1,
                   **kwargs):
         """
         @param eventRegistry: instance of EventRegistry class. used to query new article list and uris
         @param sortBy: how are articles sorted. Options: date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -357,18 +366,18 @@
         # if we have already obtained all pages, then exit
         if self._totalPages != None and self._articlePage > self._totalPages:
             return
         self.setRequestedResult(RequestArticlesInfo(page=self._articlePage,
             sortBy=self._sortBy, sortByAsc=self._sortByAsc,
             returnInfo = self._returnInfo))
         if self._er._verboseOutput:
-            logger.debug("Downloading article page %d..." % (self._articlePage))
+            logger.debug("Downloading article page %d...", self._articlePage)
         res = self._er.execQuery(self)
         if "error" in res:
-            logger.error("Error while obtaining a list of articles: " + res["error"])
+            logger.error("Error while obtaining a list of articles: %s", res["error"])
         else:
             self._totalPages = res.get("articles", {}).get("pages", 0)
         results = res.get("articles", {}).get("results", [])
         self._articleList.extend(results)
 
 
     def __iter__(self):
@@ -400,38 +409,40 @@
 
 
 class RequestArticlesInfo(RequestArticles):
     def __init__(self,
                  page: int = 1,
                  count: int = 100,
                  sortBy: str = "date", sortByAsc: bool = False,
-                 returnInfo : ReturnInfo = None):
+                 returnInfo : Union[ReturnInfo, None] = None):
         """
         return article details for resulting articles
         @param page: page of the articles to return
         @param count: number of articles to return for the given page (at most 100)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 200, "at most 100 articles can be returned per call"
         self.resultType = "articles"
         self.articlesPage = page
         self.articlesCount = count
         self.articlesSortBy = sortBy
         self.articlesSortByAsc = sortByAsc
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("articles"))
 
 
     def setPage(self, page: int):
         """
         set the page of results to obtain
         """
+        super(RequestArticles, self).__init__()
         assert page >= 1, "page has to be >= 1"
         self.articlesPage = page
 
 
 
 class RequestArticlesUriWgtList(RequestArticles):
     def __init__(self,
@@ -441,14 +452,15 @@
         """
         return a list of article uris together with the scores
         @param page: page of the results (1, 2, ...)
         @param count: number of items to return in a single query (at most 50000)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False) according to the sortBy criteria
         """
+        super(RequestArticles, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 50000
         self.resultType = "uriWgtList"
         self.uriWgtListPage = page
         self.uriWgtListCount = count
         self.uriWgtListSortBy = sortBy
         self.uriWgtListSortByAsc = sortByAsc
@@ -461,37 +473,39 @@
 
 
 class RequestArticlesTimeAggr(RequestArticles):
     def __init__(self):
         """
         return time distribution of resulting articles
         """
+        super(RequestArticles, self).__init__()
         self.resultType = "timeAggr"
 
 
 
 class RequestArticlesConceptAggr(RequestArticles):
     def __init__(self,
                  conceptCount: int = 25,
-                 conceptCountPerType: int = None,
+                 conceptCountPerType: Union[int, None] = None,
                  conceptScoring: str = "importance",
-                 articlesSampleSize: str = 10000,
+                 articlesSampleSize: int = 10000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of concepts of resulting articles
         @param conceptCount: number of top concepts to return (at most 500)
         @param conceptCountPerType: if you wish to limit the number of top concepts per type (person, org, loc, wiki) then set this to some number.
             If you want to get equal number of concepts for each type then set conceptCountPerType to conceptCount/4 (since there are 4 concept types)
         @param conceptScoring: how should the top concepts be computed. Possible values are
             "importance" (takes into account how frequently a concept is mentioned and how relevant it is in an article),
             "frequency" (ranks the concepts simply by how frequently the concept is mentioned in the results) and
             "uniqueness" (computes what are the top concepts that are frequently mentioned in the results of your search query but less frequently mentioned in the news in general)
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 20000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert conceptCount <= 500
         assert articlesSampleSize <= 20000
         self.resultType = "conceptAggr"
         self.conceptAggrConceptCount = conceptCount
         self.conceptAggrSampleSize = articlesSampleSize
         self.conceptAggrScoring = conceptScoring
         if conceptCountPerType != None:
@@ -505,14 +519,15 @@
                  articlesSampleSize: int = 20000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of categories of resulting articles
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the categories should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert articlesSampleSize <= 50000
         self.resultType = "categoryAggr"
         self.categoryAggrSampleSize = articlesSampleSize
         self.__dict__.update(returnInfo.getParams("categoryAggr"))
 
 
 
@@ -526,27 +541,29 @@
         @param sourceCount: the number of top sources to return
         @param normalizeBySourceArts: some sources generate significantly more content than others which is why
             they can appear as top souce for a given query. If you want to normalize and sort the sources by the total number of
             articles that they have published set this to True. This will return as top sources those that potentially publish less
             content overall, but their published content is more about the searched query.
         @param returnInfo: what details about the sources should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         self.resultType = "sourceAggr"
         self.sourceAggrSourceCount = sourceCount
         self.sourceAggrNormalizeBySourceArts = normalizeBySourceArts
         self.__dict__.update(returnInfo.getParams("sourceAggr"))
 
 
 class RequestArticlesKeywordAggr(RequestArticles):
     def __init__(self,
                  articlesSampleSize: int = 2000):
         """
         get top keywords in the resulting articles
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 20000)
         """
+        super(RequestArticles, self).__init__()
         assert articlesSampleSize <= 20000
         self.resultType = "keywordAggr"
         self.keywordAggrSampleSize = articlesSampleSize
 
 
 
 class RequestArticlesConceptGraph(RequestArticles):
@@ -559,14 +576,15 @@
         """
         get concept graph of resulting articles. Identify concepts that frequently co-occur with other concepts
         @param conceptCount: how many concepts should be returned (at most 1000)
         @param linkCount: how many top links between the concepts should be returned (at most 2000)
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert conceptCount <= 1000
         assert linkCount <= 2000
         assert articlesSampleSize <= 50000
         self.resultType = "conceptGraph"
         self.conceptGraphConceptCount = conceptCount
         self.conceptGraphLinkCount = linkCount
         self.conceptGraphSampleSize = articlesSampleSize
@@ -584,99 +602,103 @@
         """
         get aggreate of concept co-occurences of resulting articles
         @param conceptCount: how many concepts should be returned (at most 200)
         @param measure: how should the interestingness between the selected pairs of concepts be computed. Options: pmi (pointwise mutual information), pairTfIdf (pair frequence * IDF of individual concepts), chiSquare
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert conceptCount <= 200
         assert articlesSampleSize <= 50000
         self.resultType = "conceptMatrix"
         self.conceptMatrixConceptCount = conceptCount
         self.conceptMatrixMeasure = measure
         self.conceptMatrixSampleSize = articlesSampleSize
         self.__dict__.update(returnInfo.getParams("conceptMatrix"))
 
 
 
 class RequestArticlesConceptTrends(RequestArticles):
     def __init__(self,
-                 conceptUris: Union[str, List[str]] = None,
+                 conceptUris: Union[str, List[str], None] = None,
                  conceptCount: int = 25,
                  articlesSampleSize: int = 10000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get trending of concepts in the resulting articles
         @param conceptUris: list of concept URIs for which to return trending information. If None, then top concepts will be automatically computed
         @param conceptCount: if the concepts are not provided, what should be the number of automatically determined concepts to return (at most 50)
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert conceptCount <= 50
         assert articlesSampleSize <= 50000
         self.resultType = "conceptTrends"
-        if conceptUris != None:
+        if conceptUris is not None:
             self.conceptTrendsConceptUri = conceptUris
         self.conceptTrendsConceptCount = conceptCount
         self.conceptTrendsSampleSize = articlesSampleSize
         self.__dict__.update(returnInfo.getParams("conceptTrends"))
 
 
 
 class RequestArticlesDateMentionAggr(RequestArticles):
     """
     get mentioned dates in the articles
     """
     def __init__(self):
+        super(RequestArticles, self).__init__()
         self.resultType = "dateMentionAggr"
 
 
 
 class RequestArticlesRecentActivity(RequestArticles):
     def __init__(self,
                  maxArticleCount: int = 100,
-                 updatesAfterNewsUri: str = None,
-                 updatesafterBlogUri: str = None,
-                 updatesAfterPrUri: str = None,
-                 updatesAfterTm: Union[datetime.datetime, datetime.date, str] = None,
-                 updatesAfterMinsAgo: int = None,
-                 updatesUntilTm: Union[datetime.datetime, datetime.date, str] = None,
-                 updatesUntilMinsAgo: int = None,
+                 updatesAfterNewsUri: Union[str, None] = None,
+                 updatesafterBlogUri: Union[str, None] = None,
+                 updatesAfterPrUri: Union[str, None] = None,
+                 updatesAfterTm: Union[datetime.datetime, str, None] = None,
+                 updatesAfterMinsAgo: Union[int, None] = None,
+                 updatesUntilTm: Union[datetime.datetime, str, None] = None,
+                 updatesUntilMinsAgo: Union[int, None] = None,
                  mandatorySourceLocation: bool = False,
-                 returnInfo: ReturnInfo = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         get the list of articles that were recently added to the Event Registry and match the selected criteria
         @param maxArticleCount: the maximum number of articles to return in the call (the number can be even higher than 100 but in case more articles
             are returned, the call will also use more tokens)
         @param updatesAfterTm: the time after which the articles were added (returned by previous call to the same method)
         @param updatesAfterMinsAgo: how many minutes into the past should we check (set either this or updatesAfterTm property, but not both)
         @param updatesUntilTm: what is the latest time when the articles were added (in case you don't want the most recent articles)
         @param updatesUntilMinsAgo: how many minutes ago was the latest time when the articles were added
         @param mandatorySourceLocation: return only articles for which we know the source's geographic location
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestArticles, self).__init__()
         assert maxArticleCount <= 2000
-        assert updatesAfterTm == None or updatesAfterMinsAgo == None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
-        assert updatesUntilTm == None or updatesUntilMinsAgo == None, "You should specify either updatesUntilTm or updatesUntilMinsAgo parameter, but not both"
+        assert updatesAfterTm is None or updatesAfterMinsAgo is None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
+        assert updatesUntilTm is None or updatesUntilMinsAgo is None, "You should specify either updatesUntilTm or updatesUntilMinsAgo parameter, but not both"
         self.resultType = "recentActivityArticles"
         self.recentActivityArticlesMaxArticleCount  = maxArticleCount
-        if updatesAfterTm != None:
+        if updatesAfterTm is not None:
             self.recentActivityArticlesUpdatesAfterTm = QueryParamsBase.encodeDateTime(updatesAfterTm)
-        if updatesAfterMinsAgo != None:
+        if updatesAfterMinsAgo is not None:
             self.recentActivityArticlesUpdatesAfterMinsAgo = updatesAfterMinsAgo
-        if updatesUntilTm != None:
+        if updatesUntilTm is not None:
             self.recentActivityArticlesUpdatesUntilTm = QueryParamsBase.encodeDateTime(updatesUntilTm)
-        if updatesUntilMinsAgo != None:
+        if updatesUntilMinsAgo is not None:
             self.recentActivityArticlesUpdatesUntilMinsAgo = updatesUntilMinsAgo
 
         # set the stopping uris, if provided
-        if updatesAfterNewsUri != None:
+        if updatesAfterNewsUri is not None:
             self.recentActivityArticlesNewsUpdatesAfterUri = updatesAfterNewsUri
-        if updatesafterBlogUri != None:
+        if updatesafterBlogUri is not None:
             self.recentActivityArticlesBlogUpdatesAfterUri = updatesafterBlogUri
-        if updatesAfterPrUri != None:
+        if updatesAfterPrUri is not None:
             self.recentActivityArticlesPrUpdatesAfterUri = updatesAfterPrUri
 
         self.recentActivityArticlesMaxArticleCount = maxArticleCount
         self.recentActivityArticlesMandatorySourceLocation = mandatorySourceLocation
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("recentActivityArticles"))
```

### Comparing `eventregistry-9.0/eventregistry/QueryEvent.py` & `eventregistry-9.1/eventregistry/QueryEvent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.QueryArticles import QueryArticles, RequestArticlesInfo
 from eventregistry.Query import *
 from eventregistry.Logger import logger
 from eventregistry.EventRegistry import EventRegistry
-from typing import Union, List
+from typing import Union, List, Literal
 
 
 class QueryEvent(Query):
     """
     Class for obtaining available info for one or more events in the Event Registry
     """
     def __init__(self,
                  eventUriOrList: Union[str, List[str]],
-                 requestedResult: "RequestEvent" = None):
+                 requestedResult: Union["RequestEvent", None] = None):
         """
         @param eventUriOrUriList: a single event uri or a list of event uris (max 50)
         @param requestedResult: the information to return as the result of the query. By default return the details of the event
         """
         super(QueryEvent, self).__init__()
         self._setVal("action", "getEvent")
         self._setVal("eventUri", eventUriOrList)
@@ -40,28 +40,29 @@
 
 
 class QueryEventArticlesIter(QueryEvent, six.Iterator):
     """
     Class for obtaining an iterator over all articles in the event
     """
     def __init__(self, eventUri: str,
-                lang: Union[str, QueryItems] = None,
-                keywords: Union[str, QueryItems] = None,
-                conceptUri: Union[str, QueryItems] = None,
-                categoryUri: Union[str, QueryItems] = None,
-                sourceUri: Union[str, QueryItems] = None,
-                sourceLocationUri: Union[str, QueryItems] = None,
-                sourceGroupUri: Union[str, QueryItems] = None,
-                authorUri: Union[str, QueryItems] = None,
-                locationUri: Union[str, QueryItems] = None,
-                dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                lang: Union[str, QueryItems, None] = None,
+                keywords: Union[str, QueryItems, None] = None,
+                conceptUri: Union[str, QueryItems, None] = None,
+                categoryUri: Union[str, QueryItems, None] = None,
+                sourceUri: Union[str, QueryItems, None] = None,
+                sourceLocationUri: Union[str, QueryItems, None] = None,
+                sourceGroupUri: Union[str, QueryItems, None] = None,
+                authorUri: Union[str, QueryItems, None] = None,
+                locationUri: Union[str, QueryItems, None] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str, None] = None,
                 keywordsLoc: str = "body",
+                keywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
 
                 startSourceRankPercentile: int = 0,
                 endSourceRankPercentile: int = 100,
                 minSentiment: float = -1,
                 maxSentiment: float = 1):
         """
         @param eventUri: a single event for which we want to obtain the list of articles in it
@@ -95,14 +96,15 @@
             Location uri can either be a city or a country. Location uri for a given name can be obtained using EventRegistry.getLocationUri().
         @param dateStart: find articles that were written on or after dateStart. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
         @param dateEnd: find articles that occurred before or on dateEnd. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
 
         @param dateMentionStart: limit the event articles to those that explicitly mention a date that is equal or greater than dateMentionStart.
         @param dateMentionEnd: limit the event articles to those that explicitly mention a date that is lower or equal to dateMentionEnd.
         @param keywordsLoc: where should we look when searching using the keywords provided by "keywords" parameter. "body" (default), "title", or "body,title"
+        @param keywordSearchMode: what search mode to use when specifying keywords. Possible values are: simple, exact, phrase
 
         @param startSourceRankPercentile: starting percentile of the sources to consider in the results (default: 0). Value should be in range 0-90 and divisible by 10.
         @param endSourceRankPercentile: ending percentile of the sources to consider in the results (default: 100). Value should be in range 10-100 and divisible by 10.
         @param minSentiment: minimum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all articles that are not reported in English language)
         @param maxSentiment: maximum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all articles that are not reported in English language)
@@ -116,28 +118,29 @@
         self._setQueryArrVal(sourceGroupUri, "sourceGroupUri", "sourceGroupOper", "or")
         self._setQueryArrVal(authorUri, "authorUri", "authorOper", "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
         self._setQueryArrVal(lang, "articlesLang", None, "or")                      # a single lang or list
 
         # starting date of the published articles (e.g. 2014-05-02)
-        if dateStart != None:
+        if dateStart is not None:
             self._setDateVal("dateStart", dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
-        if dateEnd != None:
+        if dateEnd is not None:
             self._setDateVal("dateEnd", dateEnd)
 
         # first valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionStart != None:
+        if dateMentionStart is not None:
             self._setDateVal("dateMentionStart", dateMentionStart)
         # last valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionEnd != None:
+        if dateMentionEnd is not None:
             self._setDateVal("dateMentionEnd", dateMentionEnd)
 
         self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
+        self._setValIfNotDefault("keywordSearchMode", keywordSearchMode, "phrase")
 
         assert startSourceRankPercentile >= 0 and startSourceRankPercentile % 10 == 0 and startSourceRankPercentile <= 100
         assert endSourceRankPercentile >= 0 and endSourceRankPercentile % 10 == 0 and endSourceRankPercentile <= 100
         assert startSourceRankPercentile < endSourceRankPercentile
         if startSourceRankPercentile != 0:
             self._setVal("startSourceRankPercentile", startSourceRankPercentile)
         if endSourceRankPercentile != 100:
@@ -161,15 +164,15 @@
             logger.error(res["error"])
         count = res.get(self.queryParams["eventUri"], {}).get("articles", {}).get("totalResults", 0)
         return count
 
 
     def execQuery(self, eventRegistry: EventRegistry,
             sortBy: str = "cosSim", sortByAsc: bool = False,
-            returnInfo: ReturnInfo = None,
+            returnInfo: Union[ReturnInfo, None] = None,
             maxItems: int = -1):
         """
         @param eventRegistry: instance of EventRegistry class. used to obtain the necessary data
 
         @param sortBy: order in which event articles are sorted. Options: none (no specific sorting), id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -196,15 +199,15 @@
         eventUri = self.queryParams["eventUri"]
         # move to the next page to download
         self._articlePage += 1
         # if we have already obtained all pages, then exit
         if self._totalPages != None and self._articlePage > self._totalPages:
             return
         if self._er._verboseOutput:
-            logger.debug("Downloading article page %d from event %s" % (self._articlePage, eventUri))
+            logger.debug("Downloading article page %d from event %s", self._articlePage, eventUri)
 
         self.setRequestedResult(RequestEventArticles(
             page = self._articlePage,
             sortBy = self._articlesSortBy, sortByAsc = self._articlesSortByAsc,
             returnInfo = self._returnInfo,
             **self.queryParams))
         res = self._er.execQuery(self)
@@ -256,34 +259,35 @@
 
 
 class RequestEventArticles(RequestEvent, QueryParamsBase):
     def __init__(self,
                 page = 1,
                 count = 100,
 
-                lang: Union[str, QueryItems] = None,
-                keywords: Union[str, QueryItems] = None,
-                conceptUri: Union[str, QueryItems] = None,
-                categoryUri: Union[str, QueryItems] = None,
-                sourceUri: Union[str, QueryItems] = None,
-                sourceLocationUri: Union[str, QueryItems] = None,
-                sourceGroupUri: Union[str, QueryItems] = None,
-                authorUri: Union[str, QueryItems] = None,
-                locationUri: Union[str, QueryItems] = None,
-                dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                lang: Union[str, QueryItems, None] = None,
+                keywords: Union[str, QueryItems, None] = None,
+                conceptUri: Union[str, QueryItems, None] = None,
+                categoryUri: Union[str, QueryItems, None] = None,
+                sourceUri: Union[str, QueryItems, None] = None,
+                sourceLocationUri: Union[str, QueryItems, None] = None,
+                sourceGroupUri: Union[str, QueryItems, None] = None,
+                authorUri: Union[str, QueryItems, None] = None,
+                locationUri: Union[str, QueryItems, None] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str, None] = None,
                 keywordsLoc: str = "body",
+                keywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
 
                 startSourceRankPercentile: int = 0,
                 endSourceRankPercentile: int = 100,
 
                 sortBy: str = "cosSim", sortByAsc: bool = False,
-                returnInfo: ReturnInfo = None,
+                returnInfo: Union[ReturnInfo, None] = None,
                 **kwds):
         """
         return articles about the event
         @param page: page of the articles to return (1, 2, ...)
         @param count: number of articles to return per page (at most 100)
 
         @param keywords: limit the event articles to those that mention the specified keywords.
@@ -316,14 +320,15 @@
             If more than one language is specified, resulting articles has to be written in *any* of the languages.
         @param dateStart: find articles that were written on or after dateStart. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
         @param dateEnd: find articles that occurred before or on dateEnd. Date should be provided in YYYY-MM-DD format, datetime.time or datetime.datetime.
 
         @param dateMentionStart: limit the event articles to those that explicitly mention a date that is equal or greater than dateMentionStart.
         @param dateMentionEnd: limit the event articles to those that explicitly mention a date that is lower or equal to dateMentionEnd.
         @param keywordsLoc: where should we look when searching using the keywords provided by "keywords" parameter. "body" (default), "title", or "body,title"
+        @param keywordSearchMode: what search mode to use when specifying keywords. Possible values are: simple, exact, phrase
 
         @param startSourceRankPercentile: starting percentile of the sources to consider in the results (default: 0). Value should be in range 0-100 and divisible by 10.
         @param endSourceRankPercentile: ending percentile of the sources to consider in the results (default: 100). Value should be in range 0-100 and divisible by 10.
 
         @param sortBy: order in which event articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         @param returnInfo: what details should be included in the returned information. Use None to get the default information.
@@ -344,28 +349,29 @@
         self._setQueryArrVal(sourceGroupUri, "sourceGroupUri", "sourceGroupOper", "or")
         self._setQueryArrVal(authorUri, "authorUri", "authorOper", "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
         self._setQueryArrVal(lang, "lang", None, "or")                      # a single lang or list (possible: eng, deu, spa, zho, slv)
 
         # starting date of the published articles (e.g. 2014-05-02)
-        if dateStart != None:
+        if dateStart is not None:
             self._setDateVal("dateStart", dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
-        if dateEnd != None:
+        if dateEnd is not None:
             self._setDateVal("dateEnd", dateEnd)
 
         # first valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionStart != None:
+        if dateMentionStart is not None:
             self._setDateVal("dateMentionStart", dateMentionStart)
         # last valid mentioned date detected in articles (e.g. 2014-05-02)
-        if dateMentionEnd != None:
+        if dateMentionEnd is not None:
             self._setDateVal("dateMentionEnd", dateMentionEnd)
 
         self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
+        self._setValIfNotDefault("keywordSearchMode", keywordSearchMode, "phrase")
 
         assert startSourceRankPercentile >= 0 and startSourceRankPercentile % 10 == 0 and startSourceRankPercentile <= 100
         assert endSourceRankPercentile >= 0 and endSourceRankPercentile % 10 == 0 and endSourceRankPercentile <= 100
         assert startSourceRankPercentile < endSourceRankPercentile
         if startSourceRankPercentile != 0:
             self._setVal("startSourceRankPercentile", startSourceRankPercentile)
         if endSourceRankPercentile != 100:
@@ -379,15 +385,15 @@
             self.__dict__.update(returnInfo.getParams("articles"))
         del self.queryParams
 
 
 
 class RequestEventArticleUriWgts(RequestEvent):
     def __init__(self,
-                 lang: Union[str, List[str]] = None,
+                 lang: Union[str, List[str], None] = None,
                  sortBy: str = "cosSim", sortByAsc: bool = False,
                  **kwds):
         """
         return just a list of article uris and their associated weights
         @param lang: a single language or a list of languages in which to return the articles. Set None to return all articles
         @param sortBy: order in which event articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
@@ -399,15 +405,15 @@
         self.uriWgtListSortByAsc = sortByAsc
         self.resultType = "uriWgtList"
         self.__dict__.update(**kwds)
 
 
 
 class RequestEventKeywordAggr(RequestEvent):
-    def __init__(self, lang: Union[str, List[str]] = None,
+    def __init__(self, lang: Union[str, List[str], None] = None,
                 **kwds):
         """
         return keyword aggregate (tag-cloud) from articles in the event
         @param lang: if not `None` then the top keywords will only be computed from the articles in the specified language.
             The value should match one of the languages for which we have articles in the event.
         @param kwds: any other potential query parameters - can be any of the parameters used in RequestEventArticles() constructor
         """
@@ -433,15 +439,15 @@
         """
         self.resultType = "dateMentionAggr"
 
 
 
 class RequestEventArticleTrend(RequestEvent):
     def __init__(self,
-                 lang: str = None,
+                 lang: Union[str, None] = None,
                  page: int = 1, count: int = 100,
                  minArticleCosSim: int = -1,
                  returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
         """
         return trending information for the articles about the event
         @param lang: languages for which to compute the trends. If None, then compute trends for all articles
         @param page: page of the articles for which to return information (1, 2, ...)
@@ -460,16 +466,16 @@
 
 
 
 class RequestEventSimilarEvents(RequestEvent):
     def __init__(self,
                 conceptInfoList: List[dict],
                 count: int = 50,                    # number of similar events to return
-                dateStart: Union[datetime.datetime, datetime.date, str] = None,              # what can be the oldest date of the similar events
-                dateEnd: Union[datetime.datetime, datetime.date, str] = None,                # what can be the newest date of the similar events
+                dateStart: Union[datetime.datetime, datetime.date, str, None] = None,              # what can be the oldest date of the similar events
+                dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,                # what can be the newest date of the similar events
                 addArticleTrendInfo: bool = False,   # add info how the articles in the similar events are distributed over time
                 aggrHours: int = 6,                 # if similarEventsAddArticleTrendInfo == True then this is the aggregating window
                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         compute and return a list of similar events
         @param conceptInfoList: array of concepts and their importance, e.g. [{ "uri": "http://en.wikipedia.org/wiki/Barack_Obama", "wgt": 100 }, ...]
         @param count: number of similar events to return (at most 50)
@@ -480,16 +486,16 @@
         @param returnInfo: what details should be included in the returned information
         """
         assert count <= 50
         assert isinstance(conceptInfoList, list)
         self.action = "getSimilarEvents"
         self.concepts = json.dumps(conceptInfoList)
         self.eventsCount = count
-        if dateStart != None:
+        if dateStart is not None:
             self.dateStart = QueryParamsBase.encodeDate(dateStart)
-        if dateEnd != None:
+        if dateEnd is not None:
             self.dateEnd = QueryParamsBase.encodeDate(dateEnd)
         self.similarEventsAddArticleTrendInfo = addArticleTrendInfo
         self.similarEventsAggrHours = aggrHours
         # setting resultType since we have to, but it's actually ignored on the backend
         self.resultType = "similarEvents"
         self.__dict__.update(returnInfo.getParams(""))
```

### Comparing `eventregistry-9.0/eventregistry/QueryEvents.py` & `eventregistry-9.1/eventregistry/QueryEvents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Query import *
 from eventregistry.Logger import logger
 from eventregistry.EventRegistry import EventRegistry
-from typing import Union, List
+from typing import Union, List, Literal
 
 class QueryEvents(Query):
     def __init__(self,
-                 keywords: Union[str, QueryItems] = None,
-                 conceptUri: Union[str, QueryItems] = None,
-                 categoryUri: Union[str, QueryItems] = None,
-                 sourceUri: Union[str, QueryItems] = None,
-                 sourceLocationUri: Union[str, QueryItems] = None,
-                 sourceGroupUri: Union[str, QueryItems] = None,
-                 authorUri: Union[str, QueryItems] = None,
-                 locationUri: Union[str, QueryItems] = None,
-                 lang: Union[str, QueryItems] = None,
-                 dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                 dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-                 reportingDateStart: Union[datetime.datetime, datetime.date, str] = None,
-                 reportingDateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                 keywords: Union[str, QueryItems, None] = None,
+                 conceptUri: Union[str, QueryItems, None] = None,
+                 categoryUri: Union[str, QueryItems, None] = None,
+                 sourceUri: Union[str, QueryItems, None] = None,
+                 sourceLocationUri: Union[str, QueryItems, None] = None,
+                 sourceGroupUri: Union[str, QueryItems, None] = None,
+                 authorUri: Union[str, QueryItems, None] = None,
+                 locationUri: Union[str, QueryItems, None] = None,
+                 lang: Union[str, QueryItems, None] = None,
+                 dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                 dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+                 reportingDateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                 reportingDateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
                  minSentiment: float = -1,
                  maxSentiment: float = 1,
-                 minArticlesInEvent: int = None,
-                 maxArticlesInEvent: int = None,
-                 dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
-                 dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
-                 ignoreKeywords: Union[str, QueryItems] = None,
-                 ignoreConceptUri: Union[str, QueryItems] = None,
-                 ignoreCategoryUri: Union[str, QueryItems] = None,
-                 ignoreSourceUri: Union[str, QueryItems] = None,
-                 ignoreSourceLocationUri: Union[str, QueryItems] = None,
-                 ignoreSourceGroupUri: Union[str, QueryItems] = None,
-                 ignoreAuthorUri: Union[str, QueryItems] = None,
-                 ignoreLocationUri: Union[str, QueryItems] = None,
-                 ignoreLang: Union[str, QueryItems] = None,
+                 minArticlesInEvent: Union[int, None] = None,
+                 maxArticlesInEvent: Union[int, None] = None,
+                 dateMentionStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                 dateMentionEnd: Union[datetime.datetime, datetime.date, str, None] = None,
                  keywordsLoc: str = "body",
+                 keywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
+
+                 ignoreKeywords: Union[str, QueryItems, None] = None,
+                 ignoreConceptUri: Union[str, QueryItems, None] = None,
+                 ignoreCategoryUri: Union[str, QueryItems, None] = None,
+                 ignoreSourceUri: Union[str, QueryItems, None] = None,
+                 ignoreSourceLocationUri: Union[str, QueryItems, None] = None,
+                 ignoreSourceGroupUri: Union[str, QueryItems, None] = None,
+                 ignoreAuthorUri: Union[str, QueryItems, None] = None,
+                 ignoreLocationUri: Union[str, QueryItems, None] = None,
+                 ignoreLang: Union[str, QueryItems, None] = None,
                  ignoreKeywordsLoc: str = "body",
-                 requestedResult: "RequestEvents" = None):
+                 ignoreKeywordSearchMode: Literal["simple", "exact", "phrase"] = "phrase",
+
+                 requestedResult: Union["RequestEvents", None] = None):
         """
         Query class for searching for events in the Event Registry.
         The resulting events have to match all specified conditions. If a parameter value equals "" or [], then it is ignored.
         In order for query to be valid, it has to have at least one positive condition (condition that does not start with ignore*).
 
         @param keywords: find events where articles mention all the specified keywords.
             A single keyword/phrase can be provided as a string, multiple keywords/phrases can be provided as a list of strings.
@@ -80,25 +84,29 @@
                 a computed value for the sentiment (all events that are not reported in English language)
         @param maxSentiment: maximum value of the sentiment, that the returned events should have. Range [-1, 1]. Note: setting the value will remove all events that don't have
                 a computed value for the sentiment (all events that are not reported in English language)
         @param minArticlesInEvent: find events that have been reported in at least minArticlesInEvent articles (regardless of language)
         @param maxArticlesInEvent: find events that have not been reported in more than maxArticlesInEvent articles (regardless of language)
         @param dateMentionStart: find events where articles explicitly mention a date that is equal or greater than dateMentionStart.
         @param dateMentionEnd: find events where articles explicitly mention a date that is lower or equal to dateMentionEnd.
+        @param keywordsLoc: what data should be used when searching using the keywords provided by "keywords" parameter. "body" (default), "title", or "body,title"
+        @param keywordSearchMode: what search mode to use when specifying keywords. Possible values are: simple, exact, phrase
+
         @param ignoreKeywords: ignore events where articles about the event mention any of the provided keywords
         @param ignoreConceptUri: ignore events that are about any of the provided concepts
         @param ignoreCategoryUri: ignore events that are about any of the provided categories
         @param ignoreSourceUri: ignore events that have have articles which have been written by any of the specified news sources
         @param ignoreSourceLocationUri: ignore events that have articles which been written by sources located at *any* of the specified locations
         @param ignoreSourceGroupUri: ignore events that have articles which have been written by sources in *any* of the specified source groups
         @param ignoreAuthorUri: ignore articles that were written by *any* of the specified authors
         @param ignoreLocationUri: ignore events that occurred in any of the provided locations. A location can be a city or a place
         @param ignoreLang: ignore events that are reported in any of the provided languages
-        @param keywordsLoc: what data should be used when searching using the keywords provided by "keywords" parameter. "body" (default), "title", or "body,title"
         @param ignoreKeywordsLoc: what data should be used when searching using the keywords provided by "ignoreKeywords" parameter. "body" (default), "title", or "body,title"
+        @param ignoreKeywordSearchMode: what search mode to use when specifying ignoreKeywords. Possible values are: simple, exact, phrase
+
         @param requestedResult: the information to return as the result of the query. By default return the list of matching events
         """
         super(QueryEvents, self).__init__()
 
         self._setVal("action", "getEvents")
 
         self._setQueryArrVal(keywords, "keyword", "keywordOper", "and")
@@ -108,52 +116,55 @@
         self._setQueryArrVal(sourceLocationUri, "sourceLocationUri", None, "or")
         self._setQueryArrVal(sourceGroupUri, "sourceGroupUri", "sourceGroupOper", "or")
         self._setQueryArrVal(authorUri, "authorUri", "authorOper", "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
         self._setQueryArrVal(lang, "lang", None, "or")                      # a single lang or list (possible: eng, deu, spa, zho, slv)
 
-        if (dateStart != None):
+        if dateStart is not None:
             self._setDateVal("dateStart", dateStart)        # e.g. 2014-05-02
-        if (dateEnd != None):
+        if dateEnd is not None:
             self._setDateVal("dateEnd", dateEnd)            # e.g. 2014-05-02
-        if (reportingDateStart != None):
+        if reportingDateStart is not None:
             self._setDateVal("reportingDateStart", reportingDateStart)        # e.g. 2014-05-02
-        if (reportingDateEnd != None):
+        if reportingDateEnd is not None:
             self._setDateVal("reportingDateEnd", reportingDateEnd)            # e.g. 2014-05-02
         if minSentiment != -1:
             assert minSentiment >= -1 and minSentiment <= 1
             self._setVal("minSentiment", minSentiment)      # e.g. -0.5
         if maxSentiment != 1:
             assert maxSentiment >= -1 and maxSentiment <= 1
             self._setVal("maxSentiment", maxSentiment)      # e.g. 0.5
 
         self._setValIfNotDefault("minArticlesInEvent", minArticlesInEvent, None)
         self._setValIfNotDefault("maxArticlesInEvent", maxArticlesInEvent, None)
 
-        if (dateMentionStart != None):
+        if dateMentionStart is not None:
             self._setDateVal("dateMentionStart", dateMentionStart)      # e.g. 2014-05-02
-        if (dateMentionEnd != None):
+        if dateMentionEnd is not None:
             self._setDateVal("dateMentionEnd", dateMentionEnd)          # e.g. 2014-05-02
 
+        self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
+        self._setValIfNotDefault("keywordSearchMode", keywordSearchMode, "phrase")
+
 
         # for the negative conditions, only the OR is a valid operator type
         self._setQueryArrVal(ignoreKeywords, "ignoreKeywords", None, "or")
         self._setQueryArrVal(ignoreConceptUri, "ignoreConceptUri", None, "or")
         self._setQueryArrVal(ignoreCategoryUri, "ignoreCategoryUri", None, "or")
         self._setQueryArrVal(ignoreSourceUri, "ignoreSourceUri", None, "or")
         self._setQueryArrVal(ignoreSourceLocationUri, "ignoreSourceLocationUri", None, "or")
         self._setQueryArrVal(ignoreSourceGroupUri, "ignoreSourceGroupUri", None, "or")
         self._setQueryArrVal(ignoreAuthorUri, "ignoreAuthorUri", None, "or")
         self._setQueryArrVal(ignoreLocationUri, "ignoreLocationUri", None, "or")
 
         self._setQueryArrVal(ignoreLang, "ignoreLang", None, "or")
 
-        self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
         self._setValIfNotDefault("ignoreKeywordLoc", ignoreKeywordsLoc, "body")
+        self._setValIfNotDefault("ignoreKeywordSearchMode", ignoreKeywordSearchMode, "phrase")
 
         self.setRequestedResult(requestedResult or RequestEventsInfo())
 
 
     def _getPath(self):
         return "/api/v1/event"
 
@@ -236,15 +247,15 @@
         count = res.get("events", {}).get("totalResults", 0)
         return count
 
 
     def execQuery(self, eventRegistry: EventRegistry,
                   sortBy: str = "rel",
                   sortByAsc: bool = False,
-                  returnInfo: ReturnInfo = None,
+                  returnInfo: Union[ReturnInfo, None] = None,
                   maxItems: int = -1,
                   **kwargs):
         """
         @param eventRegistry: instance of EventRegistry class. used to query new event list and uris
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
@@ -284,25 +295,25 @@
         return q
 
 
     def _getNextEventBatch(self):
         """download next batch of events based on the event uris in the uri list"""
         self._eventPage += 1
         # if we have already obtained all pages, then exit
-        if self._totalPages != None and self._eventPage > self._totalPages:
+        if self._totalPages is not None and self._eventPage > self._totalPages:
             return
         self.setRequestedResult(RequestEventsInfo(page=self._eventPage, count=self._eventBatchSize,
             sortBy= self._sortBy, sortByAsc=self._sortByAsc,
             returnInfo = self._returnInfo))
         # download articles and make sure that we set the same archive flag as it was returned when we were processing the uriList request
         if self._er._verboseOutput:
-            logger.debug("Downloading event page %d..." % (self._eventPage))
+            logger.debug("Downloading event page %d...", self._eventPage)
         res = self._er.execQuery(self)
         if "error" in res:
-            logger.error("Error while obtaining a list of events: " + res["error"])
+            logger.error("Error while obtaining a list of events: %s", res["error"])
         else:
             self._totalPages = res.get("events", {}).get("pages", 0)
         results = res.get("events", {}).get("results", [])
         self._eventList.extend(results)
 
 
     def __iter__(self):
@@ -333,32 +344,33 @@
 
 
 
 class RequestEventsInfo(RequestEvents):
     def __init__(self, page: int = 1,
                  count: int = 50,
                  sortBy: str = "rel", sortByAsc: bool = False,
-                 returnInfo: ReturnInfo = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         return event details for resulting events
         @param page: page of the results to return (1, 2, ...)
         @param count: number of events to return per page (at most 50)
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 50, "at most 50 events can be returned per call"
         self.resultType = "events"
         self.eventsPage = page
         self.eventsCount = count
         self.eventsSortBy = sortBy
         self.eventsSortByAsc = sortByAsc
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("events"))
 
 
     def setPage(self, page: int):
         assert page >= 1, "page has to be >= 1"
         self.eventsPage = page
 
@@ -377,58 +389,63 @@
         return a simple list of event uris together with the scores for resulting events
         @param page: page of the results (1, 2, ...)
         @param count: number of results to include per page (at most 100000)
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the events be sorted in ascending order (True) or descending (False)
         """
+        super(RequestEvents, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 100000
         self.resultType = "uriWgtList"
         self.uriWgtListPage = page
         self.uriWgtListCount = count
         self.uriWgtListSortBy = sortBy
         self.uriWgtListSortByAsc = sortByAsc
 
+
     def setPage(self, page):
         assert page >= 1, "page has to be >= 1"
         self.uriWgtListPage = page
 
 
 
 class RequestEventsTimeAggr(RequestEvents):
     def __init__(self):
         """
         return time distribution of resulting events
         """
+        super(RequestEvents, self).__init__()
         self.resultType = "timeAggr"
 
 
 
 class RequestEventsKeywordAggr(RequestEvents):
-    def __init__(self, lang: str = None):
+    def __init__(self, lang: Union[str, None] = None):
         """
         return keyword aggregate (tag cloud) on words in articles in resulting events
         @param lang: in which language to produce the list of top keywords. If None, then compute on all articles
         """
+        super(RequestEvents, self).__init__()
         self.resultType = "keywordAggr"
-        if lang != None:
+        if lang is not None:
             self.keywordAggrLang = lang
 
 
 
 class RequestEventsLocAggr(RequestEvents):
     def __init__(self,
                  eventsSampleSize: int = 100000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of locations of resulting events
         @param eventsSampleSize: sample of events to use to compute the location aggregate (at most 100000)
         @param returnInfo: what details (about locations) should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert eventsSampleSize <= 100000
         self.resultType = "locAggr"
         self.locAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("locAggr"))
 
 
 
@@ -438,14 +455,15 @@
                  eventsSampleSize: int = 100000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of locations and times of resulting events
         @param eventsSampleSize: sample of events to use to compute the location aggregate (at most 100000)
         @param returnInfo: what details (about locations) should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert eventsSampleSize <= 100000
         self.resultType = "locTimeAggr"
         self.locTimeAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("locTimeAggr"))
 
 
 
@@ -456,14 +474,15 @@
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         compute which concept are the most frequently occuring in the list of resulting events
         @param conceptCount: number of top concepts to return (at most 200)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 1000000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert conceptCount <= 200
         assert eventsSampleSize <= 1000000
         self.resultType = "conceptAggr"
         self.conceptAggrConceptCount = conceptCount
         self.conceptAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("conceptAggr"))
 
@@ -478,14 +497,15 @@
         """
         compute which concept pairs frequently co-occur together in the resulting events
         @param conceptCount: number of top concepts to return (at most 1,000)
         @param linkCount: number of links between the concepts to return (at most 2,000)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 100000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert conceptCount <= 1000
         assert linkCount <= 2000
         assert eventsSampleSize <= 300000
         self.resultType = "conceptGraph"
         self.conceptGraphConceptCount = conceptCount
         self.conceptGraphLinkCount = linkCount
         self.conceptGraphSampleSize = eventsSampleSize
@@ -504,38 +524,40 @@
         return how frequently they co-occur in the resulting events and
         how "surprising" this is, based on the frequency of individual concepts
         @param conceptCount: number of top concepts to return (at most 200)
         @param measure: how should the interestingness between the selected pairs of concepts be computed. Options: pmi (pointwise mutual information), pairTfIdf (pair frequence * IDF of individual concepts), chiSquare
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert conceptCount <= 200
         assert eventsSampleSize <= 300000
         self.resultType = "conceptMatrix"
         self.conceptMatrixConceptCount = conceptCount
         self.conceptMatrixMeasure = measure
         self.conceptMatrixSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("conceptMatrix"))
 
 
 
 class RequestEventsConceptTrends(RequestEvents):
     def __init__(self,
-                 conceptUris: Union[str, List[str]] = None,
+                 conceptUris: Union[str, List[str], None] = None,
                  conceptCount: int = 10,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return a list of top trending concepts and their daily trending info over time
         @param conceptUris: list of concept URIs for which to return trending information. If None, then top concepts will be automatically computed
         @param count: if the concepts are not provided, what should be the number of automatically determined concepts to return (at most 50)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert conceptCount <= 50
         self.resultType = "conceptTrends"
-        if conceptUris != None:
+        if conceptUris is not None:
             self.conceptTrendsConceptUri = conceptUris
         self.conceptTrendsConceptCount = conceptCount
         self.__dict__.update(returnInfo.getParams("conceptTrends"))
 
 
 
 class RequestEventsSourceAggr(RequestEvents):
@@ -545,14 +567,15 @@
                  returnInfo : ReturnInfo = ReturnInfo()):
         """
         return top news sources that report about the events that match the search conditions
         @param sourceCount: number of top sources to return (at most 200)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
         @param returnInfo: what details about the sources should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert sourceCount <= 200
         assert eventsSampleSize <= 100000
         self.resultType = "sourceAggr"
         self.sourceAggrSourceCount = sourceCount
         self.sourceAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("sourceAggr"))
 
@@ -565,14 +588,15 @@
                  eventsSampleSize: int = 100000):
         """
         return events and the dates that are mentioned in articles about these events
         @param minDaysApart: ignore events that don't have a date that is more than this number of days apart from the tested event
         @param minDateMentionCount: report only dates that are mentioned at least this number of times
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
         """
+        super(RequestEvents, self).__init__()
         assert eventsSampleSize <= 300000
         self.resultType = "dateMentionAggr"
         self.dateMentionAggrMinDaysApart = minDaysApart
         self.dateMentionAggrMinDateMentionCount = minDateMentionCount
         self.dateMentionAggrSampleSize = eventsSampleSize
 
 
@@ -584,14 +608,15 @@
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return hierarchical clustering of events into smaller clusters. 2-means clustering is applied on each node in the tree
         @param keywordCount: number of keywords to report in each of the clusters (at most 100)
         @param maxEventsToCluster: try to cluster at most this number of events (at most 10000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert keywordCount <= 100
         assert maxEventsToCluster <= 10000
         self.resultType = "eventClusters"
         self.eventClustersKeywordCount = keywordCount
         self.eventClustersMaxEventsToCluster = maxEventsToCluster
         self.__dict__.update(returnInfo.getParams("eventClusters"))
 
@@ -600,66 +625,69 @@
 class RequestEventsCategoryAggr(RequestEvents):
     def __init__(self,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return distribution of events into dmoz categories
         @param returnInfo: what details about the categories should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         self.resultType = "categoryAggr"
         self.__dict__.update(returnInfo.getParams("categoryAggr"))
 
 
 
 class RequestEventsRecentActivity(RequestEvents):
     def __init__(self,
                  maxEventCount: int = 50,
-                 updatesAfterTm: Union[datetime.datetime, datetime.date, str] = None,
-                 updatesAfterMinsAgo: int = None,
-                 mandatoryLocation: bool = True,
+                 updatesAfterTm: Union[datetime.datetime, str, None] = None,
+                 updatesAfterMinsAgo: Union[int, None] = None,
+                 mandatoryLocation: Union[bool, None] = True,
                  minAvgCosSim: float = 0,
-                 returnInfo: ReturnInfo = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         return a list of recently changed events that match search conditions
         @param maxEventCount: max events to return (at most 200)
         @param updatesAfterTm: the time after which the events were added/updated (returned by previous call to the same method)
         @param updatesAfterMinsAgo: how many minutes into the past should we check (set either this or updatesAfterTm property, but not both)
         @param mandatoryLocation: return only events that have a geographic location assigned to them
         @param minAvgCosSim: the minimum avg cos sim of the events to be returned (events with lower quality should not be included)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert maxEventCount <= 2000
-        assert updatesAfterTm == None or updatesAfterMinsAgo == None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
+        assert updatesAfterTm is None or updatesAfterMinsAgo is None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
         self.resultType = "recentActivityEvents"
         self.recentActivityEventsMaxEventCount = maxEventCount
         self.recentActivityEventsMandatoryLocation = mandatoryLocation
-        if updatesAfterTm != None:
+        if updatesAfterTm is not None:
             self.recentActivityEventsUpdatesAfterTm = QueryParamsBase.encodeDateTime(updatesAfterTm)
-        if updatesAfterMinsAgo != None:
+        if updatesAfterMinsAgo is not None:
             self.recentActivityEventsUpdatesAfterMinsAgo = updatesAfterMinsAgo
         self.recentActivityEventsMinAvgCosSim = minAvgCosSim
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("recentActivityEvents"))
 
 
 class RequestEventsBreakingEvents(RequestEvents):
     def __init__(self,
                  page: int = 1,
                  count: int = 50,
                  minBreakingScore: float = 0.2,
-                 returnInfo: ReturnInfo = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         return a list of events that are currently breaking
         @param page: max events to return (at most 50)
         @param count: max events to return (at most 50)
         @param minBreakingScore: the minimum score of "breakingness" of the events to be returned
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestEvents, self).__init__()
         assert page >= 1
         assert count <= 50
         self.resultType = "breakingEvents"
         self.breakingEventsPage = page
         self.breakingEventsCount = count
         self.breakingEventsMinBreakingScore = minBreakingScore
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("breakingEvents"))
```

### Comparing `eventregistry-9.0/eventregistry/QueryMentions.py` & `eventregistry-9.1/eventregistry/QueryMentions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 from eventregistry.Logger import logger
 from eventregistry.EventRegistry import EventRegistry
 from typing import Union, List
 
 
 class QueryMentions(Query):
     def __init__(self,
-                eventTypeUri: Union[str, QueryItems] = None,
-                keywords: Union[str, QueryItems] = None,
-                conceptUri: Union[str, QueryItems] = None,
-                categoryUri: Union[str, QueryItems] = None,
-                sourceUri: Union[str, QueryItems] = None,
-                sourceLocationUri: Union[str, QueryItems] = None,
-                sourceGroupUri: Union[str, QueryItems] = None,
-                industryUri: Union[str, QueryItems] = None,
-                sdgUri: Union[str, QueryItems] = None,
-                sasbUri: Union[str, QueryItems] = None,
-                esgUri: Union[str, QueryItems] = None,
-                locationUri: Union[str, QueryItems] = None,
-                lang: Union[str, QueryItems] = None,
-                dateStart: Union[datetime.datetime, datetime.date, str] = None,
-                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
-
-                ignoreEventTypeUri: Union[str, QueryItems] = None,
-                ignoreKeywords: Union[str, QueryItems] = None,
-                ignoreConceptUri: Union[str, QueryItems] = None,
-                ignoreCategoryUri: Union[str, QueryItems] = None,
-                ignoreSourceUri: Union[str, QueryItems] = None,
-                ignoreSourceLocationUri: Union[str, QueryItems] = None,
-                ignoreSourceGroupUri: Union[str, QueryItems] = None,
-                ignoreIndustryUri: Union[str, QueryItems] = None,
-                ignoreSdgUri: Union[str, QueryItems] = None,
-                ignoreSasbUri: Union[str, QueryItems] = None,
-                ignoreEsgUri: Union[str, QueryItems] = None,
-                ignoreLocationUri: Union[str, QueryItems] = None,
-                ignoreLang: Union[str, QueryItems] = None,
+                eventTypeUri: Union[str, QueryItems, None] = None,
+                keywords: Union[str, QueryItems, None] = None,
+                conceptUri: Union[str, QueryItems, None] = None,
+                categoryUri: Union[str, QueryItems, None] = None,
+                sourceUri: Union[str, QueryItems, None] = None,
+                sourceLocationUri: Union[str, QueryItems, None] = None,
+                sourceGroupUri: Union[str, QueryItems, None] = None,
+                industryUri: Union[str, QueryItems, None] = None,
+                sdgUri: Union[str, QueryItems, None] = None,
+                sasbUri: Union[str, QueryItems, None] = None,
+                esgUri: Union[str, QueryItems, None] = None,
+                locationUri: Union[str, QueryItems, None] = None,
+                lang: Union[str, QueryItems, None] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str, None] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str, None] = None,
+
+                ignoreEventTypeUri: Union[str, QueryItems, None] = None,
+                ignoreKeywords: Union[str, QueryItems, None] = None,
+                ignoreConceptUri: Union[str, QueryItems, None] = None,
+                ignoreCategoryUri: Union[str, QueryItems, None] = None,
+                ignoreSourceUri: Union[str, QueryItems, None] = None,
+                ignoreSourceLocationUri: Union[str, QueryItems, None] = None,
+                ignoreSourceGroupUri: Union[str, QueryItems, None] = None,
+                ignoreIndustryUri: Union[str, QueryItems, None] = None,
+                ignoreSdgUri: Union[str, QueryItems, None] = None,
+                ignoreSasbUri: Union[str, QueryItems, None] = None,
+                ignoreEsgUri: Union[str, QueryItems, None] = None,
+                ignoreLocationUri: Union[str, QueryItems, None] = None,
+                ignoreLang: Union[str, QueryItems, None] = None,
 
                 showDuplicates: bool = False,
                 startSourceRankPercentile: int = 0,
                 endSourceRankPercentile: int = 100,
                 minSentiment: float = -1,
                 maxSentiment: float = 1,
-                minSentenceIndex: int = None,
-                maxSentenceIndex: int = None,
-                requestedResult: "RequestMentions" = None):
+                minSentenceIndex: Union[int, None] = None,
+                maxSentenceIndex: Union[int, None] = None,
+                requestedResult: Union["RequestMentions", None] = None):
         """
         Query class for searching for individual mentions in the Event Registry.
         The resulting mentions (objects, containing sentence, article information, mentioned entities, etc.) have to match all specified conditions.
         If a parameter value equals "" or [], then it is ignored.
         In order for query to be valid, it has to have at least one positive condition (condition that does not start with ignore*).
         @param eventTypeUri: find mentions that express a certain type of a relation.
             A single event type can be provided as a string, multiple event types can be provided as a list of strings.
@@ -140,18 +140,18 @@
         self._setQueryArrVal(sasbUri, "sasbUri", None, "or")
         self._setQueryArrVal(esgUri, "esgUri", None, "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
         self._setQueryArrVal(lang, "lang", None, "or")                      # a single lang or list (possible: eng, deu, spa, zho, slv)
 
         # starting date of the published articles (e.g. 2014-05-02)
-        if dateStart != None:
+        if dateStart is not None:
             self._setDateVal("dateStart", dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
-        if dateEnd != None:
+        if dateEnd is not None:
             self._setDateVal("dateEnd", dateEnd)
 
 
         # for the negative conditions, only the OR is a valid operator type
         self._setQueryArrVal(ignoreEventTypeUri, "ignoreEventTypeUri", None, "or")
         self._setQueryArrVal(ignoreKeywords, "ignoreKeyword", None, "or")
         self._setQueryArrVal(ignoreConceptUri, "ignoreConceptUri", None, "or")
@@ -177,18 +177,18 @@
             self._setVal("endSourceRankPercentile", endSourceRankPercentile)
         if minSentiment != -1:
             assert minSentiment >= -1 and minSentiment <= 1
             self._setVal("minSentiment", minSentiment)
         if maxSentiment != 1:
             assert maxSentiment >= -1 and maxSentiment <= 1
             self._setVal("maxSentiment", maxSentiment)
-        if minSentenceIndex != None:
+        if minSentenceIndex is not None:
             assert minSentenceIndex >= 0
             self._setVal("minSentenceIndex", minSentenceIndex)
-        if maxSentenceIndex != None:
+        if maxSentenceIndex is not None:
             assert maxSentenceIndex >= 0
             self._setVal("maxSentenceIndex", maxSentenceIndex)
 
         # set the information that should be returned
         self.setRequestedResult(requestedResult or RequestMentionsInfo())
 
 
@@ -266,15 +266,15 @@
         count = res.get("mentions", {}).get("totalResults", 0)
         return count
 
 
     def execQuery(self, eventRegistry: EventRegistry,
                   sortBy: str = "rel",
                   sortByAsc: bool = False,
-                  returnInfo: ReturnInfo = None,
+                  returnInfo: Union[ReturnInfo, None] = None,
                   maxItems: int = -1,
                   **kwargs):
         """
         @param eventRegistry: instance of EventRegistry class. used to query new mention list and uris
         @param sortBy: how are mentions sorted. Options: date (publishing date), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -326,24 +326,24 @@
 
 
     def _getNextMentionBatch(self):
         """download next batch of mentions based on the mention uris in the uri list"""
         # try to get more uris, if none
         self._mentionPage += 1
         # if we have already obtained all pages, then exit
-        if self._totalPages != None and self._mentionPage > self._totalPages:
+        if self._totalPages is not None and self._mentionPage > self._totalPages:
             return
         self.setRequestedResult(RequestMentionsInfo(page=self._mentionPage,
             sortBy=self._sortBy, sortByAsc=self._sortByAsc,
             returnInfo = self._returnInfo))
         if self._er._verboseOutput:
-            logger.debug("Downloading mention page %d..." % (self._mentionPage))
+            logger.debug("Downloading mention page %d...", self._mentionPage)
         res = self._er.execQuery(self)
         if "error" in res:
-            logger.error("Error while obtaining a list of mentions: " + res["error"])
+            logger.error("Error while obtaining a list of mentions: %s", res["error"])
         else:
             self._totalPages = res.get("mentions", {}).get("pages", 0)
         results = res.get("mentions", {}).get("results", [])
         self._mentionList.extend(results)
 
 
     def __iter__(self):
@@ -375,31 +375,32 @@
 
 
 class RequestMentionsInfo(RequestMentions):
     def __init__(self,
                  page: int = 1,
                  count: int = 100,
                  sortBy: str = "date", sortByAsc: bool = False,
-                 returnInfo: RequestMentions = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         return mention details for resulting mentions
         @param page: page of the mentions to return
         @param count: number of mentions to return for the given page (at most 100)
         @param sortBy: how are mentions sorted. Options: id (internal id), date (publishing date), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 200, "at most 100 mentions can be returned per call"
         self.resultType = "mentions"
         self.mentionsPage = page
         self.mentionsCount = count
         self.mentionsSortBy = sortBy
         self.mentionsSortByAsc = sortByAsc
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("mentions"))
 
 
     def setPage(self, page):
         """
         set the page of results to obtain
         """
@@ -416,14 +417,15 @@
         """
         return a list of mention uris together with the scores
         @param page: page of the results (1, 2, ...)
         @param count: number of items to return in a single query (at most 50000)
         @param sortBy: how are mentions sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False) according to the sortBy criteria
         """
+        super(RequestMentions, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 50000
         self.resultType = "uriWgtList"
         self.uriWgtListPage = page
         self.uriWgtListCount = count
         self.uriWgtListSortBy = sortBy
         self.uriWgtListSortByAsc = sortByAsc
@@ -436,22 +438,23 @@
 
 
 class RequestMentionsTimeAggr(RequestMentions):
     def __init__(self):
         """
         return time distribution of resulting mentions
         """
+        super(RequestMentions, self).__init__()
         self.resultType = "timeAggr"
 
 
 
 class RequestMentionsConceptAggr(RequestMentions):
     def __init__(self,
                  conceptCount: int = 25,
-                 conceptCountPerType: bool = None,
+                 conceptCountPerType: Union[int, None] = None,
                  conceptScoring: str = "importance",
                  mentionsSampleSize: int = 10000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of concepts of resulting mentions
         @param conceptCount: number of top concepts to return (at most 500)
         @param conceptCountPerType: if you wish to limit the number of top concepts per type (person, org, loc, wiki) then set this to some number.
@@ -459,35 +462,37 @@
         @param conceptScoring: how should the top concepts be computed. Possible values are
             "importance" (takes into account how frequently a concept is mentioned and how relevant it is in an mention),
             "frequency" (ranks the concepts simply by how frequently the concept is mentioned in the results) and
             "uniqueness" (computes what are the top concepts that are frequently mentioned in the results of your search query but less frequently mentioned in the news in general)
         @param mentionsSampleSize: on what sample of results should the aggregate be computed (at most 20000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         assert conceptCount <= 500
         assert mentionsSampleSize <= 20000
         self.resultType = "conceptAggr"
         self.conceptAggrConceptCount = conceptCount
         self.conceptAggrSampleSize = mentionsSampleSize
         self.conceptAggrScoring = conceptScoring
-        if conceptCountPerType != None:
+        if conceptCountPerType is not None:
             self.conceptAggrConceptCountPerType = conceptCountPerType
         self.__dict__.update(returnInfo.getParams("conceptAggr"))
 
 
 
 class RequestMentionsCategoryAggr(RequestMentions):
     def __init__(self,
                  mentionsSampleSize: int = 20000,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of categories of resulting mentions
         @param mentionsSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the categories should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         assert mentionsSampleSize <= 50000
         self.resultType = "categoryAggr"
         self.categoryAggrSampleSize = mentionsSampleSize
         self.__dict__.update(returnInfo.getParams("categoryAggr"))
 
 
 
@@ -496,26 +501,28 @@
                  sourceCount: int = 50,
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of news sources of resulting mentions
         @param sourceCount: the number of top sources to return
         @param returnInfo: what details about the sources should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         self.resultType = "sourceAggr"
         self.sourceAggrSourceCount = sourceCount
         self.__dict__.update(returnInfo.getParams("sourceAggr"))
 
 
 class RequestMentionsKeywordAggr(RequestMentions):
     def __init__(self,
                  mentionsSampleSize: int = 2000):
         """
         get top keywords in the resulting mentions
         @param mentionsSampleSize: on what sample of results should the aggregate be computed (at most 20000)
         """
+        super(RequestMentions, self).__init__()
         assert mentionsSampleSize <= 20000
         self.resultType = "keywordAggr"
         self.keywordAggrSampleSize = mentionsSampleSize
 
 
 
 class RequestMentionsConceptGraph(RequestMentions):
@@ -528,14 +535,15 @@
         """
         get concept graph of resulting mentions. Identify concepts that frequently co-occur with other concepts
         @param conceptCount: how many concepts should be returned (at most 1000)
         @param linkCount: how many top links between the concepts should be returned (at most 2000)
         @param mentionsSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         assert conceptCount <= 1000
         assert linkCount <= 2000
         assert mentionsSampleSize <= 50000
         self.resultType = "conceptGraph"
         self.conceptGraphConceptCount = conceptCount
         self.conceptGraphLinkCount = linkCount
         self.conceptGraphSampleSize = mentionsSampleSize
@@ -543,47 +551,48 @@
         self.__dict__.update(returnInfo.getParams("conceptGraph"))
 
 
 
 class RequestMentionsRecentActivity(RequestMentions):
     def __init__(self,
                  maxMentionCount: int = 100,
-                 updatesAfterUri: str =None,
-                 updatesAfterTm: Union[datetime.datetime, str] = None,
-                 updatesAfterMinsAgo: int = None,
-                 updatesUntilTm: Union[datetime.datetime, str] = None,
-                 updatesUntilMinsAgo: int = None,
+                 updatesAfterUri: Union[str, None] = None,
+                 updatesAfterTm: Union[datetime.datetime, str, None] = None,
+                 updatesAfterMinsAgo: Union[int, None] = None,
+                 updatesUntilTm: Union[datetime.datetime, str, None] = None,
+                 updatesUntilMinsAgo: Union[int, None] = None,
                  mandatorySourceLocation: bool = False,
-                 returnInfo: ReturnInfo = None):
+                 returnInfo: Union[ReturnInfo, None] = None):
         """
         get the list of mentions that were recently added to the Event Registry and match the selected criteria
         @param maxMentionCount: the maximum number of mentions to return in the call (the number can be even higher than 100 but in case more mentions
             are returned, the call will also use more tokens)
         @param updatesAfterTm: the time after which the mentions were added (returned by previous call to the same method)
         @param updatesAfterMinsAgo: how many minutes into the past should we check (set either this or updatesAfterTm property, but not both)
         @param updatesUntilTm: what is the latest time when the mentions were added (in case you don't want the most recent mentions)
         @param updatesUntilMinsAgo: how many minutes ago was the latest time when the mentions were added
         @param mandatorySourceLocation: return only mentions for which we know the source's geographic location
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestMentions, self).__init__()
         assert maxMentionCount <= 2000
-        assert updatesAfterTm == None or updatesAfterMinsAgo == None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
-        assert updatesUntilTm == None or updatesUntilMinsAgo == None, "You should specify either updatesUntilTm or updatesUntilMinsAgo parameter, but not both"
+        assert updatesAfterTm is None or updatesAfterMinsAgo is None, "You should specify either updatesAfterTm or updatesAfterMinsAgo parameter, but not both"
+        assert updatesUntilTm is None or updatesUntilMinsAgo is None, "You should specify either updatesUntilTm or updatesUntilMinsAgo parameter, but not both"
         self.resultType = "recentActivityMentions"
         self.recentActivityMentionsMaxMentionCount  = maxMentionCount
-        if updatesAfterTm != None:
+        if updatesAfterTm is not None:
             self.recentActivityMentionsUpdatesAfterTm = QueryParamsBase.encodeDateTime(updatesAfterTm)
-        if updatesAfterMinsAgo != None:
+        if updatesAfterMinsAgo is not None:
             self.recentActivityMentionsUpdatesAfterMinsAgo = updatesAfterMinsAgo
-        if updatesUntilTm != None:
+        if updatesUntilTm is not None:
             self.recentActivityMentionsUpdatesUntilTm = QueryParamsBase.encodeDateTime(updatesUntilTm)
-        if updatesUntilMinsAgo != None:
+        if updatesUntilMinsAgo is not None:
             self.recentActivityMentionsUpdatesUntilMinsAgo = updatesUntilMinsAgo
 
         # set the stopping uris, if provided
-        if updatesAfterUri != None:
+        if updatesAfterUri is not None:
             self.recentActivityMentionsUpdatesAfterUri = updatesAfterUri
 
         self.recentActivityMentionsMaxMentionCount = maxMentionCount
         self.recentActivityMentionsMandatorySourceLocation = mandatorySourceLocation
-        if returnInfo != None:
+        if returnInfo is not None:
             self.__dict__.update(returnInfo.getParams("recentActivityMentions"))
```

### Comparing `eventregistry-9.0/eventregistry/QueryStory.py` & `eventregistry-9.1/eventregistry/QueryStory.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     Class for obtaining available info for one or more stories (clusters) in the Event Registry
     NOTE: Story in our terminology is a cluster of articles (and not a single article). An event is
     then something that consists of one or more stories (typically in different languages).
 
     @param storyUriOrList: a single story uri or a list of story uris
     """
-    def __init__(self, storyUriOrList: Union[str, List[str]] = None):
+    def __init__(self, storyUriOrList: Union[str, List[str], None] = None):
         super(QueryStory, self).__init__()
         self._setVal("action", "getStory")
         if storyUriOrList != None:
             self.queryByUri(storyUriOrList)
 
 
     def _getPath(self):
@@ -49,14 +49,15 @@
 
 
 class RequestStoryInfo(RequestStory):
     """
     return details about a story
     """
     def __init__(self, returnInfo: ReturnInfo = ReturnInfo()):
+        super(RequestStory, self).__init__()
         self.resultType = "info"
         self.__dict__.update(returnInfo.getParams("info"))
 
 
 
 class RequestStoryArticles(RequestStory):
     """
@@ -71,14 +72,15 @@
         return articles in the story (cluster)
         @param page: page of the articles to return (1, 2, ...)
         @param count: number of articles to return per page (at most 100)
         @param sortBy: order in which articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         @param returnInfo: what details should be included in the returned information
         """
+        super(RequestStory, self).__init__()
         assert page >= 1, "page has to be >= 1"
         assert count <= 100
         self.resultType = "articles"
         self.articlesPage = page
         self.articlesCount = count
         self.articlesSortBy = sortBy
         self.articlesSortByAsc = sortByAsc
@@ -94,28 +96,30 @@
                  sortBy: str = "cosSim", sortByAsc: bool = False  # order in which story articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to story centroid), socialScore (total shares in social media), facebookShares (shares on fb), twitterShares (shares on twitter)
                  ):
         """
         return articles in the story (cluster)
         @param sortBy: order in which articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         """
+        super(RequestStory, self).__init__()
         self.articleUrisSortBy = sortBy
         self.articleUrisSortByAsc = sortByAsc
         self.resultType = "articleUris"
 
 
 
 class RequestStoryArticleTrend(RequestStory):
     """
     return trending information for the articles about the story
     """
     def __init__(self,
                  lang: Union[str, List[str]] = mainLangs,
                  minArticleCosSim: float = -1,
                  returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
+        super(RequestStory, self).__init__()
         self.resultType = "articleTrend"
         self.articleTrendLang = lang
         self.articleTrendMinArticleCosSim = minArticleCosSim
         self.__dict__.update(returnInfo.getParams("articleTrend"))
 
 
 
@@ -128,26 +132,27 @@
         @param dateEnd: what can be the newest date of the similar stories
         @param addArticleTrendInfo: for the returned stories compute how they were trending (intensity of reporting) in different time periods
         @param aggrHours: time span that is used as a unit when computing the trending info
         @param returnInfo: what details should be included in the returned information
         """
     def __init__(self,
                 conceptInfoList: Union[str, List[str]],
-                count: int = 50,                                    # number of similar stories to return
-                dateStart: Union[datetime.date, str] = None,        # what can be the oldest date of the similar stories
-                dateEnd: Union[datetime.date, str] = None,          # what can be the newest date of the similar stories
+                count: int = 50,                                          # number of similar stories to return
+                dateStart: Union[datetime.date, str, None] = None,        # what can be the oldest date of the similar stories
+                dateEnd: Union[datetime.date, str, None] = None,          # what can be the newest date of the similar stories
                 lang: Union[str, List[str]] = [],
                 returnInfo: ReturnInfo = ReturnInfo()):
+        super(RequestStory, self).__init__()
         assert count <= 50
         assert isinstance(conceptInfoList, list)
         self.action = "getSimilarStories"
         self.concepts = json.dumps(conceptInfoList)
         self.storiesCount = count
-        if dateStart != None:
+        if dateStart is not None:
             self.dateStart = QueryParamsBase.encodeDate(dateStart)
-        if dateEnd != None:
+        if dateEnd is not None:
             self.dateEnd = QueryParamsBase.encodeDate(dateEnd)
         if len(lang) > 0:
             self.lang = lang
         # setting resultType since we have to, but it's actually ignored on the backend
         self.resultType = "similarStories"
         self.__dict__.update(returnInfo.getParams("similarStories"))
```

### Comparing `eventregistry-9.0/eventregistry/Recent.py` & `eventregistry-9.1/eventregistry/Recent.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from eventregistry.ReturnInfo import *
 from eventregistry.EventRegistry import EventRegistry
 from typing import Union, List
 
 class GetRecentEvents(QueryParamsBase):
     def __init__(self,
                  eventRegistry: EventRegistry,
-                 mandatoryLang: Union[str, List[str]] = None,
+                 mandatoryLang: Union[str, List[str], None] = None,
                  mandatoryLocation: bool = True,
                  returnInfo: ReturnInfo = ReturnInfo(),
                  **kwargs):
         """
         Return info about recently added/modified events
         @param eventRegistry: instance of class EventRegistry
         @param mandatoryLang: set a lang or array of langs if you wish to only get events covered at least by the specified language
@@ -22,15 +22,15 @@
         @param returnInfo: what details should be included in the returned information
         """
         QueryParamsBase.__init__(self)
 
         self._er = eventRegistry
         self._setVal("recentActivityEventsMandatoryLocation", mandatoryLocation)
         # return only events that have at least a story in the specified language
-        if mandatoryLang != None:
+        if mandatoryLang is not None:
             self._setVal("recentActivityEventsMandatoryLang", mandatoryLang)
         self.queryParams.update(kwargs)
         self._update(returnInfo.getParams("recentActivityEvents"))
 
 
     def _getPath(self):
         return "/api/v1/minuteStreamEvents"
@@ -53,29 +53,29 @@
 
 
 
 class GetRecentArticles(QueryParamsBase):
     def __init__(self,
                  eventRegistry: EventRegistry,
                  mandatorySourceLocation: bool = False,
-                 articleLang: Union[str, List[str]] = None,
+                 articleLang: Union[str, List[str], None] = None,
                  returnInfo: ReturnInfo = ReturnInfo(),
                  **kwargs):
         """
         Return info about recently added articles
         @param eventRegistry: instance of class EventRegistry
         @param mandatorySourceLocation: if True then return only articles from sources for which we know geographic location
         @param articleLang: None, string or a list of strings, depending if we should return all articles, or articles in one or more languages
         @param returnInfo: what details should be included in the returned information
         """
         QueryParamsBase.__init__(self)
 
         self._er = eventRegistry
         self._setVal("recentActivityArticlesMandatorySourceLocation", mandatorySourceLocation)
-        if articleLang != None:
+        if articleLang is not None:
             self._setVal("recentActivityArticlesLang", articleLang)
         self.queryParams.update(kwargs)
         self._update(returnInfo.getParams("recentActivityArticles"))
 
 
     def _getPath(self):
         return "/api/v1/minuteStreamArticles"
```

### Comparing `eventregistry-9.0/eventregistry/ReturnInfo.py` & `eventregistry-9.1/eventregistry/ReturnInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
     @staticmethod
     def loadFromFile(fileName: str):
         """
         load the configuration for the ReturnInfo from a fileName
         @param fileName: filename that contains the json configuration to use in the ReturnInfo
         """
         assert os.path.exists(fileName), "File " + fileName + " does not exist"
-        conf = json.load(open(fileName))
+        conf = json.load(open(fileName, encoding="utf8"))
         return ReturnInfo(
             articleInfo=ArticleInfoFlags(**conf.get("articleInfo", {})),
             eventInfo=EventInfoFlags(**conf.get("eventInfo", {})),
             sourceInfo=SourceInfoFlags(**conf.get("sourceInfo", {})),
             categoryInfo=CategoryInfoFlags(**conf.get("categoryInfo", {})),
             conceptInfo=ConceptInfoFlags(**conf.get("conceptInfo", {})),
             locationInfo=LocationInfoFlags(**conf.get("locationInfo", {})),
```

### Comparing `eventregistry-9.0/eventregistry/TopicPage.py` & `eventregistry-9.1/eventregistry/TopicPage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     """
     def __init__(self, eventRegistry: EventRegistry):
         """
         create an instance of a topic page
 
         @param eventRegistry: instance of class EventRegistry
         """
+        super(QueryParamsBase, self).__init__()
         self.eventRegistry = eventRegistry
 
+
     def getMyTopicPages(self):
         """
         get the list of topic pages owned by me
         """
         userProfile = self.eventRegistry.jsonRequest("/api/v1/user/getUserProfile", {})
         return userProfile.get("ownedTopicPages", [])
 
@@ -34,14 +36,15 @@
 class TopicPage(QueryParamsBase):
     def __init__(self, eventRegistry: EventRegistry):
         """
         create an instance of a topic page
 
         @param eventRegistry: instance of class EventRegistry
         """
+        super(QueryParamsBase, self).__init__()
         self.eventRegistry = eventRegistry
         # topic page definition
         self.topicPage = self._createEmptyTopicPage()
         self.concept = {}
 
 
     def _createEmptyTopicPage(self):
@@ -239,55 +242,55 @@
         self.topicPage["sourceGroups"] = []
 
 
     def clearLocations(self):
         self.topicPage["locations"] = []
 
 
-    def addConcept(self, conceptUri: str, weight: float, label: str = None, conceptType: str = None, required: bool = False, excluded: bool = False):
+    def addConcept(self, conceptUri: str, weight: float, label: Union[str, None] = None, conceptType: Union[str, None] = None, required: bool = False, excluded: bool = False):
         """
         add a relevant concept to the topic page
         @param conceptUri: uri of the concept to be added
         @param weight: importance of the provided concept (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO be annotated with this concept
         @param excluded: if true, then all results annotated with this concept will be ignored
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
-        assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
+        assert not (required is True and excluded is True), "Parameters required and excluded can not be True at the same time"
         concept = {"uri": conceptUri, "wgt": weight, "required": required, "excluded": excluded }
-        if label != None:
+        if label is not None:
             concept["label"] = label
-        if conceptType != None:
+        if conceptType is not None:
             concept["type"] = conceptType
         self.topicPage["concepts"].append(concept)
 
 
     def addKeyword(self, keyword: str, weight: float, required: bool = False, excluded: bool = False):
         """
         add a relevant keyword to the topic page
         @param keyword: keyword or phrase to be added
         @param weight: importance of the provided keyword (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO mention this keyword to appear in the results
         @param excluded: if true, then no results that mention this keyword will be returned
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
-        assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
+        assert not (required is True and excluded is True), "Parameters required and excluded can not be True at the same time"
         self.topicPage["keywords"].append({"keyword": keyword, "wgt": weight, "required": required, "excluded": excluded })
 
 
     def addCategory(self, categoryUri: str, weight: float, required: bool = False, excluded: bool = False):
         """
         add a relevant category to the topic page
         @param categoryUri: uri of the category to be added
         @param weight: importance of the provided category (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO be annotated with this category to appear in the results
         @param excluded: if true, then no results with this category will be returned
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
-        assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
+        assert not (required is True and excluded is True), "Parameters required and excluded can not be True at the same time"
         self.topicPage["categories"].append({"uri": categoryUri, "wgt": weight, "required": required, "excluded": excluded })
 
 
     def addSource(self, sourceUri: str, weight: float, excluded: bool = False):
         """
         add a news source to the topic page
         @param sourceUri: uri of the news source to add to the topic page
```

### Comparing `eventregistry-9.0/eventregistry/Trends.py` & `eventregistry-9.1/eventregistry/Trends.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
         get currently top trending concepts
         @param source: source information from which to compute top trends. Options: "news", "social", "pr", "blogs"
         @param count: number of top trends to return
         @param conceptType: which types of concepts are we interested in
         @param returnInfo: what details should be included in the returned information
         """
-        QueryParamsBase.__init__(self)
+        TrendsBase.__init__(self)
         self._setVal("action", "getTrendingConcepts")
         self._setVal("source", source)
         if source != "social":
             self._setVal("dataType", source)
         self._setVal("conceptCount", count)
         self._setVal("conceptType", conceptType)
         self._update(returnInfo.getParams())
@@ -44,15 +44,15 @@
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending categories
         @param source: source information from which to compute top trends. Options: "news", "social", "pr", "blogs"
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
-        QueryParamsBase.__init__(self)
+        TrendsBase.__init__(self)
         self._setVal("action", "getTrendingCategories")
         self._setVal("source", source)
         if source != "social":
             self._setVal("dataType", source)
         self._setVal("categoryCount", count)
         self._update(returnInfo.getParams())
 
@@ -64,15 +64,15 @@
                  returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending items for which the users provided the data
         this data can be stock prices, energy prices, etc...
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
-        QueryParamsBase.__init__(self)
+        TrendsBase.__init__(self)
         self._setVal("action", "getTrendingCustom")
         self._setVal("conceptCount", count)
         self._update(returnInfo.getParams())
 
 
 
 class GetTrendingConceptGroups(TrendsBase):
@@ -83,15 +83,15 @@
         """
         get currently top trending groups of concepts
         a group can be identified by the concept type or by a concept class uri
         @param source: source information from which to compute top trends. Options: "news", "social"
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
-        QueryParamsBase.__init__(self)
+        TrendsBase.__init__(self)
         self._setVal("action", "getConceptTrendGroups")
         self._setVal("source", source)
         self._setVal("conceptCount", count)
         self._update(returnInfo.getParams())
 
 
     def getConceptTypeGroups(self, types: Union[str, List[str]] = ["person", "org", "loc"]):
```

### Comparing `eventregistry-9.0/eventregistry/__init__.py` & `eventregistry-9.1/eventregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/eventregistry.egg-info/PKG-INFO` & `eventregistry-9.1/eventregistry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventregistry
-Version: 9.0
+Version: 9.1
 Summary: A package that can be used to query information in Event Registry (http://eventregistry.org/)
 Home-page: https://github.com/EventRegistry/event-registry-python
 Author: Gregor Leban
 Author-email: gregor@eventregistry.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eventregistry-9.0/eventregistry.egg-info/SOURCES.txt` & `eventregistry-9.1/eventregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eventregistry-9.0/setup.py` & `eventregistry-9.1/setup.py`

 * *Files identical despite different names*

