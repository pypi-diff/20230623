# Comparing `tmp/dipense-0.1.1.tar.gz` & `tmp/dipense-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipense-0.1.1.tar", last modified: Sun May 28 20:35:38 2023, max compression
+gzip compressed data, was "dipense-0.1.2.tar", last modified: Fri Jun 23 14:01:47 2023, max compression
```

## Comparing `dipense-0.1.1.tar` & `dipense-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.296496 dipense-0.1.1/
--rw-rw-r--   0 usman     (1000) usman     (1000)      138 2023-05-28 20:01:27.000000 dipense-0.1.1/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-05-28 19:56:33.000000 dipense-0.1.1/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       64 2023-05-28 20:31:21.000000 dipense-0.1.1/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     3657 2023-05-28 20:35:38.292496 dipense-0.1.1/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2043 2023-05-28 19:59:14.000000 dipense-0.1.1/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.280495 dipense-0.1.1/dipense/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2637 2023-05-28 20:01:37.000000 dipense-0.1.1/dipense/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1379 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/default.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/drone.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/icheckp.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1770 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/structure.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.292496 dipense-0.1.1/dipense.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3657 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-05-28 20:35:38.000000 dipense-0.1.1/dipense.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-05-28 20:35:38.296496 dipense-0.1.1/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     1706 2023-05-28 20:33:28.000000 dipense-0.1.1/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:47.012213 dipense-0.1.2/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      221 2023-06-23 13:56:36.000000 dipense-0.1.2/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-23 13:56:36.000000 dipense-0.1.2/LICENSE
+-rw-r--r--   0 usman     (1000) usman     (1000)       64 2023-06-20 05:06:50.000000 dipense-0.1.2/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3829 2023-06-23 14:01:47.000213 dipense-0.1.2/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2306 2023-06-23 13:56:36.000000 dipense-0.1.2/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:46.988212 dipense-0.1.2/dipense/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2626 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1351 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/default.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/drone.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/icheckp.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1750 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/structure.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:46.996213 dipense-0.1.2/dipense.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3829 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-23 14:01:47.012213 dipense-0.1.2/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2269 2023-06-23 14:01:37.000000 dipense-0.1.2/setup.py
```

### Comparing `dipense-0.1.1/LICENSE` & `dipense-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Usman Musa
+Copyright (c) 2023 Usman Musa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dipense-0.1.1/README.md` & `dipense-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 
 # DiPense
 
 An OSINT tool for IT ninjas
 
 
 # How to use the library
-
 First we recommend creating a virtual environment `python -m venv venv` and then activate it `source venv/bin/activate`
 
-Once that finish now install the library using `pip install dipense` and wait for the installation basically the library was uploaded using `sdist` (Source Distribution)
+Once that finish now install the library using
+
+```
+pip install --upgrade dipense
+```
+
+Wait for the installation to finish, basically the library was uploaded using `sdist` (Source Distribution)
 
 After that, create a new file let call it `route.py` in the file put the below code
 
 ```python
 from dipense import payloads
 from dipense.structure import helper
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     payloads(helper)
 ```
 
 save the file and navigate to where the file is located in terminal and your are ready to go
 
 To find information about a domain name run the file like:
 
@@ -78,15 +83,18 @@
 
 ```
 python route.py
 ```
 
 ## Useful links
 
-- Repository: https://github.com/usmanmusa1920/dipense
 - Documentation: https://dipense.readthedocs.io
