# Comparing `tmp/groupdocs-rewriter-cloud-23.4.tar.gz` & `tmp/groupdocs-rewriter-cloud-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-rewriter-cloud-23.4.tar", last modified: Wed Apr 26 08:46:24 2023, max compression
+gzip compressed data, was "dist\groupdocs-rewriter-cloud-23.6.tar", last modified: Fri Jun 23 09:09:38 2023, max compression
```

## Comparing `groupdocs-rewriter-cloud-23.4.tar` & `groupdocs-rewriter-cloud-23.6.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.546115 groupdocs-rewriter-cloud-23.4/
--rw-rw-rw-   0        0        0    13635 2023-04-26 08:46:24.546115 groupdocs-rewriter-cloud-23.4/PKG-INFO
--rw-rw-rw-   0        0        0    10944 2023-04-26 08:37:48.000000 groupdocs-rewriter-cloud-23.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.347335 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/
--rw-rw-rw-   0        0        0    13635 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-26 08:46:24.000000 groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.378398 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/
--rw-rw-rw-   0        0        0     1665 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.403856 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/
--rw-rw-rw-   0        0        0     1482 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/__init__.py
--rw-rw-rw-   0        0        0    10682 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/rewriter_api.py
--rw-rw-rw-   0        0        0    56910 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/storage_api.py
--rw-rw-rw-   0        0        0    25431 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api_client.py
--rw-rw-rw-   0        0        0    10057 2022-12-30 11:43:49.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.517444 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/
--rw-rw-rw-   0        0        0     2094 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/__init__.py
--rw-rw-rw-   0        0        0     2972 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/base_model.py
--rw-rw-rw-   0        0        0     3556 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     3718 2022-12-30 11:20:06.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/document_response.py
--rw-rw-rw-   0        0        0     4586 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error.py
--rw-rw-rw-   0        0        0     3377 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error_details.py
--rw-rw-rw-   0        0        0     7202 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_version.py
--rw-rw-rw-   0        0        0     2650 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_versions.py
--rw-rw-rw-   0        0        0     2682 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_list.py
--rw-rw-rw-   0        0        0     3416 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     3575 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3803 2022-12-30 09:03:16.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_document.py
--rw-rw-rw-   0        0        0     3249 2022-12-30 09:06:12.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_text.py
--rw-rw-rw-   0        0        0     2711 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     5521 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_file.py
--rw-rw-rw-   0        0        0     4348 2022-12-30 09:07:44.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/text_response.py
--rw-rw-rw-   0        0        0    14697 2022-12-23 16:57:19.000000 groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/rest.py
--rw-rw-rw-   0        0        0       42 2023-04-26 08:46:24.547112 groupdocs-rewriter-cloud-23.4/setup.cfg
--rw-rw-rw-   0        0        0     3255 2023-04-26 08:39:17.000000 groupdocs-rewriter-cloud-23.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:46:24.545115 groupdocs-rewriter-cloud-23.4/test/
--rw-rw-rw-   0        0        0     1441 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/__init__.py
--rw-rw-rw-   0        0        0     3534 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_helper.py
--rw-rw-rw-   0        0        0     3483 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_rewriter_api.py
--rw-rw-rw-   0        0        0    13208 2022-12-30 22:38:33.000000 groupdocs-rewriter-cloud-23.4/test/test_storage_api.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:38.194774 groupdocs-rewriter-cloud-23.6/
+-rw-rw-rw-   0        0        0    16123 2023-06-23 09:09:38.193780 groupdocs-rewriter-cloud-23.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12999 2023-06-23 08:50:15.000000 groupdocs-rewriter-cloud-23.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:37.919622 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/
+-rw-rw-rw-   0        0        0    16123 2023-06-23 09:09:37.000000 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-06-23 09:09:37.000000 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:09:37.000000 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-06-23 09:09:37.000000 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-23 09:09:37.000000 groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:37.956529 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/
+-rw-rw-rw-   0        0        0     1665 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:37.988481 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/
+-rw-rw-rw-   0        0        0     1482 2023-06-21 18:48:41.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/__init__.py
+-rw-rw-rw-   0        0        0    16443 2023-06-21 18:48:41.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/rewriter_api.py
+-rw-rw-rw-   0        0        0    56910 2023-06-21 18:48:41.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/storage_api.py
+-rw-rw-rw-   0        0        0    25431 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api_client.py
+-rw-rw-rw-   0        0        0    10057 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:38.156576 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/
+-rw-rw-rw-   0        0        0     2094 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/__init__.py
+-rw-rw-rw-   0        0        0     2972 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/base_model.py
+-rw-rw-rw-   0        0        0     3556 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     3718 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/document_response.py
+-rw-rw-rw-   0        0        0     4586 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/error.py
+-rw-rw-rw-   0        0        0     3377 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/error_details.py
+-rw-rw-rw-   0        0        0     7202 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/file_version.py
+-rw-rw-rw-   0        0        0     2650 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     2682 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/files_list.py
+-rw-rw-rw-   0        0        0     3416 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     3575 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3803 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/rewrite_document.py
+-rw-rw-rw-   0        0        0     3249 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/rewrite_text.py
+-rw-rw-rw-   0        0        0     2711 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     5521 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     3660 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/summarize_document.py
+-rw-rw-rw-   0        0        0     2464 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/summarize_text.py
+-rw-rw-rw-   0        0        0     4348 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/text_response.py
+-rw-rw-rw-   0        0        0    14697 2023-06-21 18:45:45.000000 groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/rest.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:09:38.194774 groupdocs-rewriter-cloud-23.6/setup.cfg
+-rw-rw-rw-   0        0        0     3258 2023-06-21 18:40:22.000000 groupdocs-rewriter-cloud-23.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:09:38.191823 groupdocs-rewriter-cloud-23.6/test/
+-rw-rw-rw-   0        0        0     1441 2023-06-21 18:41:19.000000 groupdocs-rewriter-cloud-23.6/test/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-06-21 18:41:19.000000 groupdocs-rewriter-cloud-23.6/test/test_helper.py
+-rw-rw-rw-   0        0        0     3483 2023-06-21 18:41:30.000000 groupdocs-rewriter-cloud-23.6/test/test_rewriter_api.py
+-rw-rw-rw-   0        0        0    13208 2023-06-21 18:41:30.000000 groupdocs-rewriter-cloud-23.6/test/test_storage_api.py
```

### Comparing `groupdocs-rewriter-cloud-23.4/PKG-INFO` & `groupdocs-rewriter-cloud-23.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-rewriter-cloud
-Version: 23.4
+Version: 23.6
 Summary: GroupDocs.Rewriter Cloud SDK
 Home-page: https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python
 Author: Aspose
 Author-email: ekaterina.tretiak@aspose.com
 License: MIT
 Description: # Python SDK for GroupDocs.Rewriter Cloud
         
