# Comparing `tmp/talkytrend-1.3.5.tar.gz` & `tmp/talkytrend-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.3.5.tar", max compression
+gzip compressed data, was "talkytrend-1.4.0.tar", max compression
```

## Comparing `talkytrend-1.3.5.tar` & `talkytrend-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-22 09:00:11.587352 talkytrend-1.3.5/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-22 09:00:11.587352 talkytrend-1.3.5/README.md
--rw-r--r--   0        0        0     2178 2023-06-22 09:00:12.275374 talkytrend-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-22 09:00:12.275374 talkytrend-1.3.5/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-22 09:00:11.591352 talkytrend-1.3.5/talkytrend/config.py
--rw-r--r--   0        0        0      932 2023-06-22 09:00:11.591352 talkytrend-1.3.5/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6121 2023-06-22 09:00:11.591352 talkytrend-1.3.5/talkytrend/main.py
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-23 18:35:47.369806 talkytrend-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-23 18:35:47.369806 talkytrend-1.4.0/README.md
+-rw-r--r--   0        0        0     2178 2023-06-23 18:35:48.365837 talkytrend-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 18:35:48.365837 talkytrend-1.4.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-23 18:35:47.369806 talkytrend-1.4.0/talkytrend/config.py
+-rw-r--r--   0        0        0     1653 2023-06-23 18:35:47.369806 talkytrend-1.4.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6419 2023-06-23 18:35:47.369806 talkytrend-1.4.0/talkytrend/main.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 talkytrend-1.4.0/PKG-INFO
```

### Comparing `talkytrend-1.3.5/LICENSE` & `talkytrend-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.5/README.md` & `talkytrend-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.5/pyproject.toml` & `talkytrend-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.3.5"
+version = "1.4.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.3.5/talkytrend/config.py` & `talkytrend-1.4.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.3.5/talkytrend/default_settings.toml` & `talkytrend-1.4.0/talkytrend/default_settings.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [default]
+VALUE = "On Default"
 talkytrend_enabled = true
 talkytrend_mode = "scanner"
 talkytrend_scanner = false
 talkytrend_scheduler = false
 scanner_frequency = 86400
 enable_signals = true
 assets = [
@@ -11,14 +12,31 @@
     #use https://tvdb.brianthe.dev/ to get details
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
+fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
 enable_news = true
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 [testing]
 VALUE = "On Testing"
+talkytrend_enabled = true
+talkytrend_mode = "scanner"
+talkytrend_scanner = false
+talkytrend_scheduler = false
+scanner_frequency = 86400
+enable_signals = true
+assets = [
+    { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
+]
+enable_events = true
+economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
+fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
+enable_news = true
+news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
+news_api_key = ""
+live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
```

### Comparing `talkytrend-1.3.5/talkytrend/main.py` & `talkytrend-1.4.0/talkytrend/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,16 +67,15 @@
                     table.add_row([asset["id"], current_signal])
                     signals.append(signal_item)
             #return signals
             #return str(table)
             # table.border = False
             table.set_style(MARKDOWN)
 
-            table_text = table.get_string()
-            return table_text
+            return table.get_string()
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
 
 
     def is_new_signal(self, asset_id, interval, current_signal):
@@ -93,47 +92,62 @@
         self.asset_signals[asset_id][interval] = current_signal
 
 
     def get_asset_signals(self):
         return self.asset_signals
 
     async def fetch_key_events(self):
-        try:
-            async with aiohttp.ClientSession() as session:
-                async with session.get(self.economic_calendar, timeout=10) as response:
-                    if response.status == 200:
-                        event_list = await response.json()
-                        today = date.today().isoformat()
-                        for event in event_list:
-                            impact = event.get('impact')
-                            country = event.get('country')
-                            title = event.get('title')
-                            event_date = event.get('date')
-                            if event_date and event_date.startswith(today):
-                                if impact == 'High' and country in {'USD', 'ALL'}:
-                                    return f"💬 {title}\n⏰ {event_date}"
-                                if "OPEC" in title or "FOMC" in title:
-                                    return f"💬 {title}\n⏰ {event_date}"
-            return None
-        except Exception as error:
-            self.logger.error("event %s",error)
+        def filter_events(data, today):
+            return [event for event in data if event.get('date', '').startswith(today)]
+
+        def is_usd_high_impact(event):
+            return event.get('impact') == 'High' and event.get('country') in {'USD', 'ALL'}
+
+        def is_all_high_impact(event):
+            return event.get('impact') == 'High' and event.get('country') == 'ALL'
+
+        def is_opec_or_fomc(event):
+            return "OPEC" in event.get('title') or "FOMC" in event.get('title')
+
+        def format_event(event):
+            return f"💬 {event['title']}\n⏰ {event['date']}"
+    
+        async with aiohttp.ClientSession() as session:
+            async with session.get(self.economic_calendar, timeout=10) as response:
+                response.raise_for_status()
+                data = await response.json()
+                today = date.today().isoformat()
+                events = filter_events(data, today)
+                for event in events:
+                    if is_usd_high_impact(event) or is_all_high_impact(event):
+                        return format_event(event)
+                    if is_opec_or_fomc(event):
+                        return format_event(event)
+        return None
+
+
     
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
                     key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
                     last_item = key_news[-1]
                     return f"{last_item['title']} {last_item['url']}"
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
+    async def check_fomc(self):
+        event_dates = settings.fomc_decision_date
+        current_date = date.today().isoformat()
+        return any(event.startswith(current_date) for event in event_dates)
+
 
     async def scanner(self):
         while True:
             try:
                 if settings.enable_events:
                     key_events = await self.fetch_key_events()
                     if key_events is not None:
```

### Comparing `talkytrend-1.3.5/PKG-INFO` & `talkytrend-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.3.5
+Version: 1.4.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

