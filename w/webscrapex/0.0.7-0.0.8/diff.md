# Comparing `tmp/webscrapex-0.0.7.tar.gz` & `tmp/webscrapex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapex-0.0.7.tar", max compression
+gzip compressed data, was "webscrapex-0.0.8.tar", max compression
```

## Comparing `webscrapex-0.0.7.tar` & `webscrapex-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      772 2023-06-19 05:19:40.581293 webscrapex-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2406 2023-06-19 05:12:49.699574 webscrapex-0.0.7/README.md
--rw-r--r--   0        0        0       48 2023-06-19 05:19:29.840530 webscrapex-0.0.7/WebScrapeX/__init__.py
--rw-r--r--   0        0        0    14722 2023-06-13 17:43:15.245938 webscrapex-0.0.7/WebScrapeX/WebScrapeX.py
--rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 webscrapex-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-06-23 07:07:47.606673 webscrapex-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2406 2023-06-19 05:12:49.699574 webscrapex-0.0.8/README.md
+-rw-r--r--   0        0        0       48 2023-06-23 07:07:39.418396 webscrapex-0.0.8/WebScrapeX/__init__.py
+-rw-r--r--   0        0        0    14722 2023-06-23 07:07:03.880342 webscrapex-0.0.8/WebScrapeX/WebScrapeX.py
+-rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 webscrapex-0.0.8/PKG-INFO
```

### Comparing `webscrapex-0.0.7/pyproject.toml` & `webscrapex-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebScrapeX"
-version = "0.0.7"
+version = "0.0.8"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/WebScrapeX"
 repository = "https://github.com/ILisa250/WebScrapeX"
 keywords = ["WebScrapeX", "web-data-extraction", "web-scraping", "web data collection",
```

### Comparing `webscrapex-0.0.7/README.md` & `webscrapex-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `webscrapex-0.0.7/WebScrapeX/WebScrapeX.py` & `webscrapex-0.0.8/WebScrapeX/WebScrapeX.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         >>> from web_data_extraction import scrape_clean_save_data
         scrape_clean_save_data("link/url", "filename", ".envfilepath(with credentials)")
         
         """
         # Empty list to store links
         Links = []
         #Looping through the pages
-        for page in range(1,11):
+        for page in range(1,16):
             # Headers used to specify how the HTTP request should be processed by the server. 
             # i.e - User-Agent header specifying the user agent string that should be sent with the request,
             # - Accept header specifying the types of content that the client can handle.
             headers = {'Accept-Encoding': 'gzip, deflate, sdch','Accept-Language': 'en-US,en;q=0.8','Upgrade-Insecure-Requests': '1',
                        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
                        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                        'Cache-Control': 'max-age=0','Connection': 'keep-alive',}      
@@ -70,15 +70,15 @@
                 # Loop through every house's link
                 for div in soup.findAll('div', {'class': 'item-list'}):
                     # Find the link for the current property
                     link = div.find('a').attrs['href']
                     # Keep the links in the Links list
                     Links.append("https://imali.biz" + link) 
                 # Break the loop after collecting the first 10 page
-                if page == 10:
+                if page == 15:
                     break
             except requests.exceptions.RequestException as e:
                 print(f"An error occurred while fetching data: {e}")
         # Create a DataFrame from the list
         imali_data = pd.DataFrame({f'{filename}_links': Links})
         imali_data.to_csv(f"{filename}_links.csv")
```

### Comparing `webscrapex-0.0.7/PKG-INFO` & `webscrapex-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapex
-Version: 0.0.7
+Version: 0.0.8
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/WebScrapeX
 License: MIT
 Keywords: WebScrapeX,web-data-extraction,web-scraping,web data collection,web data integration,web data aggregation,automated data extraction,Lisa Yvette INYANGE
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3,<4
```