@@ -55,18 +55,19 @@
         .PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
         .MD                | .MD<br />
         .HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
         
         ## Supported languages
         
         - **ar** — to paraphrase Arabic text or document
-        — **de** — to paraphrase German text or document
+        - **de** — to paraphrase German text or document
         - **en** — to paraphrase English text or document
-        — **fr** — to paraphrase French text or document
-        — **id** — to paraphrase Indonesian text or document
+        - **es** — to paraphrase Spanish text or document
+        - **fr** — to paraphrase French text or document
+        - **id** — to paraphrase Indonesian text or document
         - **ru** — to paraphrase Russian text or document
         - **uk** — to paraphrase Ukrainian text or document
         
         ## Quick start
         
         To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
         
@@ -163,18 +164,18 @@
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         language = "en"
         text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
         
-        rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
+        rewriter = RewriteText(language, text, diversity="medium", suggestions=2)
         request = rewriter.to_string()
-        res_text = api.post_rewrite_text(request)
-        print(res_text.message)
+        output = api.post_rewrite_text(request)
+        print(output.result)
         ```
         
         ### Rewrite a Word document
         
         ```python
         # Load the gem
         import groupdocs_rewriter_cloud
@@ -187,24 +188,77 @@
         api = RewriterApi(configuration)
         
         # Document paraphrasing
         language = "en"
         _format = "docx"
         outformat = "docx"
         storage = "internal"
-        name = "test_python.docx"
+        name = "test_file.docx"
         folder = ""
         savepath = ""
         savefile = "paraphrased.docx"
         
         rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
-        
         request = rewriter.to_string()