-- PYPI Release: https://pypi.org/project/dipense
+- Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
-![DiPense at a glance](docs/screen-shot.png)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/screen-shot.png)](https://dipense.readthedocs.io)
+
+## DiPense at a glance (pypi)
+
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/dipense-terminal.png)](https://dipense.readthedocs.io)
```

### Comparing `dipense-0.1.1/dipense/__init__.py` & `dipense-0.1.2/dipense/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,41 +15,42 @@
   into the ICHECKP class, this will automatically open a map in
   your webbrowser, e.g
     _______________________________________________
     ICHECKP(autoOpenMap=True).icheckp('197.3.11.7')
     
 """
 
-__title__ = "dipense"
-__version__ = "0.1.1"
-__author__ = "Usman Musa"
-__author_email__ = "usmanmusa1920@gmail.com"
-__author_website__ = "https://usmanmusa1920.github.io"
-__repository__ = "https://github.com/usmanmusa1920/dipense-lib"
-__website__ = "https://dipense-lib.readthedocs.io"
-__copyright__ = "Copyright (C) 2022 - 2023 Usman Musa"
+__title__ = 'dipense'
+__version__ = '0.1.2'
+__author__ = 'Usman Musa'
+__author_email__ = 'usmanmusa1920@gmail.com'
+__author_website__ = 'https://usmanmusa1920.github.io'
+__repository__ = 'https://github.com/usmanmusa1920/dipense'
+__url__ = 'https://dipense.readthedocs.io'
+__copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
+
 
 import argparse
 from .icheckp import ICHECKP
 from .default import default
 from .default import Default
 
 
 # def icheckp(ip, autoOpenMap=False):
-#   print("The year is", default()["the_year"])
+#   print('The year is', default()['the_year'])
 
 getout = print
 def ipLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog="scan an ip address", description="This scan an ip address!")
+  parser = argparse.ArgumentParser(prog='scan an ip address', description='This scan an ip address!')
   
   # metavar make the -help to look cleaan
-  parser.add_argument("--ip", "-i", required=True, type=str, metavar="", help="What is the ip address?")
-  parser.add_argument("--open", "-o", default=False, required=False, type=str, metavar="", help="This will automatic open your map in web browser, it is a boolean of `True or False`")
-  parser.add_argument(dest="payloadip", default="payloadip", type=str, metavar="", help="The payload is to find an ip address infomation")
+  parser.add_argument('--ip', '-i', required=True, type=str, metavar='', help='What is the ip address?')
+  parser.add_argument('--open', '-o', default=False, required=False, type=str, metavar='', help='This will automatic open your map in web browser, it is a boolean of `True or False`')
+  parser.add_argument(dest='payloadip', default='payloadip', type=str, metavar='', help='The payload is to find an ip address infomation')
   
   args = parser.parse_args()
   ICHECKP(autoOpenMap=args.open).icheckp(args.ip)
   
   
 def payloads(helper):
   import sys
@@ -71,18 +72,18 @@
   this return a list of positional argument that
   can be use in the command line/terminal
   where we concatenate `dft` with each item in `lst_1`
   """
   lst_2 = [dft+i for i in lst_1]
   
   if len(sys.argv) == 1:
-    getout("\n Include a positional argument!")
+    getout('\n Include a positional argument!')
     getout(helper())
   elif sys.argv[1] not in lst_2:
-    getout(f"\n `{sys.argv[1]}` is not a valid positional argument!")
+    getout(f'\n `{sys.argv[1]}` is not a valid positional argument!')
     getout(helper())
   else:
     for i in lst_1:
-      if sys.argv[1] == f"{dft}{i}":
-        # if __name__ == "__main__":
-        logger.debug(run(eval(f"{i}Load()")))
+      if sys.argv[1] == f'{dft}{i}':
+        # if __name__ == '__main__':
+        logger.debug(run(eval(f'{i}Load()')))
         break
```

### Comparing `dipense-0.1.1/dipense/default.py` & `dipense-0.1.2/dipense/default.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 
 
 class Default:
   
   @staticmethod
   def default():
     """
-      it is mainly created so that it can be use (access) in any page,
-      for example the year that will show in the footer
-      it is not only for one page it is for all pages in the site
-      
-      so by using this class method we can access it in any page
-      instead of creating `the_year` variable in each view
-      
-      like so the category list in the menu bar also it is not for one page
-      and possibly for other variables ==> [the_year, category, comment, reply, search, message]
-      
-      Also for the notification of new recent comment, reply, search, or message
-      that will show on the menu bar button (in the header)
+    It is mainly created so that it can be use (access) in any page,
+    for example the year that will show in the footer
+    it is not only for one page it is for all pages in the site
+    
+    so by using this class method we can access it in any page
+    instead of creating `the_year` variable in each view
+    
+    like so the category list in the menu bar also it is not for one page
+    and possibly for other variables ==> [the_year, category, comment, reply, search, message]
+    
+    Also for the notification of new recent comment, reply, search, or message
+    that will show on the menu bar button (in the header)
     """
     
     the_year = datetime.utcnow().year
     data = {
-      "the_year": the_year,
+      'the_year': the_year,
     }
     
     return data
 
-  payload = "payload"
-  suffix_payload = ["num", "who", "ip"]
+  payload = 'payload'
+  suffix_payload = ['num', 'who', 'ip']
   sites_list = [
-    "site:facebook.com",
-    "site:twitter.com",
-    "site:instagram.com",
-    "site:tiktok.com",
-    "site:youtube.com",
-    "site:linkedin.com",
-    "site:github.com",
+    'site:facebook.com',
+    'site:twitter.com',
+    'site:instagram.com',
+    'site:tiktok.com',
+    'site:youtube.com',
+    'site:linkedin.com',
+    'site:github.com',
   ]
   
   
 def default():
   """
-    this is the function (shortcut of `Default.default") that we will call in some of our site view
-    instead of calling the `Default.default" which will make our code so large
+  This is the function (shortcut of `Default.default") that we will call in some of our site view
+  instead of calling the `Default.default" which will make our code so large
   """
   return Default.default()
```

### Comparing `dipense-0.1.1/dipense/drone.py` & `dipense-0.1.2/dipense/drone.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 from phonenumbers import carrier
 from phonenumbers import geocoder
 from phonenumbers import timezone
 
 
 def numLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog="scan phone number", description="This scan a phone number!")
