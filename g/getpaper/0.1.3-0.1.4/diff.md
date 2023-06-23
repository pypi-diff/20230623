# Comparing `tmp/getpaper-0.1.3.tar.gz` & `tmp/getpaper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.3.tar", last modified: Thu Jun 22 20:58:07 2023, max compression
+gzip compressed data, was "getpaper-0.1.4.tar", last modified: Fri Jun 23 01:02:25 2023, max compression
```

## Comparing `getpaper-0.1.3.tar` & `getpaper-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.3/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4019 2023-06-22 20:58:07.287085 getpaper-0.1.3/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3404 2023-06-22 20:56:44.000000 getpaper-0.1.3/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.3/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6944 2023-06-22 20:56:44.000000 getpaper-0.1.3/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.3/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5455 2023-06-21 21:39:55.000000 getpaper-0.1.3/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.3/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-22 20:58:07.287085 getpaper-0.1.3/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4019 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-22 20:58:07.000000 getpaper-0.1.3/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-22 20:58:07.287085 getpaper-0.1.3/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-22 20:56:44.000000 getpaper-0.1.3/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.4/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3965 2023-06-23 01:02:25.874754 getpaper-0.1.4/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3350 2023-06-23 01:02:04.000000 getpaper-0.1.4/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.4/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6949 2023-06-23 01:00:00.000000 getpaper-0.1.4/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.4/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6795 2023-06-23 00:55:10.000000 getpaper-0.1.4/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.4/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3965 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 01:02:25.874754 getpaper-0.1.4/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-23 01:02:04.000000 getpaper-0.1.4/setup.py
```

### Comparing `getpaper-0.1.3/LICENSE` & `getpaper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.3/PKG-INFO` & `getpaper-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.3
+Version: 0.1.4
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -60,26 +60,26 @@
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
               ('10.1038/s41597-020-00710-z',
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
  ['wrong'])
 ```
 Same function can be called from the command line:
 ```bash
-download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
+getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
 ```
-You can also parse papers on a per file basis, for example:
+You can also parse papers on a per-file basis, for example:
 ```bash
-getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
+getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
```

### Comparing `getpaper-0.1.3/README.md` & `getpaper-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -42,26 +42,26 @@
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
               ('10.1038/s41597-020-00710-z',
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
  ['wrong'])
 ```
 Same function can be called from the command line:
 ```bash
-download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
+getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
 ```
-You can also parse papers on a per file basis, for example:
+You can also parse papers on a per-file basis, for example:
 ```bash
-getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
+getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
```

### Comparing `getpaper-0.1.3/getpaper/download.py` & `getpaper-0.1.4/getpaper/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 def download_pubmed_command(pubmed: str, folder: str, skip_existing: bool, name: Optional[str]):
     where = Path(folder)
     where.mkdir(exist_ok=True, parents=True)
     custom_name = pubmed if name == "pmid" or name == "PMID" else name
     return download_pubmed(pubmed, where, skip_existing, custom_name)
 
 @app.command("download_papers")
-@click.argument('dois', nargs=-1)
+@click.option('--dois', multiple=True)
 @click.option('--folder', type=click.Path(), default=".", help="where to download the paper")
 @click.option('--threads', '-t', type=int, default=5, help='Number of threads (default: 5)')
 def download_papers_command(dois: List[str], folder: str, threads: int):
     """Downloads papers with the given DOIs to the specified destination."""
     if not dois:
         dois = []
     # Call the actual function with the provided arguments
```

### Comparing `getpaper-0.1.3/getpaper/index.py` & `getpaper-0.1.4/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.3/getpaper/parse.py` & `getpaper-0.1.4/getpaper/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,14 +71,42 @@
                 doc = Document(
                     page_content = text,
                     metadata={"source": doi}
                 )
                 docs.append(doc)
     return docs
 
+import asyncio
+from concurrent.futures import ThreadPoolExecutor
+
+def parse_papers_async(parse_folder: Path, destination: Optional[Path] = None,
+                 mode: str = "single", strategy: str = "auto",
+                 pdf_infer_table_structure: bool = True,
+                 include_page_breaks: bool = False,
+                 threads: int = 5):
+    papers: list[Path] = traverse(parse_folder, lambda p: "pdf" in p.suffix)
+    print(f"indexing {len(papers)} papers")
+
+    async def async_parse_paper(paper):
+        loop = asyncio.get_running_loop()
+        where = destination if destination is not None else paper.parent
+        return await loop.run_in_executor(
+            executor, parse_paper, paper, where, mode, strategy, pdf_infer_table_structure, include_page_breaks
+        )
+
+    executor = ThreadPoolExecutor(max_workers=threads)
+
+    loop = asyncio.get_event_loop()
+    tasks = [async_parse_paper(paper) for paper in papers]
+    parsed_papers = loop.run_until_complete(asyncio.gather(*tasks))
+
+    print("papers parsing finished!")
+    return parsed_papers
+
+
 @click.group(invoke_without_command=False)
 @click.pass_context
 def app(ctx: Context):
     #if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
     #    test_index()
     pass
@@ -99,16 +127,20 @@
 @app.command("parse_folder")
 @click.option('--folder', type=click.Path(exists=True), help="folder to parse papers in")
 @click.option('--destination', type=click.STRING, default=None, help="destination folder")
 @click.option('--mode', type=click.Choice(["single", "elements", "paged"]), default="single", help="paper mode to be used")
 @click.option('--strategy', type=click.Choice(["auto", "hi_res", "fast"]), default="auto", help="parsing strategy to be used, auto by default")
 @click.option('--infer_tables', type=click.BOOL, default=True, help="if the table structure should be inferred")
 @click.option('--include_page_breaks', type=click.BOOL, default=False, help="if page breaks should be included")
-def parse_paper_command(folder: str,destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool):
+@click.option('--threads', '-t', type=int, default=1, help='Number of threads (default: 5)')
+def parse_paper_command(folder: str,destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, threads: int):
     parse_folder = Path(folder)
     destination_folder = Path(destination) if destination is not None else None
     print(f"parsing paper {folder} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
-    return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks)
+    if threads <2:
+        return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks)
+    else:
+        return parse_papers_async(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks)
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `getpaper-0.1.3/getpaper/splitter.py` & `getpaper-0.1.4/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.3/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.4/getpaper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.3
+Version: 0.1.4
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -60,26 +60,26 @@
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.3390/ijms22031073.pdf')),
               ('10.1038/s41597-020-00710-z',
                PosixPath('/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers/10.1038/s41597-020-00710-z.pdf'))]),
  ['wrong'])
 ```
 Same function can be called from the command line:
 ```bash
-download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder ""/home/antonkulaga/sources/getpaper/notebooks/data/output/test/papers" --threads 5
+download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
 You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
 ```bash
-getpaper/parse.py parse_folder --folder /home/antonkulaga/sources/getpaper/test
+getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
 ```
-You can also parse papers on a per file basis, for example:
+You can also parse papers on a per-file basis, for example:
 ```bash
-getpaper/parse.py parse_paper --paper /home/antonkulaga/sources/getpaper/test/22266545.pdf
+getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
```

### Comparing `getpaper-0.1.3/setup.py` & `getpaper-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