-        res_doc = api.post_rewrite_document(request)
-        print(res_doc.message)
+        output = api.post_rewrite_document(request)
+        print(output.message)
+        ```
+        
+        SDK also provides a tool for summarizing texts and documents in English. To do this, put the same parameters as for paraphrasing (except for "diversity" and "suggestions") in the requests body.
+        
+        ### Summarize a text
+        
+        ```python
+        # Load the gem
+        import groupdocs_rewriter_cloud
+        
+        # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+        my_client_id = ""
+        my_client_secret = ""
+        
+        # Create instance of the API
+        configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+        api = RewriterApi(configuration)
+        
+        language = "en"
+        text = "The modern Olympic Games are the leading international sporting events featuring summer and winter sports competitions in which thousands of athletes from around the world participate in a variety of competitions. The Olympic Games are considered the world's foremost sports competition with more than 200 teams, representing sovereign states and territories, participating. The Olympic Games are normally held every four years, and since 1994, have alternated between the Summer and Winter Olympics every two years during the four-year period."
+        
+        summarizer = SummarizeText(language, text)
+        request = summarizer.to_string()
+        output = api.post_summarize_text(request)
+        print(output.result)
+        ```
+        
+        ### Summarize a PDF document
+        
+        ```python
+        # Load the gem
+        import groupdocs_rewriter_cloud
+        # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+        my_client_id = ""
+        my_client_secret = ""
+        
+        # Create instance of the API
+        configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+        api = RewriterApi(configuration)
+        
+        # Document summarization
+        language = "en"
+        _format = "pdf"
+        outformat = "pdf"
+        storage = "internal"
+        name = "test_file.pdf"
+        folder = ""
+        savepath = ""
+        savefile = "summarized.pdf"
+        
+        summarizer = SummarizeDocument(language, _format, outformat, storage, name, folder, savepath, savefile)
+        request = summarizer.to_string()
+        output = api.post_summarize_document(request)
+        print(output.message)
         ```
         
         ## Other SDKs for GroupDocs.Rewriter Cloud
         
         GroupDocs also offers native SDK packages for other popular programming languages:
         
         ### .NET
@@ -212,15 +266,15 @@
         - [NuGet](https://www.nuget.org/packages/GroupDocs.Rewriter-Cloud/)
         - [GitHub](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-dotnet)
         
         ---
         
         [Product Page](https://products.groupdocs.cloud/rewriter/dotnet/) | [Docs](https://docs.groupdocs.cloud/rewriter/) | [Demos](https://products.groupdocs.app/rewriter/family) | [Swagger UI](https://apireference.groupdocs.cloud/rewriter/) | [Examples](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-dotnet) | [Blog](https://blog.groupdocs.cloud/category/rewriter/) | [Search](https://search.groupdocs.cloud/) | [Free Support](https://forum.groupdocs.cloud/c/rewriter) | [Free Trial](https://purchase.groupdocs.cloud/trial)
         
-Keywords: GroupDocs.Rewriter Cloud API Reference,Aspose,GroupDocs,RewriterRewriter Cloud
+Keywords: GroupDocs.Rewriter Cloud API Reference,Aspose,GroupDocs,Rewriter,Rewriter Cloud
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `groupdocs-rewriter-cloud-23.4/README.md` & `groupdocs-rewriter-cloud-23.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 .PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
 .MD                | .MD<br />
 .HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
 
 ## Supported languages
 
 - **ar** — to paraphrase Arabic text or document
-— **de** — to paraphrase German text or document
+- **de** — to paraphrase German text or document
 - **en** — to paraphrase English text or document
-— **fr** — to paraphrase French text or document
-— **id** — to paraphrase Indonesian text or document
+- **es** — to paraphrase Spanish text or document
+- **fr** — to paraphrase French text or document
+- **id** — to paraphrase Indonesian text or document
 - **ru** — to paraphrase Russian text or document
 - **uk** — to paraphrase Ukrainian text or document
 
 ## Quick start
 
 To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
 
@@ -155,18 +156,18 @@
 # Create instance of the API
 configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
 api = RewriterApi(configuration)
 
 language = "en"
 text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
 
-rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
+rewriter = RewriteText(language, text, diversity="medium", suggestions=2)
 request = rewriter.to_string()
-res_text = api.post_rewrite_text(request)
-print(res_text.message)
+output = api.post_rewrite_text(request)
+print(output.result)
 ```
 
 ### Rewrite a Word document
 
 ```python
 # Load the gem
 import groupdocs_rewriter_cloud
@@ -179,24 +180,77 @@
 api = RewriterApi(configuration)
 
 # Document paraphrasing
 language = "en"
 _format = "docx"
 outformat = "docx"
 storage = "internal"