+  parser = argparse.ArgumentParser(prog='scan phone number', description='This scan a phone number!')
   
   # metavar make the -help to look cleaan
-  parser.add_argument("--number", "-n", required=True, type=str, metavar="", help="What is the phone number? it should start with country code e.g +2348123456789")
-  parser.add_argument(dest="payloadnum", default="payloadnum", type=str, metavar="", help="The payload is to find phone number infomation")
+  parser.add_argument('--number', '-n', required=True, type=str, metavar='', help='What is the phone number? it should start with country code e.g +2348123456789')
+  parser.add_argument(dest='payloadnum', default='payloadnum', type=str, metavar='', help='The payload is to find phone number infomation')
   
   args = parser.parse_args()
   p_num = args.number
 
   try:
     num_parse = phonenumbers.parse(p_num, None)
     num_valid = phonenumbers.is_valid_number(num_parse)
     p_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.NATIONAL)
     inter_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.INTERNATIONAL)
     p_e164 = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.E164)
-    p_geo = geocoder.description_for_number(num_parse, "en")
-    p_carr = carrier.name_for_number(num_parse, "en")
+    p_geo = geocoder.description_for_number(num_parse, 'en')
+    p_carr = carrier.name_for_number(num_parse, 'en')
     time_zone_1 = timezone.time_zones_for_number(num_parse)
     time_zone_2 = timezone.time_zones_for_geographical_number(num_parse)
     
     """
       >>> p_num = '+2349083513047'
       >>> num_parse = phonenumbers.parse(p_num, None)
       >>> num_parse
@@ -62,24 +62,24 @@
       ('Africa/Lagos',)
       >>> time_zone_2 = timezone.time_zones_for_geographical_number(num_parse)
       >>> time_zone_2
       ('Africa/Lagos',)
     """
 
     context = {
-      "num_parse": num_parse,
-      "num_valid": num_valid,
-      "p_nation": p_nation,
-      "inter_nation": inter_nation,
-      "p_e164": p_e164,
-      "p_geo": p_geo,
-      "p_carr": p_carr,
-      "time_zone_1": time_zone_1,
-      "time_zone_2": time_zone_2,
-      "sites_list": Default.sites_list,
+      'num_parse': num_parse,
+      'num_valid': num_valid,
+      'p_nation': p_nation,
+      'inter_nation': inter_nation,
+      'p_e164': p_e164,
+      'p_geo': p_geo,
+      'p_carr': p_carr,
+      'time_zone_1': time_zone_1,
+      'time_zone_2': time_zone_2,
+      'sites_list': Default.sites_list,
     }
     
     getout(colored(r"""
            _..._
          .'     '.
         /  _   _  \
         | (o)_(o) |
@@ -88,50 +88,50 @@
         //   .   \ \
        ||   .     \ \
        |\   :     / |
        \ `) '   (`  /_
      _)``".____,.'"` (_
      )     )'--'(     (
       '---`      `---`
-""", "cyan", attrs=["blink"]))
+""", 'cyan', attrs=['blink']))
     
-    # q1 = f"{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}""
-    # q2 = q1.replace(" ", "+")
-    # for site in context["sites_list"]:
-    #   # q1 = f"{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}""
-    #   # q2 = q1.replace(" ", "+")
-    #   url_g = "[+] " + f'https://www.google.com/search?q={site}+intext%3A{p_e164}"+OR+intext"{inter_nation}"+OR +ntext:"{p_nation}"'
-    #   getout(colored(url_g, "magenta"))
+    # q1 = f'{site} intext: '{p_e164}' OR intex: '{inter_nation}' OR intex: '{p_nation}''
+    # q2 = q1.replace(' ', '+')
+    # for site in context['sites_list']:
+    #   # q1 = f'{site} intext: '{p_e164}' OR intex: '{inter_nation}' OR intex: '{p_nation}''
+    #   # q2 = q1.replace(' ', '+')
+    #   url_g = '[+] ' + f'https://www.google.com/search?q={site}+intext%3A{p_e164}'+OR+intext'{inter_nation}'+OR +ntext:'{p_nation}''
+    #   getout(colored(url_g, 'magenta'))
     
   except:
     context = {
-      "p_num": p_num,
+      'p_num': p_num,
     }
     
   for k, v in context.items():
-    if k == "sites_list":
+    if k == 'sites_list':
       pass
     else:
-      r = k + ": "
-      getout(colored(" =>", "magenta"), colored(r, "green"), v)
-  # if args.kind == "nmap":
-  #   n_cmd = "nmap -v -A -sV " + args.ip
+      r = k + ': '
+      getout(colored(' =>', 'magenta'), colored(r, 'green'), v)
+  # if args.kind == 'nmap':
+  #   n_cmd = 'nmap -v -A -sV ' + args.ip
   #   n = sp.run(shlex.split(n_cmd))
-  #   getout("This", n.args)
+  #   getout('This', n.args)
   #   return [args, n]
   return args
   
 
 def whoLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog="who is", description="This scan and find info of a domain!")
+  parser = argparse.ArgumentParser(prog='who is', description='This scan and find info of a domain!')
   
   # metavar make the -help to look cleaan
-  parser.add_argument("--domain", "-d", required=True, type=str, metavar="", help="What is the domain name? probably it gives infoof most TLD, while others like ().tk, .io, .org) it capture less")
-  parser.add_argument(dest="payloadwho", default="payloadwho", type=str, metavar="", help="The payload is to find domain name infomation")
+  parser.add_argument('--domain', '-d', required=True, type=str, metavar='', help='What is the domain name? probably it gives infoof most TLD, while others like ().tk, .io, .org) it capture less')
+  parser.add_argument(dest='payloadwho', default='payloadwho', type=str, metavar='', help='The payload is to find domain name infomation')
   
   args = parser.parse_args()
   domain = args.domain
 
   try:
     howis = whois.whois(domain)
     """
