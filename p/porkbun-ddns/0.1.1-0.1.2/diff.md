# Comparing `tmp/porkbun-ddns-0.1.1.tar.gz` & `tmp/porkbun-ddns-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porkbun-ddns-0.1.1.tar", last modified: Sun Apr 23 15:38:02 2023, max compression
+gzip compressed data, was "porkbun-ddns-0.1.2.tar", last modified: Fri Jun 23 13:01:00 2023, max compression
```

## Comparing `porkbun-ddns-0.1.1.tar` & `porkbun-ddns-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:02.552121 porkbun-ddns-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 15:38:02.552121 porkbun-ddns-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:02.552121 porkbun-ddns-0.1.1/porkbun_ddns/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/porkbun_ddns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/porkbun_ddns/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/porkbun_ddns/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/porkbun_ddns/porkbun_ddns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:38:02.552121 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 15:38:02.000000 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-23 15:38:02.000000 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:38:02.000000 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 15:38:02.000000 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 15:38:02.000000 porkbun-ddns-0.1.1/porkbun_ddns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 15:38:02.552121 porkbun-ddns-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-23 15:37:51.000000 porkbun-ddns-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/porkbun_ddns/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/porkbun_ddns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/setup.py
```

### Comparing `porkbun-ddns-0.1.1/LICENSE` & `porkbun-ddns-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.1/PKG-INFO` & `porkbun-ddns-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.1
+Version: 0.1.2
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 `porkbun-ddns` is a unofficial DDNS-Client for Porkbun Domains.
 This library will only update the records if the IP(s) have changed or the dns entry didn't exist before, it will also set/update A (IPv4) and AAAA (IPv6) records.
 
 
 Since [porkbun-dynamic-dns-python](https://github.com/porkbundomains/porkbun-dynamic-dns-python) is deprecate and [ddclient](https://github.com/ddclient/ddclient/issues/528) has no more active maintainers, I took it into my own hands to code a decent DDNS Client for Porkbun.
 Inspired by [con-f-use](https://github.com/con-f-use) [pull request](https://github.com/porkbundomains/porkbun-dynamic-dns-python/pull/6), I built a pip Package and a docker container.
 
-I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun).
+I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun) or as alternative use my [lego-certbot](https://github.com/mietzen/lego-certbot) image.
 
 # CLI
 
 ## Install via pip
 
 ```shell
 pip install porkbun-ddns
@@ -91,14 +91,15 @@
       SECRETAPIKEY: "<YOUR-SECRETAPIKEY>" # Your Porkbun Secret-API-Key
       APIKEY: "<YOUR-APIKEY>" # Your Porkbun API-Key
       # PUBLIC_IPS: "1.2.3.4,2001:043e::1" # Set if you got static IP's
       # FRITZBOX: "192.168.178.1" # Use Fritz!BOX to obtain Public IP's
       # SLEEP: "300" # Seconds to sleep between DynDNS runs
       # IPV4_ONLY: "FALSE" # Only set IPv4 address
       # IPV6_ONLY: "FALSE" # Only set IPv6 address
+      PYTHONUNBUFFERED: 1 # sent stdout and stderr straight to the terminal
     restart: unless-stopped
 ```
 
 # Python
 
 ```python
 from porkbun_ddns import PorkbunDDNS
```

### Comparing `porkbun-ddns-0.1.1/README.md` & `porkbun-ddns-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 `porkbun-ddns` is a unofficial DDNS-Client for Porkbun Domains.
 This library will only update the records if the IP(s) have changed or the dns entry didn't exist before, it will also set/update A (IPv4) and AAAA (IPv6) records.
 
 
 Since [porkbun-dynamic-dns-python](https://github.com/porkbundomains/porkbun-dynamic-dns-python) is deprecate and [ddclient](https://github.com/ddclient/ddclient/issues/528) has no more active maintainers, I took it into my own hands to code a decent DDNS Client for Porkbun.
 Inspired by [con-f-use](https://github.com/con-f-use) [pull request](https://github.com/porkbundomains/porkbun-dynamic-dns-python/pull/6), I built a pip Package and a docker container.
 
-I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun).
+I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun) or as alternative use my [lego-certbot](https://github.com/mietzen/lego-certbot) image.
 
 # CLI
 
 ## Install via pip
 
 ```shell
 pip install porkbun-ddns
@@ -75,14 +75,15 @@
       SECRETAPIKEY: "<YOUR-SECRETAPIKEY>" # Your Porkbun Secret-API-Key
       APIKEY: "<YOUR-APIKEY>" # Your Porkbun API-Key
       # PUBLIC_IPS: "1.2.3.4,2001:043e::1" # Set if you got static IP's
       # FRITZBOX: "192.168.178.1" # Use Fritz!BOX to obtain Public IP's
       # SLEEP: "300" # Seconds to sleep between DynDNS runs
       # IPV4_ONLY: "FALSE" # Only set IPv4 address
       # IPV6_ONLY: "FALSE" # Only set IPv6 address
+      PYTHONUNBUFFERED: 1 # sent stdout and stderr straight to the terminal
     restart: unless-stopped
 ```
 
 # Python
 
 ```python
 from porkbun_ddns import PorkbunDDNS
```

### Comparing `porkbun-ddns-0.1.1/porkbun_ddns/cli.py` & `porkbun-ddns-0.1.2/porkbun_ddns/cli.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.1/porkbun_ddns/helpers.py` & `porkbun-ddns-0.1.2/porkbun_ddns/helpers.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.1/porkbun_ddns/porkbun_ddns.py` & `porkbun-ddns-0.1.2/porkbun_ddns/porkbun_ddns.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
         if isinstance(config, dict):
             self.config = config
         else:
             self._load_config(config)
         self._check_config()
         self.static_ips = public_ips
         self.domain = domain.lower()
-        self.records = self.get_records()
+        self.records = None
         self.fritzbox_ip = fritzbox_ip
         self.ipv4 = ipv4
         self.ipv6 = ipv6
+        self.fqdn = self.domain
+        self.subdomain = '@'
 
     def _load_config(self, config: str) -> None:
         """Load a JSON configuration file.
         """
         with open(config) as fid:
             self.config = json.load(fid)
 
@@ -47,15 +49,16 @@
             raise PorkbunDDNS_Error("all of the following are required in '{}': {}".format(
                 self.config, required_keys))
         if 'endpoint' not in self.config.keys():
             self.config["endpoint"] = "https://porkbun.com/api/json/v3"
 
     def set_subdomain(self, subdomain: str) -> None:
         self.subdomain = subdomain.lower()
-        self.fqdn = '.'.join([self.subdomain, self.domain])
+        if self.subdomain != '@':
+            self.fqdn = '.'.join([self.subdomain, self.domain])
 
     def get_public_ips(self) -> list:
         """Retrieve the public IP addresses of the network.
         """
         if self.static_ips:
             public_ips = self.static_ips
         else:
@@ -104,14 +107,15 @@
                 'Make sure you specified the correct domain ({}),\n'.format(self.domain) +
                 'and that API access has been enabled for this domain.'
             )
 
     def update_records(self):
         """Update DNS records for the specified domain.
         """
+        self.records = self.get_records()
         domain_names = [x['name'] for x in self.records if x['type']
                         in ["A", "AAAA", "ALIAS", "CNAME"]]
         for ip in self.get_public_ips():
             record_type = "A" if ip.version == 4 else "AAAA"
             if self.fqdn in domain_names:
                 for i in self.records:
                     if i["name"] == self.fqdn:
```

### Comparing `porkbun-ddns-0.1.1/porkbun_ddns.egg-info/PKG-INFO` & `porkbun-ddns-0.1.2/porkbun_ddns.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.1
+Version: 0.1.2
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 `porkbun-ddns` is a unofficial DDNS-Client for Porkbun Domains.
 This library will only update the records if the IP(s) have changed or the dns entry didn't exist before, it will also set/update A (IPv4) and AAAA (IPv6) records.
 
 
 Since [porkbun-dynamic-dns-python](https://github.com/porkbundomains/porkbun-dynamic-dns-python) is deprecate and [ddclient](https://github.com/ddclient/ddclient/issues/528) has no more active maintainers, I took it into my own hands to code a decent DDNS Client for Porkbun.
 Inspired by [con-f-use](https://github.com/con-f-use) [pull request](https://github.com/porkbundomains/porkbun-dynamic-dns-python/pull/6), I built a pip Package and a docker container.
 
-I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun).
+I also containerized [cert-bun](https://github.com/mietzen/docker-cert-bun) or as alternative use my [lego-certbot](https://github.com/mietzen/lego-certbot) image.
 
 # CLI
 
 ## Install via pip
 
 ```shell
 pip install porkbun-ddns
@@ -91,14 +91,15 @@
       SECRETAPIKEY: "<YOUR-SECRETAPIKEY>" # Your Porkbun Secret-API-Key
       APIKEY: "<YOUR-APIKEY>" # Your Porkbun API-Key
       # PUBLIC_IPS: "1.2.3.4,2001:043e::1" # Set if you got static IP's
       # FRITZBOX: "192.168.178.1" # Use Fritz!BOX to obtain Public IP's
       # SLEEP: "300" # Seconds to sleep between DynDNS runs
       # IPV4_ONLY: "FALSE" # Only set IPv4 address
       # IPV6_ONLY: "FALSE" # Only set IPv6 address
+      PYTHONUNBUFFERED: 1 # sent stdout and stderr straight to the terminal
     restart: unless-stopped
 ```
 
 # Python
 
 ```python
 from porkbun_ddns import PorkbunDDNS
```

### Comparing `porkbun-ddns-0.1.1/setup.py` & `porkbun-ddns-0.1.2/setup.py`

 * *Files identical despite different names*