-name = "test_python.docx"
+name = "test_file.docx"
 folder = ""
 savepath = ""
 savefile = "paraphrased.docx"
 
 rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
-
 request = rewriter.to_string()
-res_doc = api.post_rewrite_document(request)
-print(res_doc.message)
+output = api.post_rewrite_document(request)
+print(output.message)
+```
+
+SDK also provides a tool for summarizing texts and documents in English. To do this, put the same parameters as for paraphrasing (except for "diversity" and "suggestions") in the requests body.
+
+### Summarize a text
+
+```python
+# Load the gem
+import groupdocs_rewriter_cloud
+
+# Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+my_client_id = ""
+my_client_secret = ""
+
+# Create instance of the API
+configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+api = RewriterApi(configuration)
+
+language = "en"
+text = "The modern Olympic Games are the leading international sporting events featuring summer and winter sports competitions in which thousands of athletes from around the world participate in a variety of competitions. The Olympic Games are considered the world's foremost sports competition with more than 200 teams, representing sovereign states and territories, participating. The Olympic Games are normally held every four years, and since 1994, have alternated between the Summer and Winter Olympics every two years during the four-year period."
+
+summarizer = SummarizeText(language, text)
+request = summarizer.to_string()
+output = api.post_summarize_text(request)
+print(output.result)
+```
+
+### Summarize a PDF document
+
+```python
+# Load the gem
+import groupdocs_rewriter_cloud
+# Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+my_client_id = ""
+my_client_secret = ""
+
+# Create instance of the API
+configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+api = RewriterApi(configuration)
+
+# Document summarization
+language = "en"
+_format = "pdf"
+outformat = "pdf"
+storage = "internal"
+name = "test_file.pdf"
+folder = ""
+savepath = ""
+savefile = "summarized.pdf"
+
+summarizer = SummarizeDocument(language, _format, outformat, storage, name, folder, savepath, savefile)
+request = summarizer.to_string()
+output = api.post_summarize_document(request)
+print(output.message)
 ```
 
 ## Other SDKs for GroupDocs.Rewriter Cloud
 
 GroupDocs also offers native SDK packages for other popular programming languages:
 
 ### .NET
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/PKG-INFO` & `groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-rewriter-cloud
-Version: 23.4
+Version: 23.6
 Summary: GroupDocs.Rewriter Cloud SDK
 Home-page: https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-python
 Author: Aspose
 Author-email: ekaterina.tretiak@aspose.com
 License: MIT
 Description: # Python SDK for GroupDocs.Rewriter Cloud
         
@@ -55,18 +55,19 @@
         .PDF               | .PDF<br />.DOCX<br />.PPTX<br />.HTML<br />.XPS<br />.SVG
         .MD                | .MD<br />
         .HTML              | .HTML<br />.PDF<br />.DOCX<br />.TIFF<br />.XPS<br />
         
         ## Supported languages
         
         - **ar** — to paraphrase Arabic text or document
-        — **de** — to paraphrase German text or document
+        - **de** — to paraphrase German text or document
         - **en** — to paraphrase English text or document
-        — **fr** — to paraphrase French text or document
-        — **id** — to paraphrase Indonesian text or document
+        - **es** — to paraphrase Spanish text or document
+        - **fr** — to paraphrase French text or document
+        - **id** — to paraphrase Indonesian text or document
         - **ru** — to paraphrase Russian text or document
         - **uk** — to paraphrase Ukrainian text or document
         
         ## Quick start
         
         To start using GroupDocs.Rewriter Cloud in your Python applications, follow a few simple steps:
         
@@ -163,18 +164,18 @@
         # Create instance of the API
         configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
         api = RewriterApi(configuration)
         
         language = "en"
         text = "GroupDocs Cloud customers come from a wide variety of industries and can be found all over the globe."
         
-        rewriter = RewriteText(language, text, diversity = "medium", suggestions=2)
+        rewriter = RewriteText(language, text, diversity="medium", suggestions=2)
         request = rewriter.to_string()
-        res_text = api.post_rewrite_text(request)
-        print(res_text.message)
+        output = api.post_rewrite_text(request)
+        print(output.result)
         ```
         
         ### Rewrite a Word document
         
         ```python
         # Load the gem
         import groupdocs_rewriter_cloud
@@ -187,24 +188,77 @@
         api = RewriterApi(configuration)
         
         # Document paraphrasing
         language = "en"
         _format = "docx"
         outformat = "docx"
         storage = "internal"
-        name = "test_python.docx"
+        name = "test_file.docx"
         folder = ""
         savepath = ""
         savefile = "paraphrased.docx"
         
         rewriter = RewriteDocument(language, _format, outformat, storage, name, folder, savepath, savefile, diversity="medium")
-        
         request = rewriter.to_string()
-        res_doc = api.post_rewrite_document(request)
-        print(res_doc.message)
+        output = api.post_rewrite_document(request)
+        print(output.message)
+        ```
+        
+        SDK also provides a tool for summarizing texts and documents in English. To do this, put the same parameters as for paraphrasing (except for "diversity" and "suggestions") in the requests body.
+        
+        ### Summarize a text
+        
+        ```python
+        # Load the gem
+        import groupdocs_rewriter_cloud
+        
+        # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+        my_client_id = ""
+        my_client_secret = ""
+        
+        # Create instance of the API
+        configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+        api = RewriterApi(configuration)
+        
+        language = "en"
+        text = "The modern Olympic Games are the leading international sporting events featuring summer and winter sports competitions in which thousands of athletes from around the world participate in a variety of competitions. The Olympic Games are considered the world's foremost sports competition with more than 200 teams, representing sovereign states and territories, participating. The Olympic Games are normally held every four years, and since 1994, have alternated between the Summer and Winter Olympics every two years during the four-year period."
+        
+        summarizer = SummarizeText(language, text)
+        request = summarizer.to_string()
+        output = api.post_summarize_text(request)
+        print(output.result)
+        ```
+        
+        ### Summarize a PDF document
+        
+        ```python
+        # Load the gem
+        import groupdocs_rewriter_cloud
+        # Get Client Id and Client Secret from https://dashboard.groupdocs.cloud
+        my_client_id = ""
+        my_client_secret = ""
+        
+        # Create instance of the API
+        configuration = Configuration(apiKey=my_client_secret, appSid=my_client_id)
+        api = RewriterApi(configuration)
+        
+        # Document summarization
+        language = "en"
+        _format = "pdf"
+        outformat = "pdf"
+        storage = "internal"
+        name = "test_file.pdf"
+        folder = ""
+        savepath = ""
+        savefile = "summarized.pdf"
+        
+        summarizer = SummarizeDocument(language, _format, outformat, storage, name, folder, savepath, savefile)
+        request = summarizer.to_string()
+        output = api.post_summarize_document(request)
+        print(output.message)
         ```
         
         ## Other SDKs for GroupDocs.Rewriter Cloud
         
         GroupDocs also offers native SDK packages for other popular programming languages:
         
         ### .NET