@@ -157,57 +157,57 @@
     address = howis.address
     city = howis.city
     state = howis.state
     registrant_postal_code = howis.registrant_postal_code
     country = howis.countr
     
     context = {
-      "howis": howis,
-      "domain": domain,
-      "domain_name": domain_name,
-      "registrar": registrar,
-      "whois_server": whois_server,
-      "referral_url": referral_url,
-      "updated_date": updated_date,
-      "creation_date": creation_date,
-      "expiration_date": expiration_date,
-      "name_servers": name_servers,
-      "status": status,
-      "emails": emails,
-      "dnssec": dnssec,
-      "name": name,
-      "org": org,
-      "address": address,
-      "city": city,
-      "state": state,
-      "registrant_postal_code": registrant_postal_code,
-      "country": country,
+      'howis': howis,
+      'domain': domain,
+      'domain_name': domain_name,
+      'registrar': registrar,
+      'whois_server': whois_server,
+      'referral_url': referral_url,
+      'updated_date': updated_date,
+      'creation_date': creation_date,
+      'expiration_date': expiration_date,
+      'name_servers': name_servers,
+      'status': status,
+      'emails': emails,
+      'dnssec': dnssec,
+      'name': name,
+      'org': org,
+      'address': address,
+      'city': city,
+      'state': state,
+      'registrant_postal_code': registrant_postal_code,
+      'country': country,
     }
   except:
     context = {
-      "domain": domain,
+      'domain': domain,
     }
     
   if domain_name == None:
