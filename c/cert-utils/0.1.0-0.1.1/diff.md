# Comparing `tmp/cert_utils-0.1.0.tar.gz` & `tmp/cert_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cert_utils-0.1.0.tar", last modified: Thu Jun 22 16:29:28 2023, max compression
+gzip compressed data, was "cert_utils-0.1.1.tar", last modified: Fri Jun 23 04:05:08 2023, max compression
```

## Comparing `cert_utils-0.1.0.tar` & `cert_utils-0.1.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/
--rw-r--r--   0 jvanasco   (501) admin       (80)       54 2023-06-21 17:59:34.000000 cert_utils-0.1.0/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-20 21:57:25.000000 cert_utils-0.1.0/pyproject.toml
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2020-06-17 23:12:11.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/info.txt
--rw-------   0 jvanasco   (501) admin       (80)      887 2020-06-17 16:21:06.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      643 2020-06-17 23:12:44.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/csr.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2020-06-17 16:22:44.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2020-06-16 21:30:21.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      538 2020-06-16 22:23:01.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/csr.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2020-06-16 22:28:05.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2020-06-19 18:23:40.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2020-06-16 21:30:51.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2020-06-16 22:06:46.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      566 2020-06-16 21:30:57.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/csr.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2020-06-16 22:31:56.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2020-06-19 18:23:47.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2020-06-16 21:44:45.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2020-06-16 22:07:02.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      631 2020-06-16 21:44:45.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/csr.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/_support/
--rw-r--r--   0 jvanasco   (501) admin       (80)      913 2020-06-17 16:25:36.000000 cert_utils-0.1.0/tests/test_data/unit_tests/_support/info.txt
--rw-------   0 jvanasco   (501) admin       (80)     3247 2020-06-16 21:55:08.000000 cert_utils-0.1.0/tests/test_data/unit_tests/_support/account.key
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/
--rw-------   0 jvanasco   (501) admin       (80)     1675 2020-06-18 19:17:48.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/private_key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       86 2020-06-18 19:04:36.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/regr.json
--r--------   0 jvanasco   (501) admin       (80)     1632 2020-06-18 19:04:36.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/private_key.json
--rw-r--r--   0 jvanasco   (501) admin       (80)      212 2020-06-18 19:06:52.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/info.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       70 2020-06-18 19:07:14.000000 cert_utils-0.1.0/tests/test_data/unit_tests/account_001/meta.json
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-16 20:20:50.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/chain.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2020-06-17 21:33:21.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/info.txt
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2020-06-16 20:20:50.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/cert.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2021-11-23 16:58:36.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/test.py
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-16 20:20:50.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/privkey.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2020-06-16 20:20:50.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2020-06-16 20:20:39.000000 cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/csr.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/long_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/
--rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2021-11-24 18:11:53.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/_demo.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       76 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/_data.json
--rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2021-02-19 23:29:54.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_0_bad.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      573 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/__README__.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_0.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       46 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/long_chains/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/key_technology-ec/
--rw-r--r--   0 jvanasco   (501) admin       (80)      452 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-ec/ec384-1.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-ec/ec384-2-key.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      288 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-ec/ec384-1-key.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:28.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:31:18.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:34:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:34.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:34:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:28.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:34.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:38.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:38.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2020-06-12 15:31:18.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:34:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:34.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert3.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:38.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/privkey5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:28.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/cert2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:31:18.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:31:18.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain6.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:38.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain4.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain5.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:34:40.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain1.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:28.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain2.pem
--rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:34.000000 cert_utils-0.1.0/tests/test_data/pebble-certs/chain3.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/cert.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/privkey.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/fullchain.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/2/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-08-06 21:11:59.000000 cert_utils-0.1.0/tests/test_data/alternate_chains/1/__README__.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/__README__.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_4.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_5.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_2.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_1.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_3.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)      891 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.key
--rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2020-05-05 20:59:50.000000 cert_utils-0.1.0/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    47297 2023-06-21 21:58:15.000000 cert_utils-0.1.0/tests/test_unit.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-21 18:13:00.000000 cert_utils-0.1.0/tests/_utils.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     2134 2023-06-22 16:29:28.000000 cert_utils-0.1.0/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-22 16:28:28.000000 cert_utils-0.1.0/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     2694 2023-06-22 15:30:06.000000 cert_utils-0.1.0/setup.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1091 2023-06-21 22:54:18.000000 cert_utils-0.1.0/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-20 21:58:09.000000 cert_utils-0.1.0/tox.ini
--rw-r--r--   0 jvanasco   (501) admin       (80)      352 2023-06-22 16:29:28.000000 cert_utils-0.1.0/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-21 17:59:50.000000 cert_utils-0.1.0/MANIFEST.in
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils/
--rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-06-21 17:29:10.000000 cert_utils-0.1.0/src/cert_utils/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)   122523 2023-06-21 22:50:15.000000 cert_utils-0.1.0/src/cert_utils/core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1572 2023-06-21 19:51:46.000000 cert_utils-0.1.0/src/cert_utils/model.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3441 2023-06-21 18:19:24.000000 cert_utils-0.1.0/src/cert_utils/utils.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    16336 2023-06-21 21:15:28.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt_info.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-20 21:40:08.000000 cert_utils-0.1.0/src/cert_utils/py.typed
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
--rw-r--r--   0 jvanasco   (501) admin       (80)      893 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
--rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      790 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2021-11-24 18:11:52.000000 cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
--rw-r--r--   0 jvanasco   (501) admin       (80)      334 2023-06-20 22:15:06.000000 cert_utils-0.1.0/src/cert_utils/errors.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-22 01:44:16.000000 cert_utils-0.1.0/src/cert_utils.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     2134 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/top_level.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-22 16:29:28.000000 cert_utils-0.1.0/src/cert_utils.egg-info/dependency_links.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:08.013011 cert_utils-0.1.1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      377 2023-06-23 04:04:29.000000 cert_utils-0.1.1/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)    12231 2023-06-22 16:32:02.000000 cert_utils-0.1.1/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      191 2023-06-21 17:59:50.000000 cert_utils-0.1.1/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2761 2023-06-23 04:05:08.013333 cert_utils-0.1.1/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1931 2023-06-23 04:04:29.000000 cert_utils-0.1.1/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-20 21:57:25.000000 cert_utils-0.1.1/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      403 2023-06-23 04:05:08.014953 cert_utils-0.1.1/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2801 2023-06-23 04:04:29.000000 cert_utils-0.1.1/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:06.928185 cert_utils-0.1.1/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.068764 cert_utils-0.1.1/src/cert_utils/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      145 2023-06-23 04:04:29.000000 cert_utils-0.1.1/src/cert_utils/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)   126129 2023-06-23 04:04:29.000000 cert_utils-0.1.1/src/cert_utils/core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      334 2023-06-20 22:15:06.000000 cert_utils-0.1.1/src/cert_utils/errors.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.241098 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1680 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1797 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/fakelerootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1696 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1955 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1578 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      790 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1939 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrgrootx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1391 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1021 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1586 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1826 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1647 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2013 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1984 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      893 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2021-11-24 18:11:52.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16333 2023-06-23 04:04:29.000000 cert_utils-0.1.1/src/cert_utils/letsencrypt_info.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1597 2023-06-23 04:04:29.000000 cert_utils-0.1.1/src/cert_utils/model.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-20 21:40:08.000000 cert_utils-0.1.1/src/cert_utils/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3441 2023-06-21 18:19:24.000000 cert_utils-0.1.1/src/cert_utils/utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.122235 cert_utils-0.1.1/src/cert_utils.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2761 2023-06-23 04:05:06.000000 cert_utils-0.1.1/src/cert_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7615 2023-06-23 04:05:06.000000 cert_utils-0.1.1/src/cert_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-23 04:05:06.000000 cert_utils-0.1.1/src/cert_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-22 01:44:16.000000 cert_utils-0.1.1/src/cert_utils.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      200 2023-06-23 04:05:06.000000 cert_utils-0.1.1/src/cert_utils.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       11 2023-06-23 04:05:06.000000 cert_utils-0.1.1/src/cert_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.247428 cert_utils-0.1.1/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2020-05-05 20:59:50.000000 cert_utils-0.1.1/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7702 2023-06-21 18:13:00.000000 cert_utils-0.1.1/tests/_utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.249091 cert_utils-0.1.1/tests/test_data/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3303 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:06.931375 cert_utils-0.1.1/tests/test_data/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.273653 cert_utils-0.1.1/tests/test_data/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:06.932621 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.277612 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.280491 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/2/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1570 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1208 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2779 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/fullchain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3272 2020-08-06 21:11:59.000000 cert_utils-0.1.1/tests/test_data/alternate_chains/1/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.286424 cert_utils-0.1.1/tests/test_data/key_technology-ec/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-ec/ec384-1-key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      452 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-ec/ec384-1.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      288 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-ec/ec384-2-key.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.660705 cert_utils-0.1.1/tests/test_data/key_technology-rsa/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1671 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1679 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_1.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_2.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_3.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3243 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_4.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3247 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_5.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      664 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.crt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      558 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.csr
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.key
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.662461 cert_utils-0.1.1/tests/test_data/long_chains/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.685796 cert_utils-0.1.1/tests/test_data/long_chains/TestA/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      573 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/__README__.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       76 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/_data.json
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2683 2021-11-24 18:11:53.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/_demo.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1574 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3664 2021-02-19 23:29:54.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_0_bad.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3665 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_0.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_1.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1151 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_2.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       46 2021-03-19 21:28:12.000000 cert_utils-0.1.1/tests/test_data/long_chains/__README__.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.816790 cert_utils-0.1.1/tests/test_data/pebble-certs/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:34:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:28.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:34.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:38.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:32:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1574 2020-06-12 15:31:18.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/cert6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:34:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:28.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:34.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:38.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:32:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-12 15:31:18.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/chain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:34:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:28.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:34.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:38.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:32:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2783 2020-06-12 15:31:18.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain6.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:34:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey1.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:28.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey2.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:34.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey3.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:38.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey4.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-12 15:32:40.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey5.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3247 2020-06-12 15:31:18.000000 cert_utils-0.1.1/tests/test_data/pebble-certs/privkey6.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:06.944339 cert_utils-0.1.1/tests/test_data/unit_tests/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.821513 cert_utils-0.1.1/tests/test_data/unit_tests/_support/
+-rw-------   0 jvanasco   (501) admin       (80)     3247 2020-06-16 21:55:08.000000 cert_utils-0.1.1/tests/test_data/unit_tests/_support/account.key
+-rw-r--r--   0 jvanasco   (501) admin       (80)      913 2020-06-17 16:25:36.000000 cert_utils-0.1.1/tests/test_data/unit_tests/_support/info.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.852596 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      212 2020-06-18 19:06:52.000000 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       70 2020-06-18 19:07:14.000000 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/meta.json
+-r--------   0 jvanasco   (501) admin       (80)     1632 2020-06-18 19:04:36.000000 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/private_key.json
+-rw-------   0 jvanasco   (501) admin       (80)     1675 2020-06-18 19:17:48.000000 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/private_key.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)       86 2020-06-18 19:04:36.000000 cert_utils-0.1.1/tests/test_data/unit_tests/account_001/regr.json
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.933131 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1635 2020-06-16 20:20:50.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/cert.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1208 2020-06-16 20:20:50.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/chain.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1674 2020-06-16 20:20:39.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     2844 2020-06-16 20:20:50.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      387 2020-06-17 21:33:21.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/info.txt
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     3243 2020-06-16 20:20:50.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/privkey.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1516 2021-11-23 16:58:36.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/test.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.939292 cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      538 2020-06-16 22:23:01.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      889 2020-06-17 16:22:44.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2020-06-16 21:30:21.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.953640 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1042 2020-06-19 18:23:40.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      566 2020-06-16 21:30:57.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2250 2020-06-16 22:06:46.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      569 2020-06-16 22:28:05.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      891 2020-06-16 21:30:51.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:07.969195 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1111 2020-06-19 18:23:47.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/cert.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)      631 2020-06-16 21:44:45.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/csr.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2319 2020-06-16 22:07:02.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/fullchain.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      751 2020-06-16 22:31:56.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/info.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      887 2020-06-16 21:44:45.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/privkey.pem
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-23 04:05:08.011767 cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      643 2020-06-17 23:12:44.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/csr.pem
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)     1146 2020-06-17 23:12:11.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/info.txt
+-rw-------   0 jvanasco   (501) admin       (80)      887 2020-06-17 16:21:06.000000 cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/privkey.pem
+-rw-r--r--   0 jvanasco   (501) admin       (80)    73620 2023-06-23 04:04:29.000000 cert_utils-0.1.1/tests/test_unit.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-20 21:58:09.000000 cert_utils-0.1.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/info.txt` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/privkey.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_005/csr.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_005/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/info.txt` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/privkey.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_002/csr.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_002/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/info.txt` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/cert.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/privkey.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_003/csr.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_003/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/info.txt` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/cert.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/privkey.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_004/csr.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_004/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/_support/info.txt` & `cert_utils-0.1.1/tests/test_data/unit_tests/_support/info.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/_support/account.key` & `cert_utils-0.1.1/tests/test_data/unit_tests/_support/account.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/account_001/private_key.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/account_001/private_key.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/account_001/private_key.json` & `cert_utils-0.1.1/tests/test_data/unit_tests/account_001/private_key.json`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/chain.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/cert.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/test.py` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/test.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/privkey.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/unit_tests/cert_001/csr.pem` & `cert_utils-0.1.1/tests/test_data/unit_tests/cert_001/csr.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/_demo.py` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/_demo.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/cert.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_0_bad.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_0_bad.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_0.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_2.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_1.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/__README__.txt` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_1.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/root_2.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/root_2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/long_chains/TestA/chain_0.pem` & `cert_utils-0.1.1/tests/test_data/long_chains/TestA/chain_0.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain2.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert6.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey1.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain3.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain1.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert5.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey2.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey3.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert4.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain4.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey6.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert1.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain5.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert3.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey4.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/privkey5.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/privkey5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/cert2.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/cert2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/fullchain6.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/fullchain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain6.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain4.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain5.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain1.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain2.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/pebble-certs/chain3.pem` & `cert_utils-0.1.1/tests/test_data/pebble-certs/chain6.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/chain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/cert.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/cert.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/privkey.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/privkey.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/1/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/1/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/2/chain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem` & `cert_utils-0.1.1/tests/test_data/alternate_chains/1/alternate_chains/2/fullchain.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/__README__.txt` & `cert_utils-0.1.1/tests/test_data/__README__.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.crt` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.csr` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.crt` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-single_certificate.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_5.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_4.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_4.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_4.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.crt` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_5.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_5.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_1.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.csr` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_3.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_2.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_2.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_2.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/acme_account_1.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/acme_account_1.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/private_3.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/private_3.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_5-server.crt` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_5-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_weekly.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-global_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.csr` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_4-server.csr` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_4-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-cycle-account_daily.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_3-server.key` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_3-server.key`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-5.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_1-server.csr` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_1-server.csr`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/AcmeAccountKey-4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_data/key_technology-rsa/selfsigned_2-server.crt` & `cert_utils-0.1.1/tests/test_data/key_technology-rsa/selfsigned_2-server.crt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/tests/test_unit.py` & `cert_utils-0.1.1/tests/test_unit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # stdlib
-import logging
 import json