@@ -212,15 +266,15 @@
         - [NuGet](https://www.nuget.org/packages/GroupDocs.Rewriter-Cloud/)
         - [GitHub](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-dotnet)
         
         ---
         
         [Product Page](https://products.groupdocs.cloud/rewriter/dotnet/) | [Docs](https://docs.groupdocs.cloud/rewriter/) | [Demos](https://products.groupdocs.app/rewriter/family) | [Swagger UI](https://apireference.groupdocs.cloud/rewriter/) | [Examples](https://github.com/groupdocs-rewriter-cloud/groupdocs-rewriter-cloud-dotnet) | [Blog](https://blog.groupdocs.cloud/category/rewriter/) | [Search](https://search.groupdocs.cloud/) | [Free Support](https://forum.groupdocs.cloud/c/rewriter) | [Free Trial](https://purchase.groupdocs.cloud/trial)
         
-Keywords: GroupDocs.Rewriter Cloud API Reference,Aspose,GroupDocs,RewriterRewriter Cloud
+Keywords: GroupDocs.Rewriter Cloud API Reference,Aspose,GroupDocs,Rewriter,Rewriter Cloud
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocs_rewriter_cloud.egg-info/SOURCES.txt` & `groupdocs-rewriter-cloud-23.6/groupdocs_rewriter_cloud.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,12 +23,14 @@
 groupdocsrewritercloud/models/files_list.py
 groupdocsrewritercloud/models/files_upload_result.py
 groupdocsrewritercloud/models/object_exist.py
 groupdocsrewritercloud/models/rewrite_document.py
 groupdocsrewritercloud/models/rewrite_text.py
 groupdocsrewritercloud/models/storage_exist.py
 groupdocsrewritercloud/models/storage_file.py
+groupdocsrewritercloud/models/summarize_document.py
+groupdocsrewritercloud/models/summarize_text.py
 groupdocsrewritercloud/models/text_response.py
 test/__init__.py
 test/test_helper.py
 test/test_rewriter_api.py
 test/test_storage_api.py
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/__init__.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # s"""Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="__init__.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/__init__.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="__init__.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api/storage_api.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="storage_api.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/api_client.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="api_client.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # 
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/configuration.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="configuration.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # 
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/__init__.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="__init__.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/base_model.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="base_model.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/disc_usage.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/disc_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="disc_usage.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/document_response.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="document_response.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="error.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/error_details.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="error_details.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_version.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/file_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="file_version.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/file_versions.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/file_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="file_versions.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_list.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/files_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="files_list.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/files_upload_result.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="files_upload_result.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/object_exist.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/object_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="object_exist.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_document.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/rewrite_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="rewrite_document.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/rewrite_text.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/rewrite_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="rewrite_text.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_exist.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/storage_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="storage_exist.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/storage_file.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/storage_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="storage_file.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/models/text_response.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/models/text_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="text_response.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/groupdocsrewritercloud/rest.py` & `groupdocs-rewriter-cloud-23.6/groupdocsrewritercloud/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """Copyright
 # --------------------------------------------------------------------------------------------------------------------
 # <copyright company="Aspose" file="rest.py">
-# Copyright (c) 2022 GroupDocs.Rewriter Cloud
+# Copyright (c) 2023 GroupDocs.Rewriter Cloud
 # </copyright>
 # 
 # <summary>
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `groupdocs-rewriter-cloud-23.4/setup.py` & `groupdocs-rewriter-cloud-23.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages
 from os import path
 
 NAME = "groupdocs-rewriter-cloud"
-VERSION = "23.4"
+VERSION = "23.6"
+
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -49,15 +50,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8'
     ],
-    keywords=["GroupDocs.Rewriter Cloud API Reference", "Aspose", "GroupDocs", "Rewriter" "Rewriter Cloud"],
+    keywords=["GroupDocs.Rewriter Cloud API Reference", "Aspose", "GroupDocs", "Rewriter", "Rewriter Cloud"],
     install_requires=REQUIRES,
     packages=find_packages(),
     include_package_data=True
     # long_description="""
     # GroupDocs.Rewriter Cloud API Reference
     # This package contains GroupDocs.Rewriter Cloud SDK for Python.
     # This SDK allows you to work with GroupDocs.Rewriter Cloud REST APIs in your Python applications, and integrate Rewriter functionality in few steps.
```

### Comparing `groupdocs-rewriter-cloud-23.4/test/__init__.py` & `groupdocs-rewriter-cloud-23.6/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 """
 --------------------------------------------------------------------------------------------------------------------
  <copyright company="Aspose" file="__init__.py">
-   Copyright (c) 2022 GroupDocs.Rewriter Cloud
+   Copyright (c) 2023 GroupDocs.Rewriter Cloud
  </copyright>
  <summary>
   Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/test/test_helper.py` & `groupdocs-rewriter-cloud-23.6/test/test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 # """
 # --------------------------------------------------------------------------------------------------------------------
 #  <copyright company="Aspose" file="test_helper.py">
-#    Copyright (c) 2022 GroupDocs.Rewriter Cloud
+#    Copyright (c) 2023 GroupDocs.Rewriter Cloud
 #  </copyright>
 #  <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/test/test_rewriter_api.py` & `groupdocs-rewriter-cloud-23.6/test/test_rewriter_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 # """
 # --------------------------------------------------------------------------------------------------------------------
 #  <copyright company="Aspose" file="test_rewriter_api.py">
-#    Copyright (c) 2022 GroupDocs.Rewriter Cloud
+#    Copyright (c) 2023 GroupDocs.Rewriter Cloud
 #  </copyright>
 #  <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-rewriter-cloud-23.4/test/test_storage_api.py` & `groupdocs-rewriter-cloud-23.6/test/test_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 # """
 # --------------------------------------------------------------------------------------------------------------------
 #  <copyright company="Aspose" file="test_storage_api.py">
-#    Copyright (c) 2022 GroupDocs.Rewriter Cloud
+#    Copyright (c) 2023 GroupDocs.Rewriter Cloud
 #  </copyright>
 #  <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