-    getout(colored(" => ", "cyan"), colored("domain:", "green"), domain)
-    getout(colored(" => ", "cyan", attrs=["blink"]), colored("status:", "green"), colored("unauthorized", "red", attrs=["blink"]))
+    getout(colored(' => ', 'cyan'), colored('domain:', 'green'), domain)
+    getout(colored(' => ', 'cyan', attrs=['blink']), colored('status:', 'green'), colored('unauthorized', 'red', attrs=['blink']))
   else:
     for k, v in context.items():
       # if the value of the result is None the color should be red
       if v == None:
-        r = k + ":"
-        getout(colored(" => ", "cyan"), colored(r, "green"), colored(v, "red", attrs=["blink"]))
+        r = k + ':'
+        getout(colored(' => ', 'cyan'), colored(r, 'green'), colored(v, 'red', attrs=['blink']))
       else:
         # if the key is status, it will print different and do for loof over the result list
-        if k == "status":
-          getout("\n", colored("=> ", "cyan"), colored("status", "yellow"), ":")
+        if k == 'status':
+          getout('\n', colored('=> ', 'cyan'), colored('status', 'yellow'), ':')
           for s in v:
-            getout("\t\t", colored(" --- ", "green"), colored(s, "yellow"))
+            getout('\t\t', colored(' --- ', 'green'), colored(s, 'yellow'))
           getout()
         # else if the key is howis, it will look different
-        elif k == "howis":
-          r = k + ":"
-          getout(colored(" => ", "cyan"), colored(r, "blue"), colored(v, "blue", attrs=["blink"]))
+        elif k == 'howis':
+          r = k + ':'
+          getout(colored(' => ', 'cyan'), colored(r, 'blue'), colored(v, 'blue', attrs=['blink']))
         else:
-          r = k + ":"
-          getout(colored(" => ", "cyan"), colored(r, "green"), v)
+          r = k + ':'
+          getout(colored(' => ', 'cyan'), colored(r, 'green'), v)
   return args
```

### Comparing `dipense-0.1.1/dipense/icheckp.py` & `dipense-0.1.2/dipense/icheckp.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,108 +18,108 @@
       g = geoip.ip(i_num)
       cty = g.city # ip address city
       stt = g.state # ip address state
       ctry = g.country # ip address country
       
       json_raw = g.raw
       time_zone = list(list(json_raw.items())[6])[1] # ip address timezone area
-      d_longitude = list(list(json_raw.items())[4])[1].split(",")[1] # ip address longitude
-      d_latitude = list(list(json_raw.items())[4])[1].split(",")[0] # ip address latitude
+      d_longitude = list(list(json_raw.items())[4])[1].split(',')[1] # ip address longitude
+      d_latitude = list(list(json_raw.items())[4])[1].split(',')[0] # ip address latitude
       d_location = list(list(json_raw.items())[4])[1] # ip address coordinate
       
       location = g.latlng # a list which include latitude and longitude
       
       # creating a base map, making the `min_zoom=0`,
       # overide the `zoom_start=13` from default which is `10` to `13`, and
       # overide the `max_zoom=70` from default which is `18` to `70`
       Tmap = tracer.Map(location=location, max_zoom=70, min_zoom=0, zoom_start=13)
       
       # A circle of a fixed size with radius specified in pixels.