+import logging
+import os
 import test
 import test.test_httplib
 import unittest
 
 # pypi
 from acme import crypto_util as acme_crypto_util
 from certbot import crypto_util as certbot_crypto_util
 import cryptography
-from cryptography.hazmat.primitives import serialization as cryptography_serialization
+from cryptography.hazmat.primitives import serialization as crypto_serialization
 import josepy
 from OpenSSL import crypto as openssl_crypto
 
 # local
 import cert_utils
 from cert_utils import core
 from cert_utils import model
@@ -23,46 +24,115 @@
 from ._utils import CERT_CA_SETS
 from ._utils import CSR_SETS
 from ._utils import KEY_SETS
 from ._utils import TEST_FILES
 
 # ==============================================================================
 
-log = logging.getLogger(__name__)
-log.setLevel(logging.INFO)
+EXTENDED_TESTS = bool(int(os.getenv("CERT_UTILS_EXTENDED_TESTS", "0")))
 
 # ------------------------------------------------------------------------------
 
+# these mixins are used to simulate behavior as if we are missing libraries
+
+
+class _Mixin_fallback_possible(object):
+    _fallback = False
+    _fallback_global = False
+
+
+class _MixinNoCrypto(_Mixin_fallback_possible):
+    _fallback = True
+    _fallback_global = True
 
-class _MixinNoCrypto(object):
     def setUp(self):
         # print("_MixinNoCrypto.setUp")
         global cert_utils
-        global cryptography
         cert_utils.core.acme_crypto_util = None
-        cert_utils.core.openssl_crypto = None
         cert_utils.core.certbot_crypto_util = None
-        # cert_utils.core.crypto_util_asn1 = None
-        cert_utils.core.josepy = None
-        cert_utils.core.cryptography_serialization = None
         cert_utils.core.cryptography = None
+        cert_utils.core.crypto_serialization = None
+        cert_utils.core.josepy = None
+        cert_utils.core.openssl_crypto = None
 
     def tearDown(self):
         # print("_MixinNoCrypto.tearDown")
         global cert_utils
         cert_utils.core.acme_crypto_util = acme_crypto_util
-        cert_utils.core.openssl_crypto = openssl_crypto
         cert_utils.core.certbot_crypto_util = certbot_crypto_util
-        # cert_utils.core.crypto_util_asn1 = crypto_util_asn1
+        cert_utils.core.cryptography = cryptography
+        cert_utils.core.crypto_serialization = crypto_serialization
         cert_utils.core.josepy = josepy
-        cert_utils.core.cryptography_serialization = cryptography_serialization
+        cert_utils.core.openssl_crypto = openssl_crypto
+
+
+class _Mixin_Missing_acme(_Mixin_fallback_possible):
+    _fallback = True
+
+    def setUp(self):
+        global cert_utils
+        cert_utils.core.acme_crypto_util = None
+
+    def tearDown(self):
+        global cert_utils
+        cert_utils.core.acme_crypto_util = acme_crypto_util
+
+
+class _Mixin_Missing_certbot(_Mixin_fallback_possible):
+    _fallback = True
+
+    def setUp(self):
+        global cert_utils
+        cert_utils.core.certbot_crypto_util = None
+
+    def tearDown(self):
+        global cert_utils
+        cert_utils.core.certbot_crypto_util = certbot_crypto_util
+
+
+class _Mixin_Missing_cryptography(_Mixin_fallback_possible):
+    _fallback = True
+
+    def setUp(self):
+        global cert_utils
+        cert_utils.core.cryptography = None
+
+    def tearDown(self):
+        global cert_utils
         cert_utils.core.cryptography = cryptography
 
 