-      tracer.CircleMarker(location=location, radius=50, color="#3186cc", fill=True, fill_color="#3186cc").add_to(Tmap)
-      tracer.Circle(radius=100, location=location, popup="The Waterfront", color="crimson", fill=False).add_to(Tmap)
+      tracer.CircleMarker(location=location, radius=50, color='#3186cc', fill=True, fill_color='#3186cc').add_to(Tmap)
+      tracer.Circle(radius=100, location=location, popup='The Waterfront', color='crimson', fill=False).add_to(Tmap)
       # making the icon to be `cloud`
-      tracer.Marker(location, icon=tracer.Icon(icon="cloud")).add_to(Tmap)
+      tracer.Marker(location, icon=tracer.Icon(icon='cloud')).add_to(Tmap)
       
       self.dir_tree() # make the dir tree
-      sp.run("cd .dipense/maps && sudo touch map.html", shell=True)
+      sp.run('cd .dipense/maps && sudo touch map.html', shell=True)
       cwd = os.getcwd()
 
-      os.chdir(os.path.join(cwd, ".dipense/maps"))
-      os.system("sudo touch test.py")
+      os.chdir(os.path.join(cwd, '.dipense/maps'))
+      os.system('sudo touch test.py')
       
       map_file_method = self.mapName(i_num)
       mapF = map_file_method[0]
       csv_from_mapF = map_file_method[1]
       
-      html_map_file_cmd = "sudo touch {}".format(mapF)
-      csv_map_file_cmd = "sudo touch {}".format(csv_from_mapF)
+      html_map_file_cmd = 'sudo touch {}'.format(mapF)
+      csv_map_file_cmd = 'sudo touch {}'.format(csv_from_mapF)
       
       os.system(html_map_file_cmd)
       os.system(csv_map_file_cmd)
       
       for i in os.listdir():
-        sp.run(["sudo", "chmod", "777", i])
+        sp.run(['sudo', 'chmod', '777', i])
 
       Tmap.save(mapF)
-      cprint(os.getcwd(), "magenta")
+      cprint(os.getcwd(), 'magenta')
       
       dummy = """# this is a test module
 
   # write with focus
   """
 
-      with open("test.py", "w") as f:
+      with open('test.py', 'w') as f:
         f.write(dummy)
-      fieldnames = ["City", "State", "Country", "time_zone", "d_longitude", "d_latitude", "d_location", "location", "Map"]
+      fieldnames = ['City', 'State', 'Country', 'time_zone', 'd_longitude', 'd_latitude', 'd_location', 'location', 'Map']
       
-      with open(csv_from_mapF, "w") as csv_f:
+      with open(csv_from_mapF, 'w') as csv_f:
         csv_writer = csv.writer(csv_f)
         csv_writer.writerow(fieldnames)
         csv_writer.writerow([cty, stt, ctry, time_zone, d_longitude, d_latitude, d_location, location, mapF])
         
-      csv_loc = "csv file is located in " + os.path.realpath(csv_from_mapF)
-      cprint(csv_loc, "green")
-      # cprint(csv_loc, "green", attrs=["bold"])
+      csv_loc = 'csv file is located in ' + os.path.realpath(csv_from_mapF)
+      cprint(csv_loc, 'green')
+      # cprint(csv_loc, 'green', attrs=['bold'])
       
       if self.autoOpenMap:
         import webbrowser
         webbrowser.get().open(os.path.realpath(mapF))
-        openInfo = "Soon to open " + os.path.realpath(mapF)
-        print(colored(openInfo, "magenta", attrs=["reverse", "blink"]))
+        openInfo = 'Soon to open ' + os.path.realpath(mapF)
+        print(colored(openInfo, 'magenta', attrs=['reverse', 'blink']))
         
       context = {
-        "cty": cty,
-        "stt": stt,
-        "ctry": ctry,
-        "json_raw": json_raw,
-        "time_zone": time_zone,
-        "d_longitude": d_longitude,
-        "d_latitude": d_latitude,
-        "d_location": d_location,
-        "location coordinate": location,
+        'cty': cty,
+        'stt': stt,
+        'ctry': ctry,
+        'json_raw': json_raw,
+        'time_zone': time_zone,
+        'd_longitude': d_longitude,
+        'd_latitude': d_latitude,
+        'd_location': d_location,
+        'location coordinate': location,
       }
       
     except:
       context = {
-        "i_num": i_num,
+        'i_num': i_num,
       }
       
     from . import getout
     if g.raw == None:
-      getout(colored(" => ", "cyan"), colored("domain:", "green"), i_num)
-      getout(colored(" => ", "cyan", attrs=["blink"]), colored("status:", "green"), colored("unauthorized", "red", attrs=["blink"]))
+      getout(colored(' => ', 'cyan'), colored('domain:', 'green'), i_num)
+      getout(colored(' => ', 'cyan', attrs=['blink']), colored('status:', 'green'), colored('unauthorized', 'red', attrs=['blink']))
     else:
       for k, v in context.items():
         # if the value of the result is None the color should be red
         if v == None:
-          r = k + ":"
-          getout(colored(" => ", "cyan"), colored(r, "green"), colored(v, "red", attrs=["blink"]))
+          r = k + ':'
+          getout(colored(' => ', 'cyan'), colored(r, 'green'), colored(v, 'red', attrs=['blink']))
         else:
           # if the key is json_raw, it will print different and do for loof over the result list
-          if k == "json_raw":
-            getout("\n", colored("=> ", "cyan"), colored("json_raw", "yellow"), ":")
+          if k == 'json_raw':
+            getout('\n', colored('=> ', 'cyan'), colored('json_raw', 'yellow'), ':')
             for s in v.items():
-              getout("\t\t", colored(" --- ", "green"), colored(s, "yellow"))
+              getout('\t\t', colored(' --- ', 'green'), colored(s, 'yellow'))
             getout()
           else:
-            r = k + ":"
-            getout(colored(" => ", "cyan"), colored(r, "green"), v)
+            r = k + ':'
+            getout(colored(' => ', 'cyan'), colored(r, 'green'), v)
```

### Comparing `dipense-0.1.1/dipense/structure.py` & `dipense-0.1.2/dipense/structure.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,49 +10,49 @@
   """filiing class"""
   def __init__(self, autoOpenMap=False):
     self.autoOpenMap = autoOpenMap
     
 
   def dir_tree(self):
     """create a directory tree where file will reserved"""