-class UnitTest_CertUtils(unittest.TestCase, _Mixin_filedata):
+class _Mixin_Missing_josepy(_Mixin_fallback_possible):
+    _fallback = True
+
+    def setUp(self):
+        global cert_utils
+        cert_utils.core.josepy = None
+
+    def tearDown(self):
+        global cert_utils
+        cert_utils.core.josepy = josepy
+
+
+class _Mixin_Missing_openssl_crypto(_Mixin_fallback_possible):
+    _fallback = True
+
+    def setUp(self):
+        global cert_utils
+        cert_utils.core.openssl_crypto = None
+
+    def tearDown(self):
+        global cert_utils
+        cert_utils.core.openssl_crypto = openssl_crypto
+
+
+# ------------------------------------------------------------------------------
+
+
+class UnitTest_CertUtils(unittest.TestCase, _Mixin_fallback_possible, _Mixin_filedata):
     """python -m unittest tests.test_unit.UnitTest_CertUtils"""
 
     _account_sets = {
         "001": {
             "letsencrypt": True,
             "pem": True,
             "signature.input": "example.sample",
@@ -251,51 +321,74 @@
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
-            cert_domains = cert_utils.parse_cert__domains(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
-            self.assertEqual(
-                cert_domains, self._cert_sets[cert_set]["cert.domains.all"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                cert_domains = cert_utils.parse_cert__domains(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                self.assertEqual(
+                    cert_domains, self._cert_sets[cert_set]["cert.domains.all"]
+                )
+                if self._fallback_global or (not cert_utils.core.certbot_crypto_util):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_cert__domains > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_cert__domains > openssl fallback",
+                        logged.output,
+                    )
 
     def test__fingerprint_cert(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__fingerprint_cert
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
 
             # defaults to sha1
-            _fingerprint = cert_utils.fingerprint_cert(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
-            self.assertEqual(
-                _fingerprint, self._cert_sets[cert_set]["cert.fingerprints"]["sha1"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                _fingerprint = cert_utils.fingerprint_cert(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                self.assertEqual(
+                    _fingerprint, self._cert_sets[cert_set]["cert.fingerprints"]["sha1"]
+                )
+                if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.fingerprint_cert > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.fingerprint_cert > openssl fallback",
+                        logged.output,
+                    )
 
             # test the supported
             for _alg in ("sha1", "sha256", "md5"):
                 _fingerprint = cert_utils.fingerprint_cert(
                     cert_pem=cert_pem,
                     cert_pem_filepath=cert_pem_filepath,
                     algorithm=_alg,
                 )
                 self.assertEqual(
                     _fingerprint, self._cert_sets[cert_set]["cert.fingerprints"][_alg]
                 )
+                # no need to test the fallback behavior again
 
             # test unsupported
             with self.assertRaises(ValueError) as cm:
                 _fingerprint = cert_utils.fingerprint_cert(
                     cert_pem=cert_pem,
                     cert_pem_filepath=cert_pem_filepath,
                     algorithm="fake",
@@ -309,196 +402,361 @@
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__parse_csr_domains
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             csr_filename = "unit_tests/cert_%s/csr.pem" % cert_set
             csr_pem_filepath = self._filepath_testfile(csr_filename)
             csr_pem = self._filedata_testfile(csr_filename)
-            csr_domains = cert_utils.parse_csr_domains(
-                csr_pem=csr_pem,
-                csr_pem_filepath=csr_pem_filepath,
-                submitted_domain_names=self._cert_sets[cert_set]["csr.domains.all"],
-            )
-            self.assertEqual(csr_domains, self._cert_sets[cert_set]["csr.domains.all"])
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                csr_domains = cert_utils.parse_csr_domains(
+                    csr_pem=csr_pem,
+                    csr_pem_filepath=csr_pem_filepath,
+                    submitted_domain_names=self._cert_sets[cert_set]["csr.domains.all"],
+                )
+                self.assertEqual(
+                    csr_domains, self._cert_sets[cert_set]["csr.domains.all"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.certbot_crypto_util)
+                    or (not cert_utils.core.openssl_crypto)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_csr_domains > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_csr_domains > openssl fallback",
+                        logged.output,
+                    )
 
     def test__validate_csr(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__validate_csr
         """
-
         for cert_set in sorted(self._cert_sets.keys()):
             csr_filename = "unit_tests/cert_%s/csr.pem" % cert_set
             csr_pem_filepath = self._filepath_testfile(csr_filename)
             csr_pem = self._filedata_testfile(csr_filename)
-            cert_utils.validate_csr(csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath)
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                cert_utils.validate_csr(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
+                )
+                if self._fallback_global or (not cert_utils.core.certbot_crypto_util):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.validate_csr > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.validate_csr > openssl fallback",
+                        logged.output,
+                    )
 
     def test__validate_key(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__validate_key
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             key_filename = "unit_tests/cert_%s/privkey.pem" % cert_set
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
-            key_technology = cert_utils.validate_key(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                key_technology = cert_utils.validate_key(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.crypto_serialization)
+                    or (not cert_utils.core.crypto_rsa)
+                    or (not cert_utils.core.crypto_ec)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.validate_key > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.validate_key > openssl fallback",
+                        logged.output,
+                    )
 
         for key_filename in sorted(KEY_SETS.keys()):
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
-            key_technology = cert_utils.validate_key(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            self.assertEqual(key_technology, KEY_SETS[key_filename]["key_technology"])
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                key_technology = cert_utils.validate_key(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                self.assertEqual(
+                    key_technology, KEY_SETS[key_filename]["key_technology"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.crypto_serialization)
+                    or (not cert_utils.core.crypto_rsa)
+                    or (not cert_utils.core.crypto_ec)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.validate_key > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.validate_key > openssl fallback",
+                        logged.output,
+                    )
 
     def test__validate_cert(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__validate_cert
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
-            cert_utils.validate_cert(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                cert_utils.validate_cert(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.validate_cert > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.validate_cert > openssl fallback",
+                        logged.output,
+                    )
 
     def test__make_csr(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__make_csr
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             key_filename = "unit_tests/cert_%s/privkey.pem" % cert_set
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
-            csr_pem = cert_utils.make_csr(
-                domain_names=self._cert_sets[cert_set]["csr.domains.all"],
-                key_pem=key_pem,
-                key_pem_filepath=key_pem_filepath,
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                csr_pem = cert_utils.make_csr(
+                    domain_names=self._cert_sets[cert_set]["csr.domains.all"],
+                    key_pem=key_pem,
+                    key_pem_filepath=key_pem_filepath,
+                )
+                if self._fallback_global or (not cert_utils.core.acme_crypto_util):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.make_csr > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.make_csr > openssl fallback",
+                        logged.output,
+                    )
 
     def test__modulus_md5_key(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__modulus_md5_key
         """
         for cert_set in sorted(self._cert_sets.keys()):
             key_filename = "unit_tests/cert_%s/privkey.pem" % cert_set
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
-            modulus_md5 = cert_utils.modulus_md5_key(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            self.assertEqual(
-                modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                modulus_md5 = cert_utils.modulus_md5_key(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                self.assertEqual(
+                    modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_key > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_key > openssl fallback",
+                        logged.output,
+                    )
 
         for key_filename in sorted(KEY_SETS.keys()):
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
             modulus_md5 = cert_utils.modulus_md5_key(
                 key_pem=key_pem, key_pem_filepath=key_pem_filepath
             )
             self.assertEqual(modulus_md5, KEY_SETS[key_filename]["modulus_md5"])
+            # no need to test for fallback behavior again
 
     def test__modulus_md5_csr(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__modulus_md5_csr
         """
         for cert_set in sorted(self._cert_sets.keys()):
             csr_filename = "unit_tests/cert_%s/csr.pem" % cert_set
             csr_pem_filepath = self._filepath_testfile(csr_filename)
             csr_pem = self._filedata_testfile(csr_filename)
-            modulus_md5 = cert_utils.modulus_md5_csr(
-                csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
-            )
-            self.assertEqual(
-                modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                modulus_md5 = cert_utils.modulus_md5_csr(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
+                )
+                self.assertEqual(
+                    modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_csr > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_csr > openssl fallback",
+                        logged.output,
+                    )
 
         # csr sets
         for csr_filename in sorted(CSR_SETS.keys()):
             csr_pem_filepath = self._filepath_testfile(csr_filename)
             csr_pem = self._filedata_testfile(csr_filename)
             modulus_md5 = cert_utils.modulus_md5_csr(
                 csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
             )
             if modulus_md5 is None:
                 # TODO: no way of testing this in Pure-python right now
                 if self.__class__ == UnitTest_CertUtils:
                     continue
+                elif cert_utils.core.openssl_crypto:
+                    continue
             self.assertEqual(modulus_md5, CSR_SETS[csr_filename]["modulus_md5"])
+            # no need to test for fallback behavior again
 
     def test__modulus_md5_cert(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__modulus_md5_cert
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
-            modulus_md5 = cert_utils.modulus_md5_cert(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
-            self.assertEqual(
-                modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                modulus_md5 = cert_utils.modulus_md5_cert(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                self.assertEqual(
+                    modulus_md5, self._cert_sets[cert_set]["pubkey_modulus_md5"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_cert > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.modulus_md5_cert > openssl fallback",
+                        logged.output,
+                    )
 
         # ca certs
         for cert_filename in sorted(CERT_CA_SETS.keys()):
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
             modulus_md5 = cert_utils.modulus_md5_cert(
                 cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
             )
             self.assertEqual(modulus_md5, CERT_CA_SETS[cert_filename]["modulus_md5"])
+            # no need to test for fallback behavior again
 
     def test__parse_cert__enddate(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__parse_cert__enddate
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
-            cert_enddate = cert_utils.parse_cert__enddate(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
-            self.assertEqual(
-                str(cert_enddate), self._cert_sets[cert_set]["cert.notAfter"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                cert_enddate = cert_utils.parse_cert__enddate(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                self.assertEqual(
+                    str(cert_enddate), self._cert_sets[cert_set]["cert.notAfter"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_cert__enddate > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_cert__enddate > openssl fallback",
+                        logged.output,
+                    )
 
     def test__parse_cert__startdate(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__parse_cert__startdate
         """
 
         for cert_set in sorted(self._cert_sets.keys()):
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
-            cert_startdate = cert_utils.parse_cert__startdate(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
-            self.assertEqual(
-                str(cert_startdate), self._cert_sets[cert_set]["cert.notBefore"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                cert_startdate = cert_utils.parse_cert__startdate(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                self.assertEqual(
+                    str(cert_startdate), self._cert_sets[cert_set]["cert.notBefore"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_cert__startdate > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_cert__startdate > openssl fallback",
+                        logged.output,
+                    )
 
     def test__parse_cert(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__parse_cert
         python -m unittest tests.test_unit.UnitTest_CertUtils_fallback.test__parse_cert
 
         This UnitTest tests the following functions:
@@ -517,17 +775,32 @@
             if not self._cert_sets[cert_set]["cert"]:
                 continue
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
 
             # `cert_utils.parse_cert`
-            rval = cert_utils.parse_cert(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                rval = cert_utils.parse_cert(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_cert > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_cert > openssl fallback",
+                        logged.output,
+                    )
             self.assertEqual(
                 rval["fingerprint_sha1"],
                 self._cert_sets[cert_set]["cert.fingerprints"]["sha1"],
             )
             self.assertEqual(
                 rval["spki_sha256"], self._cert_sets[cert_set]["spki_sha256"]
             )
@@ -536,17 +809,33 @@
             )
             self.assertEqual(
                 rval["authority_key_identifier"],
                 self._cert_sets[cert_set]["cert.authority_key_identifier"],
             )
 
             # `cert_utils.parse_cert__spki_sha256`
-            spki_sha256 = cert_utils.parse_cert__spki_sha256(
-                cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                spki_sha256 = cert_utils.parse_cert__spki_sha256(
+                    cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_cert__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_cert__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
+
             self.assertEqual(spki_sha256, self._cert_sets[cert_set]["spki_sha256"])
             spki_sha256_b64 = cert_utils.parse_cert__spki_sha256(
                 cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath, as_b64=True
             )
             self.assertEqual(
                 spki_sha256_b64, self._cert_sets[cert_set]["spki_sha256.b64"]
             )
@@ -622,52 +911,93 @@
             if not self._cert_sets[cert_set]["csr"]:
                 raise ValueError("missing csr!")
             csr_filename = "unit_tests/cert_%s/csr.pem" % cert_set
             csr_pem_filepath = self._filepath_testfile(csr_filename)
             csr_pem = self._filedata_testfile(csr_filename)
 
             # `cert_utils.parse_csr`
-            rval = cert_utils.parse_csr(
-                csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
-            )
-            self.assertEqual(
-                rval["key_technology"],
-                self._cert_sets[cert_set]["key_technology"],
-            )
-            self.assertEqual(
-                rval["spki_sha256"], self._cert_sets[cert_set]["spki_sha256"]
-            )
-            self.assertEqual(
-                rval["subject"],
-                self._cert_sets[cert_set]["csr.subject"],
-            )
-            self.assertEqual(
-                rval["SubjectAlternativeName"],
-                self._cert_sets[cert_set]["csr.domains.san"],
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                rval = cert_utils.parse_csr(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
+                )
+                self.assertEqual(
+                    rval["key_technology"],
+                    self._cert_sets[cert_set]["key_technology"],
+                )
+                self.assertEqual(
+                    rval["spki_sha256"], self._cert_sets[cert_set]["spki_sha256"]
+                )
+                self.assertEqual(
+                    rval["subject"],
+                    self._cert_sets[cert_set]["csr.subject"],
+                )
+                self.assertEqual(
+                    rval["SubjectAlternativeName"],
+                    self._cert_sets[cert_set]["csr.domains.san"],
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_csr > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_csr > openssl fallback",
+                        logged.output,
+                    )
 
             # `cert_utils.parse_csr__spki_sha256`
-            spki_sha256 = cert_utils.parse_csr__spki_sha256(
-                csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
-            )
-            self.assertEqual(spki_sha256, self._cert_sets[cert_set]["spki_sha256"])
-            spki_sha256_b64 = cert_utils.parse_csr__spki_sha256(
-                csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath, as_b64=True
-            )
-            self.assertEqual(
-                spki_sha256_b64, self._cert_sets[cert_set]["spki_sha256.b64"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                spki_sha256 = cert_utils.parse_csr__spki_sha256(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
+                )
+                self.assertEqual(spki_sha256, self._cert_sets[cert_set]["spki_sha256"])
+                spki_sha256_b64 = cert_utils.parse_csr__spki_sha256(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath, as_b64=True
+                )
+                self.assertEqual(
+                    spki_sha256_b64, self._cert_sets[cert_set]["spki_sha256.b64"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_csr__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_csr__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
 
-            # `cert_utils.parse_csr__key_technology`
-            key_technology = cert_utils.parse_csr__key_technology(
-                csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
-            )
-            self.assertEqual(
-                key_technology, self._cert_sets[cert_set]["key_technology"]
-            )
+            # `cert_utils.parse_csr__key_technology
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                key_technology = cert_utils.parse_csr__key_technology(
+                    csr_pem=csr_pem, csr_pem_filepath=csr_pem_filepath
+                )
+                self.assertEqual(
+                    key_technology, self._cert_sets[cert_set]["key_technology"]
+                )
+                if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_csr__key_technology > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_csr__key_technology > openssl fallback",
+                        logged.output,
+                    )
 
         # extended csr
         for csr_set in sorted(self._csr_sets_alt.keys()):
             if not self._csr_sets_alt[csr_set]["csr"]:
                 raise ValueError("missing csr!")
             csr_filename = "%s/%s" % (
                 self._csr_sets_alt[csr_set]["directory"],
@@ -732,46 +1062,87 @@
 
         for cert_set in sorted(self._cert_sets.keys()):
             key_filename = "unit_tests/cert_%s/privkey.pem" % cert_set
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
 
             # `cert_utils.parse_key`
-            rval = cert_utils.parse_key(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            self.assertEqual(
-                rval["key_technology"], self._cert_sets[cert_set]["key_technology"]
-            )
-            self.assertEqual(
-                rval["modulus_md5"], self._cert_sets[cert_set]["pubkey_modulus_md5"]
-            )
-            self.assertEqual(
-                rval["spki_sha256"], self._cert_sets[cert_set]["spki_sha256"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                rval = cert_utils.parse_key(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                self.assertEqual(
+                    rval["key_technology"], self._cert_sets[cert_set]["key_technology"]
+                )
+                self.assertEqual(
+                    rval["modulus_md5"], self._cert_sets[cert_set]["pubkey_modulus_md5"]
+                )
+                self.assertEqual(
+                    rval["spki_sha256"], self._cert_sets[cert_set]["spki_sha256"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_key > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_key > openssl fallback",
+                        logged.output,
+                    )
 
             # `cert_utils.parse_key__spki_sha256`
-            spki_sha256 = cert_utils.parse_key__spki_sha256(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            self.assertEqual(spki_sha256, self._cert_sets[cert_set]["spki_sha256"])
-            spki_sha256_b64 = cert_utils.parse_key__spki_sha256(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath, as_b64=True
-            )
-            self.assertEqual(
-                spki_sha256_b64, self._cert_sets[cert_set]["spki_sha256.b64"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                spki_sha256 = cert_utils.parse_key__spki_sha256(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                self.assertEqual(spki_sha256, self._cert_sets[cert_set]["spki_sha256"])
+                spki_sha256_b64 = cert_utils.parse_key__spki_sha256(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath, as_b64=True
+                )
+                self.assertEqual(
+                    spki_sha256_b64, self._cert_sets[cert_set]["spki_sha256.b64"]
+                )
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_key__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_key__spki_sha256 > openssl fallback",
+                        logged.output,
+                    )
 
             # `cert_utils.parse_key__technology`
-            key_technology = cert_utils.parse_key__technology(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            self.assertEqual(
-                key_technology, self._cert_sets[cert_set]["key_technology"]
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                key_technology = cert_utils.parse_key__technology(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                self.assertEqual(
+                    key_technology, self._cert_sets[cert_set]["key_technology"]
+                )
+                if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.parse_key__technology > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.parse_key__technology > openssl fallback",
+                        logged.output,
+                    )
 
         # this will test against EC+RSA
         for key_filename in sorted(KEY_SETS.keys()):
             key_pem_filepath = self._filepath_testfile(key_filename)
             key_pem = self._filedata_testfile(key_filename)
 
             # `cert_utils.parse_key`
@@ -811,16 +1182,29 @@
             fullchain_pem_filepath = self._filepath_testfile(fullchain_filename)
             fullchain_pem = self._filedata_testfile(fullchain_filename)
 
             cert_filename = "unit_tests/cert_%s/cert.pem" % cert_set
             cert_pem_filepath = self._filepath_testfile(cert_filename)
             cert_pem = self._filedata_testfile(cert_filename)
 
-            (_cert, _chain) = cert_utils.cert_and_chain_from_fullchain(fullchain_pem)
-            self.assertEqual(_cert, cert_pem)
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                (_cert, _chain) = cert_utils.cert_and_chain_from_fullchain(
+                    fullchain_pem
+                )
+                self.assertEqual(_cert, cert_pem)
+                if self._fallback_global or (not cert_utils.core.certbot_crypto_util):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.cert_and_chain_from_fullchain > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.cert_and_chain_from_fullchain > openssl fallback",
+                        logged.output,
+                    )
 
     def test__analyze_chains(self):
         """
         This tests:
         * cert_utils.cert_and_chain_from_fullchain
         * cert_utils.decompose_chain
         * cert_utils.ensure_chain
@@ -862,32 +1246,54 @@
                 # decompose a fullchain
                 (_cert, _chain) = cert_utils.cert_and_chain_from_fullchain(
                     fullchain_pem
                 )
                 self.assertEqual(_cert, cert_pem)
                 self.assertEqual(_chain, test_pems[idx]["chain"])
 
-                _upstream_certs = cert_utils.decompose_chain(_chain)
-                self.assertEqual(len(_upstream_certs), count_intermediates)
-
-                _all_certs = cert_utils.decompose_chain(fullchain_pem)
-                self.assertEqual(len(_all_certs), count_intermediates + 1)
+                with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                    _upstream_certs = cert_utils.decompose_chain(_chain)
+                    self.assertEqual(len(_upstream_certs), count_intermediates)
+
+                    _all_certs = cert_utils.decompose_chain(fullchain_pem)
+                    self.assertEqual(len(_all_certs), count_intermediates + 1)
+                    if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                        self.assertIn(
+                            "DEBUG:cert_utils.core:.decompose_chain > openssl fallback",
+                            logged.output,
+                        )
+                    else:
+                        self.assertNotIn(
+                            "DEBUG:cert_utils.core:.decompose_chain > openssl fallback",
+                            logged.output,
+                        )
 
                 # `ensure_chain` can accept two types of data
                 root_pem = test_pems[idx]["root"]
-                self.assertTrue(
-                    cert_utils.ensure_chain(
-                        root_pem=root_pem, chain_pem=_chain, cert_pem=cert_pem
+                with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                    self.assertTrue(
+                        cert_utils.ensure_chain(
+                            root_pem=root_pem, chain_pem=_chain, cert_pem=cert_pem
+                        )
                     )
-                )
-                self.assertTrue(
-                    cert_utils.ensure_chain(
-                        root_pem=root_pem, fullchain_pem=fullchain_pem
+                    self.assertTrue(
+                        cert_utils.ensure_chain(
+                            root_pem=root_pem, fullchain_pem=fullchain_pem
+                        )
                     )
-                )
+                    if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                        self.assertIn(
+                            "DEBUG:cert_utils.core:.ensure_chain > openssl fallback",
+                            logged.output,
+                        )
+                    else:
+                        self.assertNotIn(
+                            "DEBUG:cert_utils.core:.ensure_chain > openssl fallback",
+                            logged.output,
+                        )
 
                 # `ensure_chain` will not accept user error
                 # fullchain error
                 _error_expected = "If `ensure_chain` is invoked with `fullchain_pem`, do not pass in `chain_pem` or `cert_pem`."
                 # invoking `fullchain_pem` with: `chain_pem`
                 with self.assertRaises(ValueError) as cm:
                     result = cert_utils.ensure_chain(
@@ -924,15 +1330,26 @@
                     result = cert_utils.ensure_chain(
                         root_pem=root_pem, cert_pem=cert_pem
                     )
 
                 # ENSURE THE CHAIN ORDER
                 # forward: YAY!
                 _all_certs = cert_utils.decompose_chain(fullchain_pem)
-                cert_utils.ensure_chain_order(_all_certs)
+                with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                    cert_utils.ensure_chain_order(_all_certs)
+                    if self._fallback_global or (not cert_utils.core.openssl_crypto):
+                        self.assertIn(
+                            "DEBUG:cert_utils.core:.ensure_chain_order > openssl fallback",
+                            logged.output,
+                        )
+                    else:
+                        self.assertNotIn(
+                            "DEBUG:cert_utils.core:.ensure_chain_order > openssl fallback",
+                            logged.output,
+                        )
                 # reverse: nay :(
                 _all_certs_reversed = _all_certs[::-1]
                 with self.assertRaises(OpenSslError) as cm:
                     cert_utils.ensure_chain_order(_all_certs_reversed)
                 self.assertTrue(cm.exception.args[0].startswith("could not verify:"))
 
     def test__convert_lejson_to_pem(self):
@@ -952,15 +1369,30 @@
 
             # load the pem
             key_pem_filename = "unit_tests/account_%s/private_key.pem" % account_set
             key_pem_filepath = self._filepath_testfile(key_pem_filename)
             key_pem = self._filedata_testfile(key_pem_filepath)
 
             # convert
-            rval = cert_utils.convert_lejson_to_pem(key_jsons)
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                rval = cert_utils.convert_lejson_to_pem(key_jsons)
+            if (
+                self._fallback_global
+                or (not cert_utils.core.crypto_serialization)
+                or (not cert_utils.core.josepy)
+            ):
+                self.assertIn(
+                    "DEBUG:cert_utils.core:.convert_lejson_to_pem > openssl fallback",
+                    logged.output,
+                )
+            else:
+                self.assertNotIn(
+                    "DEBUG:cert_utils.core:.convert_lejson_to_pem > openssl fallback",
+                    logged.output,
+                )
 
             # compare
             self.assertEqual(rval, key_pem)
 
     def test__account_key__parse(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__account_key__parse
@@ -970,17 +1402,28 @@
                 raise ValueError("need pem")
 
             # load the pem
             key_pem_filename = "unit_tests/account_%s/private_key.pem" % account_set
             key_pem_filepath = self._filepath_testfile(key_pem_filename)
             key_pem = self._filedata_testfile(key_pem_filepath)
 
-            rval = cert_utils.account_key__parse(
-                key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                rval = cert_utils.account_key__parse(
+                    key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                if self._fallback_global or (not cert_utils.core.josepy):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.account_key__parse > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.account_key__parse > openssl fallback",
+                        logged.output,
+                    )
 
     def test__account_key__sign(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__account_key__sign
         """
         for account_set in sorted(self._account_sets.keys()):
             if not self._account_sets[account_set]["pem"]:
@@ -990,19 +1433,36 @@
             key_pem_filename = "unit_tests/account_%s/private_key.pem" % account_set
             key_pem_filepath = self._filepath_testfile(key_pem_filename)
             key_pem = self._filedata_testfile(key_pem_filepath)
 
             input = self._account_sets[account_set]["signature.input"]
             expected = self._account_sets[account_set]["signature.output"]
 
-            signature = cert_utils.account_key__sign(
-                input, key_pem=key_pem, key_pem_filepath=key_pem_filepath
-            )
-            signature = cert_utils.jose_b64(signature)
-            self.assertEqual(signature, expected)
+            with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+                signature = cert_utils.account_key__sign(
+                    input, key_pem=key_pem, key_pem_filepath=key_pem_filepath
+                )
+                signature = cert_utils.jose_b64(signature)
+                self.assertEqual(signature, expected)
+
+                if (
+                    self._fallback_global
+                    or (not cert_utils.core.openssl_crypto)
+                    or (not cert_utils.core.crypto_rsa)
+                    or (not cert_utils.core.cryptography)
+                ):
+                    self.assertIn(
+                        "DEBUG:cert_utils.core:.account_key__sign > openssl fallback",
+                        logged.output,
+                    )
+                else:
+                    self.assertNotIn(
+                        "DEBUG:cert_utils.core:.account_key__sign > openssl fallback",
+                        logged.output,
+                    )
 
     def test__private_key__new(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test__private_key__new
         """
         _combinations = (
             (model.KeyTechnology.RSA, 2048, None),
@@ -1026,29 +1486,121 @@
                     ),
                 )
             elif _combo[0] == model.KeyTechnology.RSA:
                 self.assertEqual(
                     "-----BEGIN EC PRIVATE KEY-----", key_pem.split("\n")[0]
                 )
 
+    def test_new_key_ec(self):
+        # test no bits
+        with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+            key_pem = cert_utils.new_key_ec()
+            self.assertIn("-----BEGIN EC PRIVATE KEY-----", key_pem)
+            if (
+                self._fallback_global
+                or (not cert_utils.core.crypto_ec)
+                or (not cert_utils.core.crypto_serialization)
+            ):
+                self.assertIn(
+                    "DEBUG:cert_utils.core:.new_key_ec > openssl fallback",
+                    logged.output,
+                )
+            else:
+                self.assertNotIn(
+                    "DEBUG:cert_utils.core:.new_key_ec > openssl fallback",
+                    logged.output,
+                )
+
+        # test valid bits
+        key_pem = cert_utils.new_key_ec(bits=256)
+        self.assertIn("-----BEGIN EC PRIVATE KEY-----", key_pem)
+        key_pem = cert_utils.new_key_ec(bits=384)
+        self.assertIn("-----BEGIN EC PRIVATE KEY-----", key_pem)
+
+        # test invalid bits
+        with self.assertRaises(ValueError) as cm:
+            key_pem = cert_utils.new_key_ec(bits=1)
+        self.assertIn(
+            "LetsEncrypt only supports ECDSA keys with bits:", cm.exception.args[0]
+        )
+
+    def test_new_key_rsa(self):
+        # test no bits
+
+        def _key_compliance(key_pem: str):
+            # crypto: -----BEGIN PRIVATE KEY-----
+            # openssl fallback: -----BEGIN RSA PRIVATE KEY-----
+            self.assertIn(
+                key_pem.split("\n")[0],
+                (
+                    "-----BEGIN RSA PRIVATE KEY-----",
+                    "-----BEGIN PRIVATE KEY-----",
+                ),
+            )
+
+        with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+            key_pem = cert_utils.new_key_rsa()
+            _key_compliance(key_pem)
+            if self._fallback_global or (not cert_utils.core.certbot_crypto_util):
+                self.assertIn(
+                    "DEBUG:cert_utils.core:.new_key_rsa > openssl fallback",
+                    logged.output,
+                )
+            else:
+                self.assertNotIn(
+                    "DEBUG:cert_utils.core:.new_key_rsa > openssl fallback",
+                    logged.output,
+                )
+
+        # test valid bits
+        key_pem = cert_utils.new_key_rsa(bits=2048)
+        _key_compliance(key_pem)
+
+        key_pem = cert_utils.new_key_rsa(bits=3072)
+        _key_compliance(key_pem)
+
+        key_pem = cert_utils.new_key_rsa(bits=4096)
+        _key_compliance(key_pem)
+
+        # test invalid bits
+        with self.assertRaises(ValueError) as cm:
+            key_pem = cert_utils.new_key_rsa(bits=1)
+        self.assertIn(
+            "LetsEncrypt only supports RSA keys with bits:", cm.exception.args[0]
+        )
+
     def test_convert_pkcs7_to_pems(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test_convert_pkcs7_to_pems
         python -m unittest tests.test_unit.UnitTest_CertUtils_fallback.test_convert_pkcs7_to_pems
         """
         fname_pkcs7 = "letsencrypt-certs/trustid-x3-root.p7c"
         fpath_pkcs7 = self._filepath_testfile(fname_pkcs7)
         fdata_pkcs7 = self._filedata_testfile(fname_pkcs7, is_binary=True)
-        pkcs7_pems = cert_utils.convert_pkcs7_to_pems(fdata_pkcs7)
+        with self.assertLogs("cert_utils.core", level="DEBUG") as logged:
+            pkcs7_pems = cert_utils.convert_pkcs7_to_pems(fdata_pkcs7)
+            if (
+                self._fallback_global
+                or (not cert_utils.core.crypto_pkcs7)
+                or (not cert_utils.core.crypto_serialization)
+            ):
+                self.assertIn(
+                    "DEBUG:cert_utils.core:.convert_pkcs7_to_pems > openssl fallback",
+                    logged.output,
+                )
+            else:
+                self.assertNotIn(
+                    "DEBUG:cert_utils.core:.convert_pkcs7_to_pems > openssl fallback",
+                    logged.output,
+                )
 
         fname_pem = "letsencrypt-certs/trustid-x3-root.pem"
         fpath_pem = self._filedata_testfile(fname_pem)
         fdata_pem = self._filedata_testfile(fname_pem)
         pem_pem = cert_utils.cleanup_pem_text(fdata_pem)
-
         self.assertEqual(len(pkcs7_pems), 1)
         self.assertEqual(pkcs7_pems[0], pem_pem)
 
     def test_convert_pkix_to_pem(self):
         """
         python -m unittest tests.test_unit.UnitTest_CertUtils.test_convert_pkix_to_pem
         python -m unittest tests.test_unit.UnitTest_CertUtils_fallback.test_convert_pkix_to_pem
@@ -1062,18 +1614,21 @@
         fpath_pem = self._filedata_testfile(fname_pem)
         fdata_pem = self._filedata_testfile(fname_pem)
         pem_pem = cert_utils.cleanup_pem_text(fdata_pem)
 
         self.assertEqual(pkix_pem, pem_pem)
 
 
-class UnitTest_OpenSSL(unittest.TestCase, _Mixin_filedata):
+class UnitTest_OpenSSL(unittest.TestCase, _Mixin_fallback_possible, _Mixin_filedata):
     """python -m unittest tests.test_unit.UnitTest_OpenSSL"""
 
     def test_modulus_PrivateKey(self):
+        """
+        modulus_md5_key is covered in the CertUtils tests. not sure why we have this
+        """
         for pkey_set_id, set_data in sorted(TEST_FILES["PrivateKey"].items()):
             key_pem_filepath = self._filepath_testfile(set_data["file"])
             key_pem = self._filedata_testfile(key_pem_filepath)
             _computed_modulus_md5 = cert_utils.modulus_md5_key(
                 key_pem=key_pem,
                 key_pem_filepath=key_pem_filepath,
             )
@@ -1098,20 +1653,93 @@
 
 class UnitTest_CertUtils_fallback(_MixinNoCrypto, UnitTest_CertUtils):
     """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback"""
 
     pass
 
 
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_acme(_Mixin_Missing_acme, UnitTest_CertUtils):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_acme"""
+
+    pass
+
+
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_missing_acme(_Mixin_Missing_acme, UnitTest_CertUtils):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_missing_acme"""
+
+    pass
+
+
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_missing_certbot(
+    _Mixin_Missing_certbot, UnitTest_CertUtils
+):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_missing_certbot"""
+
+    pass
+
+
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_missing_cryptography(
+    _Mixin_Missing_cryptography, UnitTest_CertUtils
+):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_missing_cryptography"""
+
+    pass
+
+
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_missing_josepy(
+    _Mixin_Missing_josepy, UnitTest_CertUtils
+):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_missing_josepy"""
+
+    pass
+
+
+@unittest.skipUnless(EXTENDED_TESTS, "Extended tests disabled")
+class UnitTest_CertUtils_fallback_missing_openssl_crypto(
+    _Mixin_Missing_openssl_crypto, UnitTest_CertUtils
+):
+    """python -m unittest tests.test_unit.UnitTest_CertUtils_fallback_missing_openssl_crypto"""
+
+    pass
+
+
 class UnitTest_OpenSSL_fallback(_MixinNoCrypto, UnitTest_OpenSSL):
     """python -m unittest tests.test_unit.UnitTest_OpenSSL_fallback"""
 
     pass
 
 
+class UnitTest_api(unittest.TestCase):
+    """python -m unittest tests.test_unit.UnitTest_api"""
+
+    def test_check_openssl_version(self):
+        """
+        # this is not set until used, but we can't trust the execution order
+        import cert_utils
+        _original = cert_utils.core.openssl_version
+        self.assertIsNone(_original)
+        """
+        # invoking `check` will return the new version
+        active = cert_utils.check_openssl_version()
+        # first invocation should set the value
+        self.assertEqual(active, cert_utils.core.openssl_version)
+
+        # let's try to replace it
+        cert_utils.core.openssl_version = "x"
+        self.assertEqual("x", cert_utils.core.openssl_version)
+        new = cert_utils.check_openssl_version(replace=True)
+        self.assertEqual(active, new)
+        self.assertEqual(new, cert_utils.core.openssl_version)
+
+
 class UnitTest_utils(unittest.TestCase):
     """python -m unittest tests.test_unit.UnitTest_utils"""
 
     def test_validate_domains__valid(self):
         domains = (
             "EXAMPLE.com",
             "example.com",
```

### Comparing `cert_utils-0.1.0/tests/_utils.py` & `cert_utils-0.1.1/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/LICENSE.txt` & `cert_utils-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/setup.py` & `cert_utils-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 tests_require = [
     "certbot",
     "cryptography",
     "josepy",
     "mypy",
     "pytest",
     "types-psutil",
-    "types-pyOpenSSL",
     "types-python-dateutil",
     "types-requests",
 ]
 
 # PyOpenSSL Version Pinning
 #   23.1.0 is a bad release, see
 #   https://github.com/pyca/pyopenssl/issues/1199
 if (sys.version_info.major == 3) and (sys.version_info.minor == 6):
     # PyOpenSSl 23.2.0 introduces a backwards incompatible change
     #   Invalid versions are now rejected in OpenSSL.crypto.X509Req.set_version.
     # The `acme` package (via Certbot) ends support for py3.6 on version `v1.23.0`
     #   v1.23.0 calls make_csr with a bad version, and does not pin PyOpenSSL
     tests_require.append("PyOpenSSL>=17.5.0,!=23.1.0,<23.2.0")
+    tests_require.append("types-PyOpenSSL>=17.5.0,!=23.1.0,<23.2.0")
 else:
     tests_require.append("PyOpenSSL>=17.5.0,!=23.1.0")
+    tests_require.append("types-PyOpenSSL>=17.5.0,!=23.1.0")
 
 testing_extras = tests_require + []
 
 setup(
     name="cert_utils",
     description="TLS/SSL Certiicate Utilities",
     long_description=long_description,
```

### Comparing `cert_utils-0.1.0/src/cert_utils/core.py` & `cert_utils-0.1.1/src/cert_utils/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import logging
 import os
 import re
 import subprocess
 import tempfile
 import textwrap
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import Union
@@ -57,67 +58,73 @@
         EllipticCurvePublicKey,
         Ed25519PublicKey,
         Ed448PublicKey,
         X25519PublicKey,
         X448PublicKey,
     ]
 
+# ------------------------------------------------------------------------------
 # Conditional Imports
 try:
     from acme import crypto_util as acme_crypto_util
+except ImportError:
+    acme_crypto_util = None  # type: ignore[assignment]
+
+try:
     from certbot import crypto_util as certbot_crypto_util
+except ImportError:
+    certbot_crypto_util = None  # type: ignore[assignment]
 
-    # from Crypto.Util import crypto_util_asn1
+try:
     import cryptography
-    from cryptography.hazmat.backends import default_backend
-    from cryptography.hazmat.primitives import (
-        serialization as cryptography_serialization,
-    )
+    from cryptography.hazmat.backends import default_backend as crypto_default_backend
+    from cryptography.hazmat.primitives import serialization as crypto_serialization
     from cryptography.hazmat.primitives.asymmetric import ec as crypto_ec
     from cryptography.hazmat.primitives.asymmetric import rsa as crypto_rsa
-
-    try:
-        from cryptography.hazmat.primitives.serialization import pkcs7 as crypto_pkcs7
-    except ImportError as exc:  # noqa: F841
-        crypto_pkcs7 = None  # type: ignore[assignment]
-    import josepy
-    from OpenSSL import crypto as openssl_crypto
-
-except ImportError as exc:  # noqa: F841
-    acme_crypto_util = None  # type: ignore[assignment]
-    certbot_crypto_util = None  # type: ignore[assignment]
-    # crypto_util_asn1 = None  # type: ignore[assignment]
+    from cryptography.hazmat.primitives.serialization import pkcs7 as crypto_pkcs7
+except ImportError:
+    raise
     cryptography = None  # type: ignore[assignment]
-    default_backend = None  # type: ignore[assignment]
-    cryptography_serialization = None  # type: ignore[assignment]
+    crypto_default_backend = None  # type: ignore[assignment]
+    crypto_serialization = None  # type: ignore[assignment]
     crypto_ec = None  # type: ignore[assignment]
     crypto_rsa = None  # type: ignore[assignment]
     crypto_pkcs7 = None  # type: ignore[assignment]
+
+try:
+    import josepy
+except ImportError:
     josepy = None  # type: ignore[assignment]
+
+try:
+    from OpenSSL import crypto as openssl_crypto
+except ImportError:
     openssl_crypto = None  # type: ignore[assignment]
 
+# ------------------------------------------------------------------------------
+
 NEEDS_TEMPFILES = True
 if (
     acme_crypto_util
-    and cryptography_serialization
     and certbot_crypto_util
+    and crypto_serialization
     and josepy
     and openssl_crypto
 ):
     """
     acme_crypto_util
         make_csr
-    cryptography_serialization
-        convert_pkcs7_to_pems
-        convert_lejson_to_pem
     certbot_crypto_util
         parse_cert__domains
         validate_key
         validate_csr
         cert_and_chain_from_fullchain
+    crypto_serialization
+        convert_pkcs7_to_pems
+        convert_lejson_to_pem
     josepy:
         account_key__parse
     openssl_crypto and certbot_crypto_util
         parse_csr_domains
         parse_cert__spki_sha256
         parse_csr__spki_sha256
         parse_key__spki_sha256
@@ -173,15 +180,15 @@
 # * disable HTTP Challenge pre-Read
 TESTING_ENVIRONMENT = False
 
 # LetsEncrypt max
 MAX_DOMAINS_PER_CERTIFICATE = 100
 
 
-def update_from_appsettings(appsettings: Dict) -> None:
+def update_from_appsettings(appsettings: Dict[str, Any]) -> None:
     """
     update the module data based on settings
 
     :param appsettings: a dict containing the Pyramid application settings
     :type appsettings: dict or dict-like
     """
     global openssl_path
@@ -457,25 +464,27 @@
     :rtype: list
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl pkcs7 -inform DER -in {FILEPATH} -print_certs -outform PEM
     """
     log.info("convert_pkcs7_to_pems >")
-    if cryptography_serialization:
+    if crypto_pkcs7 and crypto_serialization:
         certs_loaded = crypto_pkcs7.load_der_pkcs7_certificates(pkcs7_data)
         certs_bytes = [
-            cert.public_bytes(cryptography_serialization.Encoding.PEM)
+            cert.public_bytes(crypto_serialization.Encoding.PEM)
             for cert in certs_loaded
         ]
         certs_string = [cert.decode("utf8") for cert in certs_bytes]
         certs_string = [cleanup_pem_text(cert) for cert in certs_string]
         return certs_string
     log.debug(".convert_pkcs7_to_pems > openssl fallback")
     _tmpfile_der = new_der_tempfile(pkcs7_data)
+    if openssl_version is None:
+        check_openssl_version()
     try:
         cert_der_filepath = _tmpfile_der.name
         with psutil.Popen(
             [
                 openssl_path,
                 "pkcs7",
                 "-inform",
@@ -642,14 +651,16 @@
     :rtype: str
 
     This runs via OpenSSL:
 
         openssl x509 -in {FILEPATH}
     """
     _tmpfile_pem = new_pem_tempfile(cert_pem)
+    if openssl_version is None:
+        check_openssl_version()
     try:
         cert_pem_filepath = _tmpfile_pem.name
         with psutil.Popen(
             [openssl_path, "x509", "-in", cert_pem_filepath],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         ) as proc:
@@ -687,14 +698,16 @@
         openssl dgst -sha256 -binary | \
         openssl enc -base64
     """
     if key_technology not in ("EC", "RSA"):
         raise ValueError("must submit `key_technology`")
     key_technology = key_technology.lower()
     spki_hash = None
+    if openssl_version is None:
+        check_openssl_version()
     # convert to DER
     p1 = p2 = p3 = proc4 = None
     try:
         # extract the key
         p1 = psutil.Popen(
             [
                 openssl_path,
@@ -797,14 +810,16 @@
         openssl {key_technology} -pubout -outform DER -pubin | \
         openssl dgst -sha256 -binary | \
         openssl enc -base64
     """
     if key_technology not in ("EC", "RSA"):
         raise ValueError("must submit `key_technology`")
     key_technology = key_technology.lower()
+    if openssl_version is None:
+        check_openssl_version()
     spki_hash = None
     # convert to DER
     p1 = p2 = p3 = proc4 = None
     try:
         # extract the key
         p1 = psutil.Popen(
             [
@@ -905,14 +920,16 @@
 
         openssl rsa -in {KEY_FILEPATH} -pubout -outform der | \
         openssl dgst -sha256 -binary | \
         openssl enc -base64
     """
     if key_technology not in ("EC", "RSA"):
         raise ValueError("must submit `key_technology`")
+    if openssl_version is None:
+        check_openssl_version()
     key_technology = key_technology.lower()
     spki_hash = None
     # convert to DER
     p1 = p2 = proc3 = None
     try:
         # convert to DER
         p1 = psutil.Popen(
@@ -979,15 +996,17 @@
                     pass
     return spki_hash
 
 
 # ==============================================================================
 
 
-def _openssl_crypto__key_technology(key: Union[Type, "PKey"]) -> Optional[str]:
+def _openssl_crypto__key_technology(
+    key: Union[Type, "PKey"],
+) -> Optional[str]:
     """
     :param key: key object, with a `type()` method
     :type key: instance of
       * `openssl_crypto.load_certificate.get_pubkey()`, or
       * `openssl_crypto.load_privatekey()`, or
       * similar
     :returns: type of key: RSA, EC, DSA
@@ -1014,16 +1033,16 @@
     :type cryptography_publickey: cryptography.hazmat.backends.openssl.rsa._RSAPublicKey
     :param as_b64: Should the result be returned in Base64 encoding? default None
     :type as_b64: boolean
     :returns: spki_sha256
     :rtype: str
     """
     _public_bytes = cryptography_publickey.public_bytes(  # type: ignore[union-attr]
-        cryptography_serialization.Encoding.DER,
-        cryptography_serialization.PublicFormat.SubjectPublicKeyInfo,
+        crypto_serialization.Encoding.DER,
+        crypto_serialization.PublicFormat.SubjectPublicKeyInfo,
     )
     spki_sha256 = hashlib.sha256(_public_bytes).digest()
     if as_b64:
         spki_sha256 = base64.b64encode(spki_sha256)
     else:
         spki_sha256 = binascii.b2a_hex(spki_sha256)
         spki_sha256 = spki_sha256.upper()
@@ -1236,14 +1255,16 @@
         #    :  both work, but lets go with the typing
         all_domains = certbot_crypto_util.get_names_from_cert(cert_pem.encode())
         return all_domains
 
     log.debug(".parse_cert__domains > openssl fallback")
     # fallback onto OpenSSL
     # `openssl x509 -in MYCERT -noout -text`
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "x509", "-in", cert_pem_filepath, "-noout", "-text"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if proc.returncode != 0:
@@ -1289,25 +1310,27 @@
     :rtype: list
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl req -in {FILEPATH} -noout -text
     """
     log.info("parse_csr_domains >")
-    if openssl_crypto and certbot_crypto_util:
+    if certbot_crypto_util and openssl_crypto:
         load_func = openssl_crypto.load_certificate_request
         # !!!: `_get_names_from_cert_or_req` is typed for `bytes`, but doctring is `string`
         #    :  both work, but lets go with the typing
         found_domains = certbot_crypto_util._get_names_from_cert_or_req(
             csr_pem.encode(), load_func, typ=openssl_crypto.FILETYPE_PEM
         )
     else:
         log.debug(".parse_csr_domains > openssl fallback")
         # fallback onto OpenSSL
         # openssl req -in MYCSR -noout -text
+        if openssl_version is None:
+            check_openssl_version()
         with psutil.Popen(
             [openssl_path, "req", "-in", csr_pem_filepath, "-noout", "-text"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         ) as proc:
             data_bytes, err = proc.communicate()
             if proc.returncode != 0:
@@ -1357,55 +1380,56 @@
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl EC -in {FILEPATH}
         openssl RSA -in {FILEPATH}
     """
     log.info("validate_key >")
-    if certbot_crypto_util:
+    if crypto_serialization and crypto_rsa and crypto_ec:
         log.debug(".validate_key > crypto")
         try:
             # rsa
             # try:
             #   data = certbot_crypto_util.valid_privkey(key_pem)
             # except OpenSslError_InvalidKey as exc:
             #   return None
-            data = cryptography_serialization.load_pem_private_key(
-                key_pem.encode(), None, default_backend()
+            data = crypto_serialization.load_pem_private_key(
+                key_pem.encode(), None, crypto_default_backend()
             )
             if isinstance(data, crypto_rsa.RSAPrivateKey):
                 return "RSA"
             elif isinstance(data, crypto_ec.EllipticCurvePrivateKey):
                 return "EC"
         except Exception as exc:
             raise OpenSslError_InvalidKey(exc)
-    else:
-        log.debug(".validate_key > openssl fallback")
+    log.debug(".validate_key > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
 
-        def _check_fallback(_technology):
-            log.debug(".validate_key > openssl fallback", _technology)
-            # openssl rsa -in {KEY} -check
-            try:
-                with psutil.Popen(
-                    [openssl_path, _technology, "-in", key_pem_filepath],
-                    stdout=subprocess.PIPE,
-                    stderr=subprocess.PIPE,
-                ) as proc:
-                    data_bytes, err = proc.communicate()
-                    if not data_bytes:
-                        raise OpenSslError_InvalidKey(err)
-                    data_str = data_bytes.decode("utf8")
-                    return data_str
-            except OpenSslError_InvalidKey as exc:  # noqa: F841
-                return None
+    def _check_fallback(_technology: str):
+        log.debug(".validate_key > openssl fallback: _check_fallback[%s]", _technology)
+        # openssl rsa -in {KEY} -check
+        try:
+            with psutil.Popen(
+                [openssl_path, _technology, "-in", key_pem_filepath],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            ) as proc:
+                data_bytes, err = proc.communicate()
+                if not data_bytes:
+                    raise OpenSslError_InvalidKey(err)
+                data_str = data_bytes.decode("utf8")
+                return data_str
+        except OpenSslError_InvalidKey as exc:  # noqa: F841
+            return None
 
-        if _check_fallback("rsa"):
-            return "RSA"
-        elif _check_fallback("ec"):
-            return "EC"
+    if _check_fallback("rsa"):
+        return "RSA"
+    elif _check_fallback("ec"):
+        return "EC"
 
     raise OpenSslError_InvalidKey()
 
 
 def validate_csr(
     csr_pem: str,
     csr_pem_filepath: Optional[str] = None,
@@ -1434,14 +1458,16 @@
         data = certbot_crypto_util.valid_csr(csr_pem.encode())
         if not data:
             raise OpenSslError_InvalidCSR()
         return True
 
     log.debug(".validate_csr > openssl fallback")
     # openssl req -text -noout -verify -in {CSR}
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "req", "-text", "-noout", "-verify", "-in", csr_pem_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -1481,14 +1507,16 @@
         except Exception as exc:
             raise OpenSslError_InvalidCertificate(exc)
         if not data:
             raise OpenSslError_InvalidCertificate()
         return True
 
     log.debug(".validate_cert > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tmpfile_cert = None
     if not cert_pem_filepath:
         _tmpfile_cert = new_pem_tempfile(cert_pem)
         cert_pem_filepath = _tmpfile_cert.name
     try:
         # openssl x509 -in {CERTIFICATE} -inform pem -noout -text
         with psutil.Popen(
@@ -1573,14 +1601,16 @@
             raise OpenSslError_InvalidCertificate()
         fingerprint = data.digest(algorithm)
         _fingerprint = fingerprint.decode("utf8")
         _fingerprint = _fingerprint.replace(":", "")
         return _fingerprint
 
     log.debug(".fingerprint_cert > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tmpfile_cert = None
     if not cert_pem_filepath:
         _tmpfile_cert = new_pem_tempfile(cert_pem)
         cert_pem_filepath = _tmpfile_cert.name
     try:
         with psutil.Popen(
             [
@@ -1732,25 +1762,28 @@
 
     The OpenSSL Equivalent / Fallback is::
 
         md5(openssl rsa -noout -modulus -in {FILEPATH})
     """
     # ???: Should this raise an Exception instead of returning `None`?
     log.info("modulus_md5_key >")
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         privkey = openssl_crypto.load_privatekey(
             openssl_crypto.FILETYPE_PEM, key_pem.encode()
         )
         if _openssl_crypto__key_technology(privkey) == "RSA":
             modn = privkey.to_cryptography_key().public_key().public_numbers().n  # type: ignore[union-attr]
             data_str = "{:X}".format(modn)
         else:
             return None
     else:
         log.debug(".modulus_md5_key > openssl fallback")
+        if openssl_version is None:
+            check_openssl_version()
         # original code was:
         # openssl rsa -noout -modulus -in {KEY} | openssl md5
         # BUT
         # that pipes into md5: "Modulus={MOD}\n"
         with psutil.Popen(
             [openssl_path, "rsa", "-noout", "-modulus", "-in", key_pem_filepath],
             stdout=subprocess.PIPE,
@@ -1783,15 +1816,16 @@
 
     The OpenSSL Equivalent / Fallback is::
 
         md5(openssl req -noout -modulus -in {FILEPATH})
     """
     # ???: Should this raise an Exception instead of returning `None`?
     log.info("modulus_md5_csr >")
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         csr = openssl_crypto.load_certificate_request(
             openssl_crypto.FILETYPE_PEM, csr_pem.encode()
         )
         _pubkey = csr.get_pubkey()
         if _openssl_crypto__key_technology(_pubkey) == "RSA":
             modn = _pubkey.to_cryptography_key().public_numbers().n  # type: ignore[union-attr]
             data_str = "{:X}".format(modn)
@@ -1799,14 +1833,16 @@
             return None
     else:
         log.debug(".modulus_md5_csr > openssl fallback")
         # original code was:
         # openssl req -noout -modulus -in {CSR} | openssl md5
         # BUT
         # that pipes into md5: "Modulus={MOD}\n"
+        if openssl_version is None:
+            check_openssl_version()
         with psutil.Popen(
             [openssl_path, "req", "-noout", "-modulus", "-in", csr_pem_filepath],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         ) as proc_modulus:
             data_bytes, err = proc_modulus.communicate()
             data_str = data_bytes.decode("utf8")
@@ -1833,15 +1869,16 @@
     :rtype: str or None
 
     The OpenSSL Equivalent / Fallback is::
 
         md5(openssl x509 -noout -modulus -in {FILEPATH})
     """
     log.info("modulus_md5_cert >")
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         cert = openssl_crypto.load_certificate(
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         _pubkey = cert.get_pubkey()
         if _openssl_crypto__key_technology(_pubkey) == "RSA":
             modn = cert.get_pubkey().to_cryptography_key().public_numbers().n  # type: ignore[union-attr]
             data_str = "{:X}".format(modn)
@@ -1849,14 +1886,16 @@
             return None
     else:
         log.debug(".modulus_md5_cert > openssl fallback")
         # original code was:
         # openssl x509 -noout -modulus -in {CERT} | openssl md5
         # BUT
         # that pipes into md5: "Modulus={MOD}\n"
+        if openssl_version is None:
+            check_openssl_version()
         with psutil.Popen(
             [openssl_path, "x509", "-noout", "-modulus", "-in", cert_pem_filepath],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         ) as proc_modulus:
             data_bytes, err = proc_modulus.communicate()
             data_str = data_bytes.decode("utf8")
@@ -1916,14 +1955,16 @@
         "-issuer",
         "-subject_hash",
         "-subject",
         "-startdate",
         "-enddate",
     ):
         raise ValueError("invalid `single_op`")
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "x509", "-noout", single_op, "-in", pem_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -1949,14 +1990,16 @@
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl x509 -noout -ext {EXT} -in {FILEPATH})
     """
     if ext not in ("subjectAltName", "authorityKeyIdentifier", "authorityInfoAccess"):
         raise ValueError("invalid `ext`")
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "x509", "-noout", "-ext", ext, "-in", pem_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -1984,14 +2027,16 @@
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl req -noout {OPERATION} -in {FILEPATH})
     """
     if single_op not in ("-subject",):
         raise ValueError("invalid `single_op`")
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "req", "-noout", single_op, "-in", pem_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -2042,15 +2087,16 @@
         openssl ec -noout -modulus -in {KEY}
         openssl ec -noout -text -in {KEY}
     """
     if keytype not in ("RSA", "EC"):
         raise ValueError("keytype must be `RSA or EC`")
     if single_op not in ("-check", "-modulus", "-text"):
         raise ValueError("invalid `single_op`")
-
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, keytype.lower(), "-noout", single_op, "-in", pem_filepath],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -2080,15 +2126,16 @@
     :rtype: datetime.datetime
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl x509 -noout -enddate -in {FILEPATH})
     """
     log.info("parse_cert__enddate >")
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         cert = openssl_crypto.load_certificate(
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         date = cert.to_cryptography().not_valid_after
     else:
         log.debug(".parse_cert__enddate > openssl fallback")
         # openssl x509 -enddate -noout -in {CERT}
@@ -2119,15 +2166,16 @@
     :rtype: datetime.datetime
 
     The OpenSSL Equivalent / Fallback is::
 
         openssl x509 -noout -startdate -in {FILEPATH})
     """
     log.info("parse_cert__startdate >")
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         cert = openssl_crypto.load_certificate(
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         date = cert.to_cryptography().not_valid_before
     else:
         log.debug(".parse_cert__startdate > openssl fallback")
         # openssl x509 -startdate -noout -in {CERT}
@@ -2144,15 +2192,15 @@
 
 def parse_cert__spki_sha256(
     cert_pem: str,
     cert_pem_filepath: Optional[str] = None,
     cryptography_cert: Optional["Certificate"] = None,
     key_technology: Optional[str] = None,
     as_b64: Optional[bool] = None,
-):
+) -> str:
     """
     :param str cert_pem: PEM encoded Certificate
     :param str cert_pem_filepath: Filepath to PEM encoded Certificate
     :param cryptography_cert: optional hint to aid in crypto commands
     :type cryptography_cert: `OpenSSL.crypto.load_certificate(...).to_cryptography()``
     :param str key_technology: optional hint to aid in openssl fallback
     :param bool as_b64: encode with b64?
@@ -2160,26 +2208,27 @@
     :rtype: str
 
     The OpenSSL Equivalent / Fallback is::
 
         :function :_openssl_spki_hash_cert
     """
     log.info("parse_cert__spki_sha256 >")
-    if openssl_crypto and certbot_crypto_util:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         if not cryptography_cert:
             cert = openssl_crypto.load_certificate(
                 openssl_crypto.FILETYPE_PEM, cert_pem.encode()
             )
             cryptography_cert = cert.to_cryptography()
         cryptography_publickey = cryptography_cert.public_key()
         return _cryptography__public_key_spki_sha256(
             cryptography_publickey,
             as_b64=as_b64,
         )
-    log.debug("parse_cert__spki_sha256 > openssl fallback")
+    log.debug(".parse_cert__spki_sha256 > openssl fallback")
     tmpfile_pem = None
     try:
         if key_technology is None:
             key_technology = parse_cert__key_technology(
                 cert_pem=cert_pem, cert_pem_filepath=cert_pem_filepath
             )
         spki_sha256 = _openssl_spki_hash_cert(
@@ -2216,14 +2265,16 @@
     if openssl_crypto:
         cert = openssl_crypto.load_certificate(
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         return _openssl_crypto__key_technology(cert.get_pubkey())
     log.debug(".parse_cert__key_technology > openssl fallback")
     # `openssl x509 -in MYCERT -noout -text`
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "x509", "-in", cert_pem_filepath, "-noout", "-text"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         _data_bytes, err = proc.communicate()
         if proc.returncode != 0:
@@ -2257,15 +2308,16 @@
         "key_technology": None,
         "fingerprint_sha1": None,
         "spki_sha256": None,
         "issuer_uri": None,
         "authority_key_identifier": None,
     }
 
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         cert = openssl_crypto.load_certificate(
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         cert_cryptography = cert.to_cryptography()
         _issuer = cert.get_issuer().get_components()
         _subject = cert.get_subject().get_components()
         rval["issuer"] = _format_crypto_components(_issuer, fieldset="issuer")
@@ -2384,14 +2436,16 @@
             try:
                 _text = cert_ext__pem_filepath(cert_pem_filepath, "authorityInfoAccess")
                 issuer_uri = issuer_uri_from_text(_text)
                 rval["issuer_uri"] = issuer_uri
             except Exception as exc:  # noqa: F841
                 pass
         else:
+            if openssl_version is None:
+                check_openssl_version()
             with psutil.Popen(
                 [openssl_path, "x509", "-text", "-noout", "-in", cert_pem_filepath],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             ) as proc_text:
                 data, err = proc_text.communicate()
                 data = data.decode("utf8")
@@ -2437,14 +2491,16 @@
         if not crypto_csr:
             crypto_csr = openssl_crypto.load_certificate_request(
                 openssl_crypto.FILETYPE_PEM, csr_pem.encode()
             )
         return _openssl_crypto__key_technology(crypto_csr.get_pubkey())
     log.debug(".parse_csr__key_technology > openssl fallback")
     # `openssl req -in MYCERT -noout -text`
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "req", "-in", csr_pem_filepath, "-noout", "-text"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if proc.returncode != 0:
@@ -2470,15 +2526,16 @@
     :rtype: str
 
     The OpenSSL Equivalent / Fallback is::
 
         :_see:_openssl_spki_hash_csr
     """
     log.info("parse_csr__spki_sha256 >")
-    if openssl_crypto and certbot_crypto_util:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         if not crypto_csr:
             crypto_csr = openssl_crypto.load_certificate_request(
                 openssl_crypto.FILETYPE_PEM, csr_pem.encode()
             )
         cryptography_publickey = crypto_csr.get_pubkey().to_cryptography_key()
         spki_sha256 = _cryptography__public_key_spki_sha256(
             cryptography_publickey, as_b64=as_b64
@@ -2518,15 +2575,16 @@
     rval: Dict[str, Union[None, List, str]] = {
         "key_technology": None,
         "spki_sha256": None,
         "SubjectAlternativeName": [],
         "subject": None,
     }
 
-    if openssl_crypto:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         _crypto_csr = openssl_crypto.load_certificate_request(
             openssl_crypto.FILETYPE_PEM, csr_pem.encode()
         )
         _subject = _crypto_csr.get_subject().get_components()
         rval["subject"] = _format_crypto_components(_subject, fieldset="subject")
         _cryptography_csr = _crypto_csr.to_cryptography()
         try:
@@ -2546,16 +2604,16 @@
             csr_pem_filepath=csr_pem_filepath,
             crypto_csr=_crypto_csr,
             as_b64=False,
         )
         return rval
 
     log.debug(".parse_csr > openssl fallback")
-    global openssl_version
-    global _openssl_behavior
+    if openssl_version is None:
+        check_openssl_version()
     tmpfile_pem = None
     try:
         if not csr_pem_filepath:
             tmpfile_pem = new_pem_tempfile(csr_pem)
             csr_pem_filepath = tmpfile_pem.name
         _subject2 = csr_single_op__pem_filepath(csr_pem_filepath, "-subject")
         rval["subject"] = _format_openssl_components(_subject2, fieldset="subject")
@@ -2564,15 +2622,14 @@
         )
         rval["spki_sha256"] = parse_csr__spki_sha256(
             csr_pem=csr_pem,
             csr_pem_filepath=csr_pem_filepath,
             key_technology=_key_technology,
             as_b64=False,
         )
-
         with psutil.Popen(
             [openssl_path, "req", "-text", "-noout", "-in", csr_pem_filepath],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         ) as proc_text:
             data, err = proc_text.communicate()
             data = data.decode("utf8")
@@ -2588,15 +2645,15 @@
 
 def parse_key__spki_sha256(
     key_pem: str,
     key_pem_filepath: Optional[str] = None,
     cryptography_publickey: Optional["_TYPES_CRYPTOGRAPHY_KEYS"] = None,
     key_technology: Optional[str] = None,
     as_b64: Optional[bool] = None,
-):
+) -> str:
     """
     :param str key_pem: Key in PEM form
     :param str key_pem_filepath: Filepath to PEM
     :param cryptography_publickey: optional hint to aid in crypto commands
     :type cryptography_publickey: cryptography.hazmat.backends.openssl.rsa._RSAPublicKey
         openssl_crypto.load_privatekey(...).to_cryptography_key().public_key()
     :param str key_technology: optional hint to aid in openssl fallback
@@ -2605,15 +2662,16 @@
     :rtype: str
 
     The OpenSSL Equivalent / Fallback is::
 
         :_see:_openssl_spki_hash_pkey
     """
     log.info("parse_key__spki_sha256 >")
-    if openssl_crypto and certbot_crypto_util:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         if not cryptography_publickey:
             _crypto_privkey = openssl_crypto.load_privatekey(
                 openssl_crypto.FILETYPE_PEM, key_pem
             )
             _cryptography_privkey = _crypto_privkey.to_cryptography_key()
             cryptography_publickey = _cryptography_privkey.public_key()  # type: ignore[union-attr]
         spki_sha256 = _cryptography__public_key_spki_sha256(
@@ -2649,15 +2707,15 @@
     :param str key_pem: Key in PEM form
     :param str key_pem_filepath: Filepath to PEM
     :param object crypto_privatekey: optional hint to aid in crypto commands
     :returns: key technology
     :rtype: str
     """
     log.info("parse_key__technology >")
-    if openssl_crypto and certbot_crypto_util:
+    if openssl_crypto:
         if not crypto_privatekey:
             crypto_privatekey = openssl_crypto.load_privatekey(
                 openssl_crypto.FILETYPE_PEM, key_pem
             )
         _cert_type = crypto_privatekey.type()
         if _cert_type == openssl_crypto.TYPE_RSA:
             return "RSA"
@@ -2688,15 +2746,18 @@
     except Exception as exc0:  # noqa: F841
         raise
     finally:
         if tmpfile_pem:
             tmpfile_pem.close()
 
 
-def parse_key(key_pem: str, key_pem_filepath: Optional[str] = None) -> Dict:
+def parse_key(
+    key_pem: str,
+    key_pem_filepath: Optional[str] = None,
+) -> Dict:
     """
     !!!: This is a debugging display function. The output is not guaranteed across installations.
 
     This routine will use crypto/certbot if available.
     If not, openssl is used via subprocesses
 
     :param str key_pem: Key in PEM encoding
@@ -2708,15 +2769,16 @@
     rval: Dict[str, Union[None, str]] = {
         "check": None,
         "text": None,
         "modulus_md5": None,
         "key_technology": None,
         "spki_sha256": None,
     }
-    if openssl_crypto and certbot_crypto_util:
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and cryptography:
         # TODO: crypto version of `--text`
 
         # this part ONLY works on RSA keys
         # can't do this with certbot/pyopenssl yet
         # see https://github.com/pyca/pyopenssl/issues/291
         # certbot just wraps that
         try:
@@ -2795,15 +2857,16 @@
         raise
     finally:
         if tmpfile_pem:
             tmpfile_pem.close()
 
 
 def new_account_key(
-    key_technology_id: int = KeyTechnology.RSA, rsa_bits: int = 2048
+    key_technology_id: int = KeyTechnology.RSA,
+    rsa_bits: int = 2048,
 ) -> str:
     """
     :param int key_technology_id: Key Technology type. Default: KeyTechnology.RSA
     :param int rsa_bits: number of bits. default 2048
     :returns: AccountKey in PEM format
     :rtype: str
     """
@@ -2851,28 +2914,28 @@
     log.debug(".new_key_ec > bits = %s", bits)
     if bits not in ALLOWED_BITS_ECDSA:
         raise ValueError(
             "LetsEncrypt only supports ECDSA keys with bits: %s; not %s"
             % (ALLOWED_BITS_ECDSA, bits)
         )
 
-    if openssl_crypto:
+    if crypto_ec and crypto_serialization and (crypto_default_backend is not None):
         # see https://github.com/pyca/pyopenssl/issues/291
         if 256 == bits:
             key = crypto_ec.generate_private_key(
-                crypto_ec.SECP256R1(), default_backend()
+                crypto_ec.SECP256R1(), crypto_default_backend()
             )
         elif 384 == bits:
             key = crypto_ec.generate_private_key(
-                crypto_ec.SECP384R1(), default_backend()
+                crypto_ec.SECP384R1(), crypto_default_backend()
             )
         key_pem = key.private_bytes(
-            encoding=cryptography_serialization.Encoding.PEM,
-            format=cryptography_serialization.PrivateFormat.TraditionalOpenSSL,
-            encryption_algorithm=cryptography_serialization.NoEncryption(),
+            encoding=crypto_serialization.Encoding.PEM,
+            format=crypto_serialization.PrivateFormat.TraditionalOpenSSL,
+            encryption_algorithm=crypto_serialization.NoEncryption(),
         )
         # load it: openssl_crypto.load_privatekey(openssl_crypto.FILETYPE_PEM, key_pem)
         key_pem_str = key_pem.decode("utf8")
         key_pem_str = cleanup_pem_text(key_pem_str)
         return key_pem_str
 
     log.debug(".new_key_ec > openssl fallback")
@@ -2880,14 +2943,16 @@
     curve = None
     if 256 == bits:
         curve = "secp256k1"
     elif 384 == bits:
         curve = "secp384r1"
     # openssl ecparam -name prime256v1 -genkey -noout -out private-key.pem
     # -noout will suppress printing the EC Param (see https://security.stackexchange.com/questions/29778/why-does-openssl-writes-ec-parameters-when-generating-private-key)
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "ecparam", "-name", curve, "-genkey", "-noout"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -2916,23 +2981,25 @@
     :rtype: str
     """
     log.info("new_key_rsa >")
     log.debug(".new_key_rsa > bits = %s", bits)
     if bits not in ALLOWED_BITS_RSA:
         raise ValueError(
             "LetsEncrypt only supports RSA keys with bits: %s; not %s"
-            % (ALLOWED_BITS_RSA, bits)
+            % (str(ALLOWED_BITS_RSA), bits)
         )
     if certbot_crypto_util:
         key_pem = certbot_crypto_util.make_key(bits)
         key_pem_str = key_pem.decode("utf8")
         key_pem_str = cleanup_pem_text(key_pem_str)
         return key_pem_str
     log.debug(".new_key_rsa > openssl fallback")
     # openssl genrsa 4096 > domain.key
+    if openssl_version is None:
+        check_openssl_version()
     with psutil.Popen(
         [openssl_path, "genrsa", str(bits)],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     ) as proc:
         data_bytes, err = proc.communicate()
         if not data_bytes:
@@ -2950,30 +3017,33 @@
             tmpfile_pem.close()
     return key_pem_str
 
 
 def convert_jwk_to_ans1(pkey_jsons: str) -> str:
     """
     input is a json string
-    much work from https://gist.github.com/JonLundy/f25c99ee0770e19dc595
+
+    adapted from https://github.com/JonLundy
+    who shared this gist under the MIT license:
+        https://gist.github.com/JonLundy/f25c99ee0770e19dc595
 
     :param pkey_jsons: JWK Key
     :type pkey_jsons: str
     :returns: Key in ANS1 Format
     :rtype: str
     """
     pkey = json.loads(pkey_jsons)
 
-    def enc(data):
-        missing_padding = 4 - len(data) % 4
+    def enc(data_bytes: bytes) -> str:
+        missing_padding = 4 - len(data_bytes) % 4
         if missing_padding:
-            data += b"=" * missing_padding
-        data = binascii.hexlify(base64.b64decode(data, b"-_")).upper()
-        data = data.decode("utf8")
-        return "0x" + data
+            data_bytes += b"=" * missing_padding
+        data_bytes = binascii.hexlify(base64.b64decode(data_bytes, b"-_")).upper()
+        data_str = data_bytes.decode("utf8")
+        return "0x" + data_str
 
     for k, v in list(pkey.items()):
         if k == "kty":
             continue
         pkey[k] = enc(v.encode())
 
     converted = []
@@ -2993,42 +3063,47 @@
 
 def convert_lejson_to_pem(pkey_jsons: str) -> str:
     """
     This routine will use crypto/certbot if available.
     If not, openssl is used via subprocesses
 
     input is a json string
-    much work from https://gist.github.com/JonLundy/f25c99ee0770e19dc595
+
+    adapted from https://github.com/JonLundy
+    who shared this gist under the MIT license:
+        https://gist.github.com/JonLundy/f25c99ee0770e19dc595
 
     openssl asn1parse -noout -out private_key.der -genconf <(python conv.py private_key.json)
     openssl rsa -in private_key.der -inform der > private_key.pem
     openssl rsa -in private_key.pem
 
     :param pkey_jsons: LetsEncrypt JSON formatted Key
     :type pkey_jsons: str
     :returns: Key in PEM Encoding
     :rtype: str
     """
     log.info("convert_lejson_to_pem >")
 
-    if cryptography_serialization:
+    if crypto_serialization and josepy:
         pkey = josepy.JWKRSA.json_loads(pkey_jsons)
         as_pem = pkey.key.private_bytes(
-            encoding=cryptography_serialization.Encoding.PEM,
-            format=cryptography_serialization.PrivateFormat.TraditionalOpenSSL,
-            encryption_algorithm=cryptography_serialization.NoEncryption(),
+            encoding=crypto_serialization.Encoding.PEM,
+            format=crypto_serialization.PrivateFormat.TraditionalOpenSSL,
+            encryption_algorithm=crypto_serialization.NoEncryption(),
         )
         as_pem = as_pem.decode("utf8")
         as_pem = cleanup_pem_text(as_pem)
 
         # note: we don't need to provide key_pem_filepath because we already rely on openssl
         key_technology = validate_key(key_pem=as_pem)
         return as_pem
 
     log.debug(".convert_lejson_to_pem > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     pkey_ans1 = convert_jwk_to_ans1(pkey_jsons)
     as_pem = None
     tmpfiles = []
     try:
         tmpfile_ans1 = new_pem_tempfile(pkey_ans1)
         tmpfiles.append(tmpfile_ans1)
 
@@ -3260,14 +3335,16 @@
             openssl_crypto.FILETYPE_PEM, cert_pem.encode()
         )
         _store_ctx = openssl_crypto.X509StoreContext(store, cert_parsed)
         _store_ctx.verify_certificate()
         return True
 
     log.debug(".ensure_chain > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tempfiles = []
     try:
         _tmpfile_root = new_pem_tempfile(root_pem)
         _tempfiles.append(_tmpfile_root)
 
         intermediates_unified = "\n".join(intermediates)
         _tempfile_intermediate = new_pem_tempfile(intermediates_unified)
@@ -3364,14 +3441,16 @@
                 continue
             # only after the first cert do we need to check the last cert
             upchain = parsed_certs[idx - 1]
             if upchain.get_subject() != cert.get_issuer():
                 raise OpenSslError("could not verify: upchain does not match issuer")
         return True
     log.debug(".ensure_chain_order > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tempfiles = {}
     _last_idx = len(r_chain_certs) - 1
     try:
         # make a bunch of tempfiles
         for _idx, cert_pem in enumerate(r_chain_certs):
             _tmpfile_cert = new_pem_tempfile(cert_pem)
             _tempfiles[_idx] = _tmpfile_cert
@@ -3471,14 +3550,16 @@
     if josepy:
         _jwk = josepy.JWKRSA.load(key_pem.encode("utf8"))
         jwk = _jwk.public_key().fields_to_partial_json()
         jwk["kty"] = "RSA"
         thumbprint = jose_b64(_jwk.thumbprint())
         return jwk, thumbprint, alg
     log.debug(".account_key__parse > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tmpfile = None
     try:
         if key_pem_filepath is None:
             _tmpfile = new_pem_tempfile(key_pem)
             key_pem_filepath = _tmpfile.name
         with psutil.Popen(
             [
@@ -3515,38 +3596,46 @@
     finally:
         if _tmpfile:
             _tmpfile.close()
 
 
 def account_key__sign(
     data,
-    key_pem=None,
-    key_pem_filepath=None,
-):
+    key_pem: str,
+    key_pem_filepath: Optional[str] = None,
+) -> bytes:
     """
     This routine will use crypto/certbot if available.
     If not, openssl is used via subprocesses
 
     :param key_pem: (required) the RSA Key in PEM format
     :param key_pem_filepath: (optional) the filepath to a PEM encoded RSA account key file.
     :returns: signature
-    :rtype: str
+    :rtype: bytes
     """
     log.info("account_key__sign >")
     if not isinstance(data, bytes):
         data = data.encode()
-    if openssl_crypto:
-        pkey = openssl_crypto.load_privatekey(openssl_crypto.FILETYPE_PEM, key_pem)
-        signature = pkey.to_cryptography_key().sign(
+    # cryptography *should* be installed as a dependency of openssl, but who knows!
+    if openssl_crypto and crypto_rsa and cryptography:
+        pkey: "PKey" = openssl_crypto.load_privatekey(
+            openssl_crypto.FILETYPE_PEM, key_pem
+        )
+        # possible loads are "Union[DSAPrivateKey, DSAPublicKey, RSAPrivateKey, RSAPublicKey]"
+        # but only RSAPublicKey is used or will work
+        # TODO: check to ensure key type is RSAPublicKey
+        signature = pkey.to_cryptography_key().sign(  # type: ignore[union-attr, call-arg]
             data,
-            cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15(),
+            cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15(),  # type: ignore[arg-type]
             cryptography.hazmat.primitives.hashes.SHA256(),
         )
         return signature
     log.debug(".account_key__sign > openssl fallback")
+    if openssl_version is None:
+        check_openssl_version()
     _tmpfile = None
     try:
         if key_pem_filepath is None:
             _tmpfile = new_pem_tempfile(key_pem)
             key_pem_filepath = _tmpfile.name
         with psutil.Popen(
             [openssl_path, "dgst", "-sha256", "-sign", key_pem_filepath],
```

### Comparing `cert_utils-0.1.0/src/cert_utils/model.py` & `cert_utils-0.1.1/src/cert_utils/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # ==============================================================================
 
 
 class _mixin_mapping(object):
     """handles a mapping of db codes/constants"""
 
-    _mapping: Dict
-    _mapping_reverse: Dict
+    _mapping: Dict[int, str]
+    _mapping_reverse: Dict[str, int]
 
     @classmethod
     def as_string(cls, mapping_id: int) -> str:
         if mapping_id in cls._mapping:
             return cls._mapping[mapping_id]
         return "unknown"
 
@@ -42,15 +42,15 @@
         1,
         2,
     )
     _DEFAULT_AcmeAccount: str = "RSA"
     _DEFAULT_GlobalKey: str = "RSA"
     _DEFAULT_AcmeAccount_id: int
     _DEFAULT_GlobalKey_id: int
-    _options_AcmeAccount_private_key_technology: List
+    _options_AcmeAccount_private_key_technology: List[str]
 
 
 # Assign
 
 KeyTechnology._options_AcmeAccount_private_key_technology = [
     KeyTechnology._mapping[_id]
     for _id in KeyTechnology._options_AcmeAccount_private_key_technology_id
```

### Comparing `cert_utils-0.1.0/src/cert_utils/utils.py` & `cert_utils-0.1.1/src/cert_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt_info.py` & `cert_utils-0.1.1/src/cert_utils/letsencrypt_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 Because this loads Certificates into memory for some operations, it should
 generally not be imported.
 """
 
 # stdlib
 import copy
 import os
+from typing import Any
+from typing import Dict
 
 # pypi
 import requests
 
 # localapp
 from .core import cleanup_pem_text
 from .utils import md5_text
@@ -24,15 +26,15 @@
 # ==============================================================================
 
 
 # updated ratelimits are published at:
 # https://letsencrypt.org/docs/rate-limits/
 # last checked: 2020.07.06
 
-LIMITS = {
+LIMITS: Dict[str, Dict[str, Any]] = {
     "names/certificate": {"limit": 100},  # "Names per Certificate"
     "certificates/domain": {
         "limit": 50,
         "timeframe": "1 week",
         "includes_renewals": False,
     },  # "Certificates per Registered Domain"
     "certificates/fqdn": {"limit": 5, "timeframe": "1 week"},  # "Duplicate Certificate"
@@ -128,15 +130,15 @@
     ".enddate": the args to datetime.datetime()
 
 Compatibility Info
     via https://letsencrypt.org/docs/certificate-compatibility/
     Last updated: Jan 21, 2021
 
 """
-CERT_CAS_DATA = {
+CERT_CAS_DATA: Dict[str, Any] = {
     "trustid_root_x3": {
         "display_name": "DST Root CA X3",
         "url_pem": "https://letsencrypt.org/certs/trustid-x3-root.pem",
         "is_trusted_root": True,
         "is_self_signed": True,
         "signed_by": "trustid_root_x3",
         "is_active": True,
@@ -426,20 +428,19 @@
 _dir_here = os.path.abspath(os.path.dirname(__file__))
 _dir_certs = os.path.join(_dir_here, "letsencrypt-certs")
 for cert_id, cert_data in CERT_CAS_DATA.items():
     _filename = cert_data["url_pem"].split("/")[-1]  # type: ignore[attr-defined]
     _filepath = os.path.join(_dir_certs, _filename)
     with open(_filepath, "r") as _fp:
         cert_pem_text = _fp.read()
-        # cert_pem_text = cert_pem_text.decode("utf8")
         cert_pem_text = cleanup_pem_text(cert_pem_text)
         cert_data["cert_pem"] = cert_pem_text
 
 
-def download_letsencrypt_certificates():
+def download_letsencrypt_certificates() -> Dict[str, Any]:
     """
     DEPRECATED
 
     nothing calls this. may be useful for testing to ensure the certs have not
     changed on disk, such as the whitespace issue in 2021/02
 
     download the known LetsEncrypt certificates
@@ -451,13 +452,12 @@
     """
     # ???: raise Exception if the cert_pem changes?
     certs = copy.deepcopy(CERT_CAS_DATA)
     for c in list(certs.keys()):
         resp = requests.get(certs[c]["url_pem"])
         if resp.status_code != 200:
             raise ValueError("Could not load certificate")
-        cert_pem_text = resp.content
-        cert_pem_text = cert_pem_text.decode("utf8")
+        cert_pem_text = resp.text
         cert_pem_text = cleanup_pem_text(cert_pem_text)
         certs[c]["cert_pem"] = cert_pem_text
         certs[c]["cert_pem_md5"] = md5_text(cert_pem_text)
     return certs
```

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/trustid-x3-root.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/fakelerootx1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/fakelerootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrgrootx1.pkix`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/trustid-x3-root.p7c`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/letsencryptauthorityx4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-ocsp-x1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-e1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-e2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrgrootx1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrgrootx1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/fakeleintermediatex1.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r4-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r4.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x2-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-r3.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x1-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/isrg-root-x2.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem` & `cert_utils-0.1.1/src/cert_utils/letsencrypt-certs/lets-encrypt-x3-cross-signed.pem`

 * *Files identical despite different names*

### Comparing `cert_utils-0.1.0/src/cert_utils.egg-info/SOURCES.txt` & `cert_utils-0.1.1/src/cert_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