-    sp.run(["sudo", "mkdir", "-p", ".dipense/maps"])
+    sp.run(['sudo', 'mkdir', '-p', '.dipense/maps'])
     
 
-  annot = """
+  annot = '''
 This method return a list of two files names
 (html and csv)
-"""
+'''
 
   # def mapName(self, i_num):
   def mapName(self, i_num) -> annot:
     """Filing method of assigning map files names"""
     
     """
-      replacing the dot '.' in an ip address with underscore '_'
-      also replace the spaces ' ' of the ctime with underscore '_', and
-      also the colon ':' is replaced with underscore '_' too!
-      
-      ip address format (e.g): '192.255.255.255'
-      ctime() format (e.g): 'Wed Nov 2 16:28:16 2022'
-      
-      
-      `r1` look like this at the end:
-        192_255_255_255_@_Wed_Nov__2_16:28:16_2022
+    replacing the dot '.' in an ip address with underscore '_'
+    also replace the spaces ' ' of the ctime with underscore '_', and
+    also the colon ':' is replaced with underscore '_' too!
+    
+    ip address format (e.g): '192.255.255.255'
+    ctime() format (e.g): 'Wed Nov 2 16:28:16 2022'
+    
+    
+    `r1` look like this at the end:
+      192_255_255_255_@_Wed_Nov__2_16:28:16_2022
     """
-    r1 = str(i_num.replace(".", "_")) + "_@_" + ctime().replace(" ", "_")
+    r1 = str(i_num.replace('.', '_')) + '_@_' + ctime().replace(' ', '_')
     
     """
       `r2` look like this at the end:
         192_255_255_255_@_Wed_Nov__2_16_28_16_2022
     """
-    r2 = r1.replace(":", "_")
+    r2 = r1.replace(':', '_')
     
     # the map file names (html & csv)
-    map_file_html = "map_" + str(r2) + ".html"
-    map_file_csv = "map_" + str(r2) + ".csv"
+    map_file_html = 'map_' + str(r2) + '.html'
+    map_file_csv = 'map_' + str(r2) + '.csv'
     
     return [map_file_html, map_file_csv]
     
 
 def helper():
   note = r"""
   Type '<module>.py <subcommand> -h' for help on a specific subcommand.
```

### Comparing `dipense-0.1.1/setup.py` & `dipense-0.1.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
-  name = "dipense", # name of the main package (base folder i.e dipense)
-  version = "0.1.1",
-  description = "An OSINT tool for IT ninjas",
-  long_description = open("README.md").read() + "\n\n" + open("CHANGELOG").read(),
-  long_description_content_type="text/markdown",
-  python_requires = ">=3.6",
-  # platforms="any",
+  name = 'dipense', # name of the main package (base folder i.e dipense)
+  version = '0.1.2',
+  description = 'An OSINT tool for IT ninjas',
+  long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
+  long_description_content_type='text/markdown',
+  python_requires = '>=3.7',
+  platforms='any',
   
-  url = "https://dipense.readthedocs.io",
-  repo = "https://github.com/usmanmusa1920/dipense",
-  author = "Usman Musa",
-  author_email = "usmanmusa1920@gmail.com",
-  license = "MIT", # Choose your license, note the American spelling
+  url = 'https://dipense.readthedocs.io',
+  download_url = 'https://pypi.org/project/dipense',
+  author = 'Usman Musa',
+  author_email = 'usmanmusa1920@gmail.com',
+  license = 'MIT', # Choose your license, note the American spelling
   classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3"
+    'Development Status :: 5 - Production/Stable',
+    'Environment :: Web Environment',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Natural Language :: English',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Framework :: Django',
+    'Topic :: Internet',
+    'Topic :: Terminals',
+    'Topic :: Security',
+    'Topic :: Communications :: Email',
+    'Topic :: Software Development :: Libraries :: Python Modules',
   ],
   
   # used when people are searching for a module, keywords separated with a space
-  keywords = "dipense",
+  keywords = 'dipense',
   include_package_data = True, # include files listed in MANIFEST.in
   
   # The list of packages(directories) for your library
-  packages=find_packages(), # OR packages=["dipense"] 
-  # If your package is a single module, use this instead of "packages":
-  # py_modules=[""] # list of files (modules) that are not in any directory (at the root dir)
+  packages=find_packages(), # OR packages=['dipense'] 
+  # If your package is a single module, use this instead of 'packages':
+  # py_modules=[''] # list of files (modules) that are not in any directory (at the root dir)
   # the libraries it depends on
   
   # List of other python modules which this module depends on.  For example RPi.GPIO
   install_requires = [
-    "folium==0.13.0",
-    "phonenumbers==8.13.0",
-    "geocoder==1.38.1",
-    "python-whois==0.8.0",
-    "termcolor==2.1.0",
-    ]
+    'folium==0.13.0',
+    'phonenumbers==8.13.0',
+    'geocoder==1.38.1',
+    'python-whois==0.8.0',
+    'termcolor==2.1.0',
+  ],
+  project_urls={
+    'Documentation': 'https://dipense.readthedocs.io',
+    'Source': 'https://github.com/usmanmusa1920/dipense',
+  },
 )
```

