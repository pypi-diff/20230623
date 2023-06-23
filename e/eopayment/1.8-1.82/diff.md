# Comparing `tmp/eopayment-1.8.tar.gz` & `tmp/eopayment-1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eopayment-1.8.tar", last modified: Wed Apr 20 15:21:18 2016, max compression
+gzip compressed data, was "eopayment-1.82.tar", last modified: Fri Jun 23 12:27:11 2023, max compression
```

## Comparing `eopayment-1.8.tar` & `eopayment-1.82.tar`

### file list

```diff
@@ -1,41 +1,63 @@
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:21:18.000000 eopayment-1.8/
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:21:18.000000 eopayment-1.8/debian/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        2 2015-05-06 12:46:05.000000 eopayment-1.8/debian/compat
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      620 2015-05-06 12:46:05.000000 eopayment-1.8/debian/control
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      331 2015-05-06 12:46:05.000000 eopayment-1.8/debian/changelog
--rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)      175 2015-05-06 12:46:05.000000 eopayment-1.8/debian/rules
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1036 2015-05-06 12:46:05.000000 eopayment-1.8/debian/copyright
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      144 2016-03-25 13:05:31.000000 eopayment-1.8/MANIFEST.in
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2015 2016-04-20 15:20:54.000000 eopayment-1.8/README.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2875 2016-04-20 15:21:18.000000 eopayment-1.8/PKG-INFO
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:21:18.000000 eopayment-1.8/tests/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2402 2016-04-20 15:09:53.000000 eopayment-1.8/tests/test_ogone.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:09:53.000000 eopayment-1.8/tests/__init__.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      716 2016-04-20 15:09:53.000000 eopayment-1.8/tests/test_spplus.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      598 2016-04-20 15:09:53.000000 eopayment-1.8/tests/test_systempayv2.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4860 2016-04-20 15:09:53.000000 eopayment-1.8/tests/test_paybox.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1074 2016-04-20 15:09:53.000000 eopayment-1.8/tests/test_sips2.py
--rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)     2811 2016-02-01 17:40:46.000000 eopayment-1.8/setup.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       59 2016-04-20 15:21:18.000000 eopayment-1.8/setup.cfg
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:21:18.000000 eopayment-1.8/eopayment/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     8871 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/spplus.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     7815 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/sips2.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     6897 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/dummy.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     5719 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/__init__.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    11258 2016-04-20 15:20:44.000000 eopayment-1.8/eopayment/paybox.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     6969 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/tipi.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     4743 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/common.py
--rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)       19 2015-05-06 12:46:05.000000 eopayment-1.8/eopayment/response
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     1608 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/cb.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     6685 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/sips.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      419 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/payzen.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    18523 2016-04-20 15:20:54.000000 eopayment-1.8/eopayment/systempayv2.py
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)    12005 2016-04-20 15:09:53.000000 eopayment-1.8/eopayment/ogone.py
--rwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)       29 2015-05-06 12:46:05.000000 eopayment-1.8/eopayment/request
-drwxr-xr-x   0 bdauvergne  (1000) bdauvergne  (1000)        0 2016-04-20 15:21:18.000000 eopayment-1.8/eopayment.egg-info/
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       15 2016-04-20 15:21:17.000000 eopayment-1.8/eopayment.egg-info/requires.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      678 2016-04-20 15:21:17.000000 eopayment-1.8/eopayment.egg-info/SOURCES.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)     2875 2016-04-20 15:21:17.000000 eopayment-1.8/eopayment.egg-info/PKG-INFO
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)       10 2016-04-20 15:21:17.000000 eopayment-1.8/eopayment.egg-info/top_level.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)        1 2016-04-20 15:21:17.000000 eopayment-1.8/eopayment.egg-info/dependency_links.txt
--rw-r--r--   0 bdauvergne  (1000) bdauvergne  (1000)      463 2016-02-01 17:40:46.000000 eopayment-1.8/tox.ini
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.393741 eopayment-1.82/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35147 2019-04-10 12:06:55.000000 eopayment-1.82/COPYING
+-rw-r--r--   0 fred      (1000) fred      (1000)      403 2020-11-19 18:31:16.000000 eopayment-1.82/MANIFEST.in
+-rw-r--r--   0 fred      (1000) fred      (1000)    10242 2023-06-23 12:27:11.393741 eopayment-1.82/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     9476 2021-12-25 09:40:38.000000 eopayment-1.82/README.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)        4 2023-06-23 12:27:11.000000 eopayment-1.82/VERSION
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.361741 eopayment-1.82/debian/
+-rw-r--r--   0 fred      (1000) fred      (1000)      158 2020-05-22 07:58:45.000000 eopayment-1.82/debian/changelog
+-rw-r--r--   0 fred      (1000) fred      (1000)      860 2022-10-28 06:12:53.000000 eopayment-1.82/debian/control
+-rw-r--r--   0 fred      (1000) fred      (1000)     1036 2015-04-12 19:55:13.000000 eopayment-1.82/debian/copyright
+-rw-r--r--   0 fred      (1000) fred      (1000)       11 2019-04-10 12:06:55.000000 eopayment-1.82/debian/python-eopayment.docs
+-rw-r--r--   0 fred      (1000) fred      (1000)       11 2019-04-10 12:06:55.000000 eopayment-1.82/debian/python3-eopayment.docs
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      127 2021-12-12 10:59:13.000000 eopayment-1.82/debian/rules
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.373741 eopayment-1.82/eopayment/
+-rw-r--r--   0 fred      (1000) fred      (1000)    11081 2022-10-28 06:06:19.000000 eopayment-1.82/eopayment/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4550 2021-12-12 10:59:13.000000 eopayment-1.82/eopayment/__main__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3157 2021-12-12 10:59:13.000000 eopayment-1.82/eopayment/cb.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7332 2022-10-28 06:12:57.000000 eopayment-1.82/eopayment/common.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7612 2022-12-22 16:18:46.000000 eopayment-1.82/eopayment/dummy.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4919 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/keyware.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.353741 eopayment-1.82/eopayment/locale/
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.357741 eopayment-1.82/eopayment/locale/fr/
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.377741 eopayment-1.82/eopayment/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 fred      (1000) fred      (1000)     3812 2020-11-20 08:57:56.000000 eopayment-1.82/eopayment/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 fred      (1000) fred      (1000)     4759 2023-06-20 12:32:26.000000 eopayment-1.82/eopayment/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 fred      (1000) fred      (1000)     6145 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/mollie.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    15413 2023-02-01 08:46:49.000000 eopayment-1.82/eopayment/ogone.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    17799 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/paybox.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    16855 2022-12-22 16:18:46.000000 eopayment-1.82/eopayment/payfip_ws.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1153 2020-05-22 07:58:45.000000 eopayment-1.82/eopayment/payzen.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.385741 eopayment-1.82/eopayment/resource/
+-rw-r--r--   0 fred      (1000) fred      (1000)     6935 2021-06-24 06:23:56.000000 eopayment-1.82/eopayment/resource/PaiementSecuriseService.wsdl
+-rw-r--r--   0 fred      (1000) fred      (1000)     5482 2020-01-13 20:41:03.000000 eopayment-1.82/eopayment/resource/PaiementSecuriseService1.xsd
+-rw-r--r--   0 fred      (1000) fred      (1000)     1156 2021-06-24 06:23:56.000000 eopayment-1.82/eopayment/resource/PaiementSecuriseService2.xsd
+-rw-r--r--   0 fred      (1000) fred      (1000)     2212 2020-01-13 20:41:03.000000 eopayment-1.82/eopayment/resource/PaiementSecuriseService3.xsd
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       19 2011-04-22 15:28:26.000000 eopayment-1.82/eopayment/response
+-rw-r--r--   0 fred      (1000) fred      (1000)     8536 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/saga.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    14520 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/sips2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    25649 2022-10-28 06:25:56.000000 eopayment-1.82/eopayment/systempayv2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7360 2023-06-20 12:32:26.000000 eopayment-1.82/eopayment/tipi.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.377741 eopayment-1.82/eopayment.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)    10242 2023-06-23 12:27:11.000000 eopayment-1.82/eopayment.egg-info/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     1223 2023-06-23 12:27:11.000000 eopayment-1.82/eopayment.egg-info/SOURCES.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)        1 2023-06-23 12:27:11.000000 eopayment-1.82/eopayment.egg-info/dependency_links.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       44 2023-06-23 12:27:11.000000 eopayment-1.82/eopayment.egg-info/requires.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       10 2023-06-23 12:27:11.000000 eopayment-1.82/eopayment.egg-info/top_level.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-06-23 12:27:11.393741 eopayment-1.82/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     5151 2023-06-20 12:34:34.000000 eopayment-1.82/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-06-23 12:27:11.393741 eopayment-1.82/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2012-06-02 16:45:41.000000 eopayment-1.82/tests/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4051 2021-12-12 10:59:13.000000 eopayment-1.82/tests/conftest.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4616 2021-12-12 10:59:13.000000 eopayment-1.82/tests/test_base_payment.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2975 2022-12-22 16:18:46.000000 eopayment-1.82/tests/test_dummy.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7788 2021-12-12 10:59:13.000000 eopayment-1.82/tests/test_keyware.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6067 2022-10-28 06:06:19.000000 eopayment-1.82/tests/test_misc.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9755 2022-02-02 06:57:25.000000 eopayment-1.82/tests/test_mollie.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5543 2023-02-01 08:46:49.000000 eopayment-1.82/tests/test_ogone.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    16564 2022-10-28 06:25:56.000000 eopayment-1.82/tests/test_paybox.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    17709 2022-12-22 16:18:46.000000 eopayment-1.82/tests/test_payfip_ws.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3315 2021-12-12 10:59:13.000000 eopayment-1.82/tests/test_saga.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4163 2021-12-12 10:59:13.000000 eopayment-1.82/tests/test_sips2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8639 2022-10-28 06:25:56.000000 eopayment-1.82/tests/test_systempayv2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4886 2022-10-28 06:25:56.000000 eopayment-1.82/tests/test_tipi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eopayment-1.8/debian/copyright` & `eopayment-1.82/debian/copyright`

 * *Files identical despite different names*

### Comparing `eopayment-1.8/eopayment/sips2.py` & `eopayment-1.82/eopayment/dummy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,213 +1,232 @@
-# -*- coding: utf-8 -*-
-import collections
-import urlparse
-import string
-from decimal import Decimal
+# eopayment - online payment library
+# Copyright (C) 2011-2020 Entr'ouvert
+#
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+import logging
 import uuid
-import hashlib
-from gettext import gettext as _
 import warnings
+from urllib.parse import parse_qs, urlencode
 
-from common import (PaymentCommon, FORM, Form, PaymentResponse, PAID, ERROR,
-        CANCELED, ResponseError)
+from .common import ERROR, PAID, URL, WAITING, PaymentCommon, PaymentResponse, ResponseError, _, force_text
 
 __all__ = ['Payment']
 
 
+SERVICE_URL = 'https://dummy-payment.entrouvert.com/'
+LOGGER = logging.getLogger(__name__)
+
+
 class Payment(PaymentCommon):
-    '''
-    Payment backend module for the ATOS/SIPS system used by many French banks.
+    """
+    Dummy implementation of the payment interface.
 
-    The necessary options are:
-    - merchant_id
-    - secret_key
-    - normal_return_url
-    - automatic_return_url
-
-    It was writtent using the documentation from file:
-
-        Worldline Benelux_Sips_Technical_integration_guide_Version_1.5.pdf
-
-    '''
-    URL = {
-        'test': 'https://payment-webinit.simu.sips-atos.com/paymentInit',
-        'prod': 'https://payment-webinit.sips-atos.com/paymentInit',
-    }
-    INTERFACE_VERSION = 'HP_2.3'
-    RESPONSE_CODES = {
-        '00': 'Authorisation accepted',
-        '02': 'Authorisation request to be performed via telephone with the issuer, as the '
-              'card authorisation threshold has been exceeded, if the forcing is authorised for '
-              'the merchant',
-        '03': 'Invalid distance selling contract',
-        '05': 'Authorisation refused',
-        '12': 'Invalid transaction, verify the parameters transferred in the request.',
-        '14': 'Invalid bank details or card security code',
-        '17': 'Buyer cancellation',
-        '24': 'Operation impossible. The operation the merchant wishes to perform is not '
-              'compatible with the status of the transaction.',
-        '25': 'Transaction not found in the Sips database',
-        '30': 'Format error',
-        '34': 'Suspicion of fraud',
-        '40': 'Function not supported: the operation that the merchant would like to perform '
-              'is not part of the list of operations for which the merchant is authorised',
-        '51': 'Amount too high',
-        '54': 'Card is past expiry date',
-        '60': 'Transaction pending',
-        '63': 'Security rules not observed, transaction stopped',
-        '75': 'Number of attempts at entering the card number exceeded',
-        '90': 'Service temporarily unavailable',
-        '94': 'Duplicated transaction: for a given day, the TransactionReference has already been '
-              'used',
-        '97': 'Timeframe exceeded, transaction refused',
-        '99': 'Temporary problem at the Sips Office Server level',
-    }
-    TEST_MERCHANT_ID = '002001000000001'
+    It is used with a dummy implementation of a bank payment service that
+    you can find on:
+
+        https://dummy-payment.entrouvert.com/
+
+    You must pass the following keys inside the options dictionnary:
+     - dummy_service_url, the URL of the dummy payment service, it defaults
+       to the one operated by Entr'ouvert.
+     - automatic_return_url: where to POST to notify the service of a
+       payment
+     - origin: a human string to display to the user about the origin of
+       the request.
+     - siret: an identifier for the eCommerce site, fake.
+     - normal_return_url: the return URL for the user (can be overriden on a
+       per request basis).
+    """
 
     description = {
-        'caption': 'SIPS 2',
+        'caption': 'Dummy payment backend',
         'parameters': [
             {
-                'name': 'platform',
-                'caption': _('Platform'),
-                'default': 'test',
-                'choices': ['test', 'prod'],
+                'name': 'normal_return_url',
+                'caption': _('Normal return URL'),
+                'default': '',
                 'required': True,
             },
             {
-                'name': 'merchand_id',
-                'caption': _('Merchant ID'),
-                'default': TEST_MERCHANT_ID,
-                'required': True,
+                'name': 'automatic_return_url',
+                'caption': _('Automatic return URL'),
+                'required': False,
             },
             {
-                'name': 'secret_key',
-                'caption': _('Secret Key'),
-                'default': '002001000000001_KEY1',
-                'required': True,
+                'name': 'dummy_service_url',
+                'caption': _('URL of the dummy payment service'),
+                'default': SERVICE_URL,
+                'type': str,
             },
             {
-                'name': 'key_version',
-                'caption': _('Key Version'),
-                'default': '1',
-                'required': True,
+                'name': 'origin',
+                'caption': _('name of the requesting service, ' 'to present in the user interface'),
+                'type': str,
+                'default': 'origin',
             },
             {
-                'name': 'normal_return_url',
-                'caption': _('Normal return URL'),
-                'default': '',
-                'required': True,
+                'name': 'consider_all_response_signed',
+                'caption': _(
+                    'All response will be considered as signed '
+                    '(to test payment locally for example, as you '
+                    'cannot received the signed callback)'
+                ),
+                'type': bool,
+                'default': False,
             },
             {
-                'name': 'automatic_return_url',
-                'caption': _('Automatic return URL'),
-                'required': False,
+                'name': 'number',
+                'caption': 'dummy integer input test',
+                'type': int,
             },
             {
-                'name': 'currency_code',
-                'caption': _('Currency code'),
-                'default': '978',
-                'choices': ['978'],
-                'required': True,
-            }
+                'name': 'choice',
+                'caption': 'dummy choice input test',
+                'choices': ['a', 'b'],
+            },
+            {
+                'name': 'choices',
+                'caption': 'dummy choices input test',
+                'choices': ['a', 'b'],
+                'type': list,
+            },
+            {
+                'name': 'direct_notification_url',
+                'caption': _('direct notification url (replaced by automatic_return_url)'),
+                'type': str,
+                'deprecated': True,
+            },
+            {
+                'name': 'next_url (replaced by normal_return_url)',
+                'caption': _('Return URL for the user'),
+                'type': str,
+                'deprecated': True,
+            },
+            {
+                'name': 'capture_day',
+                'type': str,
+            },
         ],
     }
 
-    def encode_data(self, data):
-        return u'|'.join(u'%s=%s' % (unicode(key), unicode(value))
-                         for key, value in data.iteritems())
-
-    def seal_data(self, data):
-        s = self.encode_data(data)
-        s += unicode(self.secret_key)
-        s = s.encode('utf-8')
-        s = hashlib.sha256(s).hexdigest()
-        return s
-
-    def get_data(self):
-        data = collections.OrderedDict()
-        data['merchantId'] = self.merchand_id
-        data['keyVersion'] = self.key_version
-        data['normalReturnUrl'] = self.normal_return_url
-        if self.automatic_return_url:
-            data['automaticResponseUrl'] = self.automatic_return_url
-        data['currencyCode'] = self.currency_code
-        return data
-
-    def get_url(self):
-        return self.URL[self.platform]
-
-    def request(self, amount, name=None, address=None, email=None, phone=None,
-                orderid=None, info1=None, info2=None, info3=None, next_url=None, **kwargs):
-        data = self.get_data()
-        transaction_id = self.transaction_id(6, string.digits, 'sips2', data['merchantId'])
-        data['transactionReference'] = unicode(transaction_id)
-        data['orderId'] = orderid or unicode(uuid.uuid4()).replace('-', '')
-        data['amount'] = unicode(int(Decimal(amount) * 100))
-        if email:
-            data['billingContact.email'] = email
+    def request(
+        self,
+        amount,
+        name=None,
+        address=None,
+        email=None,
+        phone=None,
+        orderid=None,
+        info1=None,
+        info2=None,
+        info3=None,
+        next_url=None,
+        capture_day=None,
+        subject=None,
+        **kwargs,
+    ):
+        self.logger.debug(
+            '%s amount %s name %s address %s email %s phone %s'
+            ' next_url %s info1 %s info2 %s info3 %s kwargs: %s',
+            __name__,
+            amount,
+            name,
+            address,
+            email,
+            phone,
+            info1,
+            info2,
+            info3,
+            next_url,
+            kwargs,
+        )
+        transaction_id = str(uuid.uuid4().hex)
         normal_return_url = self.normal_return_url
         if next_url and not normal_return_url:
-            warnings.warn("passing next_url to request() is deprecated, "
-                          "set normal_return_url in options", DeprecationWarning)
+            warnings.warn(
+                "passing next_url to request() is deprecated, " "set normal_return_url in options",
+                DeprecationWarning,
+            )
             normal_return_url = next_url
-        if normal_return_url:
-            data['normalReturnUrl'] = normal_return_url
-        form = Form(
-            url=self.get_url(),
-            method='POST',
-            fields=[
-                {
-                    'type': 'hidden',
-                    'name': 'Data',
-                    'value': self.encode_data(data)
-                },
-                {
-                    'type': 'hidden',
-                    'name': 'Seal',
-                    'value': self.seal_data(data),
-                },
-                {
-                    'type': 'hidden',
-                    'name': 'InterfaceVersion',
-                    'value': self.INTERFACE_VERSION,
-                },
-            ])
-        self.logger.debug('emitting request %r', data)
-        return transaction_id, FORM, form
-
-    def decode_data(self, data):
-        data = data.split('|')
-        data = [map(unicode, p.split('=')) for p in data]
-        return collections.OrderedDict(data)
-
-    def check_seal(self, data, seal):
-        return seal == self.seal_data(data)
-
-    response_code_to_result = {
-        '00': PAID,
-        '17': CANCELED,
-    }
+        automatic_return_url = self.automatic_return_url
+        if self.direct_notification_url and not automatic_return_url:
+            warnings.warn(
+                "direct_notification_url option is deprecated, " "use automatic_return_url",
+                DeprecationWarning,
+            )
+            automatic_return_url = self.direct_notification_url
+        query = {
+            'transaction_id': transaction_id,
+            'amount': amount,
+            'email': email,
+            'return_url': normal_return_url or '',
+            'direct_notification_url': automatic_return_url or '',
+            'origin': self.origin,
+        }
+        query.update(
+            dict(
+                name=name,
+                address=address,
+                email=email,
+                phone=phone,
+                orderid=orderid,
+                info1=info1,
+                info2=info2,
+                info3=info3,
+            )
+        )
+        if capture_day is not None:
+            query['capture_day'] = str(capture_day)
+        if subject is not None:
+            query['subject'] = subject
+        for key in list(query.keys()):
+            if query[key] is None:
+                del query[key]
+        url = '%s?%s' % (SERVICE_URL, urlencode(query))
+        return transaction_id, URL, url
+
+    def response(self, query_string, logger=LOGGER, **kwargs):
+        form = parse_qs(force_text(query_string))
+        if 'transaction_id' not in form:
+            raise ResponseError('missing transaction_id')
+        transaction_id = form.get('transaction_id', [''])[0]
+        form[self.BANK_ID] = transaction_id
+
+        signed = 'signed' in form
+        if signed:
+            content = 'signature ok'
+        else:
+            content = None
+        signed = signed or self.consider_all_response_signed
+        result = PAID if 'ok' in form else ERROR
+        if 'waiting' in form:
+            result = WAITING
 
-    def response(self, query_string, **kwargs):
-        form = urlparse.parse_qs(query_string)
-        if not set(form) >= set(['Data', 'Seal', 'InterfaceVersion']):
-            raise ResponseError()
-        self.logger.debug('received query string %r', form)
-        data = self.decode_data(form['Data'][0])
-        seal = form['Seal'][0]
-        self.logger.debug('parsed response %r seal %r', data, seal)
-        signed = self.check_seal(data, seal)
-        response_code = data['responseCode']
-        transaction_id = data.get('transactionReference')
-        result = self.response_code_to_result.get(response_code, ERROR)
-        merchant_id = data.get('merchantId')
-        test = merchant_id == self.TEST_MERCHANT_ID
-        return PaymentResponse(
+        response = PaymentResponse(
             result=result,
             signed=signed,
-            bank_data=data,
+            bank_data=form,
+            return_content=content,
             order_id=transaction_id,
-            transaction_id=data.get('authorisationId'),
-            bank_status=self.RESPONSE_CODES.get(response_code, u'unknown code - ' + response_code),
-            test=test)
+            transaction_id=transaction_id,
+            bank_status=form.get('reason'),
+            test=True,
+        )
+        return response
+
+    def validate(self, amount, bank_data, **kwargs):
+        return {}
+
+    def cancel(self, amount, bank_data, **kwargs):
+        return {}
```

### Comparing `eopayment-1.8/eopayment/tipi.py` & `eopayment-1.82/eopayment/tipi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,184 @@
-# -*- coding: utf-8 -*-
+# eopayment - online payment library
+# Copyright (C) 2011-2020 Entr'ouvert
+#
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from decimal import Decimal, ROUND_DOWN
-from common import (PaymentCommon, PaymentResponse, URL, PAID, DENIED,
-        CANCELLED, ERROR, ResponseError)
-from urllib import urlencode
-from urlparse import parse_qs
-from gettext import gettext as _
+import datetime
+import decimal
 import logging
+import random
+import re
 import warnings
+from urllib.parse import parse_qs, urlencode
 
-from systempayv2 import isonow
+import pytz
+
+from .common import CANCELLED, DENIED, ERROR, PAID, URL, PaymentCommon, PaymentResponse, ResponseError, _
 
 __all__ = ['Payment']
 
-TIPI_URL = 'http://www.jepaiemesserviceslocaux.dgfip.finances.gouv.fr' \
-        '/tpa/paiement.web'
+TIPI_URL = 'https://www.payfip.gouv.fr/tpa/paiement.web'
 LOGGER = logging.getLogger(__name__)
 
+
 class Payment(PaymentCommon):
-    '''Produce requests for and verify response from the TIPI online payment
+    """Produce requests for and verify response from the TIPI online payment
     processor from the French Finance Ministry.
 
-    '''
+    """
 
     description = {
-            'caption': 'TIPI, Titres Payables par Internet',
-            'parameters': [
-                {
-                    'name': 'numcli',
-                    'caption': _(u'Numéro client'),
-                    'help_text': _(u'un numéro à 6 chiffres communiqué par l’administrateur TIPI'),
-                    'validation': lambda s: str.isdigit(s) and (0 < int(s) < 1000000),
-                    'required': True,
-                },
-                {
-                    'name': 'service_url',
-                    'default': TIPI_URL,
-                    'caption': _(u'URL du service TIPI'),
-                    'help_text': _(u'ne pas modifier si vous ne savez pas'),
-                    'validation': lambda x: x.startswith('http'),
-                    'required': True,
-                },
-                {
-                    'name': 'normal_return_url',
-                    'caption': _('Normal return URL (unused by TIPI)'),
-                    'required': False,
-                },
-                {
-                    'name': 'automatic_return_url',
-                    'caption': _('Automatic return URL'),
-                    'required': True,
-                },
-            ],
+        'caption': 'TIPI, Titres Payables par Internet',
+        'parameters': [
+            {
+                'name': 'numcli',
+                'caption': _('Client number'),
+                'help_text': _('6 digits number provided by DGFIP'),
+                'validation': lambda s: str.isdigit(s) and (0 < int(s) < 1000000),
+                'required': True,
+            },
+            {
+                'name': 'normal_return_url',
+                'caption': _('Normal return URL (unused by TIPI)'),
+                'required': False,
+            },
+            {
+                'name': 'automatic_return_url',
+                'caption': _('Automatic return URL'),
+                'required': True,
+            },
+            {
+                'name': 'saisie',
+                'caption': _('Payment type'),
+                'required': True,
+                'default': 'T',
+                'choices': [
+                    ('T', _('test')),
+                    ('X', _('activation')),
+                    ('A', _('production')),
+                ],
+            },
+        ],
     }
 
-    def request(self, amount, next_url=None, exer=None, orderid=None,
-            refdet=None, objet=None, email=None, saisie=None, **kwargs):
-        try:
-            montant = Decimal(amount)
-            if Decimal('0') > montant > Decimal('9999.99'):
-                raise ValueError('MONTANT > 9999.99 euros')
-            montant = montant*Decimal('100')
-            montant = montant.to_integral_value(ROUND_DOWN)
-        except ValueError:
-            raise ValueError('MONTANT invalid format, must be '
-                    'a decimal integer with less than 4 digits '
-                    'before and 2 digits after the decimal point '
-                    ', here it is %s' % repr(amount))
+    REFDET_RE = re.compile('^[a-zA-Z0-9]{6,30}$')
+
+    minimal_amount = decimal.Decimal('1.0')
+    maximal_amount = decimal.Decimal('100000.0')
+
+    def _generate_refdet(self):
+        return '%s%010d' % (
+            datetime.datetime.now(pytz.timezone('Europe/Paris')).strftime('%Y%m%d%H%M%S'),
+            random.randint(1, 1000000000),
+        )
+
+    def request(
+        self,
+        amount,
+        email,
+        next_url=None,
+        exer=None,
+        orderid=None,
+        refdet=None,
+        objet=None,
+        saisie=None,
+        **kwargs,
+    ):
+        montant = self.clean_amount(amount, max_amount=9999.99)
 
         automatic_return_url = self.automatic_return_url
         if next_url and not automatic_return_url:
-            warnings.warn("passing next_url to request() is deprecated, "
-                          "set automatic_return_url in options", DeprecationWarning)
+            warnings.warn(
+                "passing next_url to request() is deprecated, " "set automatic_return_url in options",
+                DeprecationWarning,
+            )
             automatic_return_url = next_url
         if automatic_return_url is not None:
-            if not isinstance(automatic_return_url, str) or \
-                not automatic_return_url.startswith('http'):
+            if not isinstance(automatic_return_url, str) or not automatic_return_url.startswith('http'):
                 raise ValueError('URLCL invalid URL format')
         try:
             if exer is not None:
                 exer = int(exer)
                 if exer > 9999:
                     raise ValueError()
         except ValueError:
             raise ValueError('EXER format invalide')
-        try:
-            refdet = orderid or refdet
-            refdet = str(refdet)
-            if 6 > len(refdet) > 30:
-                raise ValueError('len(REFDET) < 6 or > 30')
-        except Exception, e:
-            raise ValueError('REFDET format invalide, %r' % refdet, e)
+        assert not (orderid and refdet), 'orderid and refdet cannot be used together'
+        # check or generate refdet
+        if refdet:
+            try:
+                if not self.REFDET_RE.match(refdet):
+                    raise ValueError
+            except (TypeError, ValueError):
+                raise ValueError('refdet must be 6 to 30 alphanumeric characters string')
+        if orderid:
+            if self.REFDET_RE.match(orderid):
+                refdet = orderid
+            else:
+                objet = orderid + (' ' + objet) if objet else ''
+        if not refdet:
+            refdet = self._generate_refdet()
+        transaction_id = refdet
+        # check objet or fix objet
         if objet is not None:
             try:
-                objet = str(objet)
-            except Exception, e:
-                raise ValueError('OBJET must be a string', e)
-            if not objet.replace(' ','').isalnum():
-                raise ValueError('OBJECT must only contains '
-                        'alphanumeric characters, %r' % objet)
-            if len(objet) > 99:
-                raise ValueError('OBJET length must be less than 100')
+                objet = objet.encode('ascii')
+            except Exception as e:
+                raise ValueError('OBJET must be an alphanumeric string', e)
         try:
             mel = str(email)
             if '@' not in mel:
                 raise ValueError('no @ in MEL')
             if not (6 <= len(mel) <= 80):
                 raise ValueError('len(MEL) is invalid, must be between 6 and 80')
-        except Exception, e:
+        except Exception as e:
             raise ValueError('MEL is not a valid email, %r' % mel, e)
 
+        # check saisie
+        saisie = saisie or self.saisie
         if saisie not in ('M', 'T', 'X', 'A'):
             raise ValueError('SAISIE invalid format, %r, must be M, T, X or A' % saisie)
 
-        iso_now = isonow()
-        transaction_id = '%s_%s' % (iso_now, refdet)
-        if objet:
-            objet = objet[:100-len(iso_now)-2] + ' ' + iso_now
-        else:
-            objet = iso_now
         params = {
-                'numcli': self.numcli,
-                'refdet': refdet,
-                'montant': montant,
-                'mel': mel,
-                'saisie': saisie,
-                'objet': objet,
+            'numcli': self.numcli,
+            'refdet': refdet,
+            'montant': montant,
+            'mel': mel,
+            'saisie': saisie,
         }
         if exer:
             params['exer'] = exer
+        if objet:
+            params['objet'] = objet
         if automatic_return_url:
             params['urlcl'] = automatic_return_url
-        url = '%s?%s' % (self.service_url, urlencode(params))
+        url = '%s?%s' % (TIPI_URL, urlencode(params))
         return transaction_id, URL, url
 
     def response(self, query_string, **kwargs):
         fields = parse_qs(query_string, True)
-        if not set(fields) >= set(['refdet', 'resultrans']):
-            raise ResponseError()
-        for key, value in fields.iteritems():
+        if not set(fields) >= {'refdet', 'resultrans'}:
+            raise ResponseError('missing refdet or resultrans')
+        for key, value in fields.items():
             fields[key] = value[0]
         refdet = fields.get('refdet')
         if refdet is None:
-            raise ValueError('refdet is missing')
-        if 'objet' in fields:
-            iso_now = fields['objet']
-        else:
-            iso_now = isonow()
-        transaction_id = '%s_%s' % (iso_now, refdet)
+            raise ResponseError('refdet is missing')
 
         result = fields.get('resultrans')
         if result == 'P':
             result = PAID
             bank_status = ''
         elif result == 'R':
             result = DENIED
@@ -162,24 +189,29 @@
         else:
             bank_status = 'wrong return: %r' % result
             result = ERROR
 
         test = fields.get('saisie') == 'T'
 
         return PaymentResponse(
-                result=result,
-                bank_status=bank_status,
-                signed=True,
-                bank_data=fields,
-                transaction_id=transaction_id,
-                test=test)
-
-if __name__ == '__main__':
-    p = Payment({'numcli': '12345'})
-    print p.request(amount=Decimal('123.12'),
-            exer=9999,
-            refdet=999900000000999999,
-            objet='tout a fait',
-            email='info@entrouvert.com',
-            urlcl='http://example.com/tipi/test',
-            saisie='T')
-    print p.response('objet=tout+a+fait&montant=12312&saisie=T&mel=info%40entrouvert.com&numcli=12345&exer=9999&refdet=999900000000999999&resultrans=P')
+            result=result,
+            bank_status=bank_status,
+            signed=True,
+            bank_data=fields,
+            order_id=refdet,
+            transaction_id=refdet,
+            test=test,
+        )
+
+    @classmethod
+    def guess(self, *, method=None, query_string=None, body=None, headers=None, backends=(), **kwargs):
+        for content in [query_string, body]:
+            if isinstance(content, bytes):
+                try:
+                    content = content.decode()
+                except UnicodeDecodeError:
+                    pass
+            if isinstance(content, str):
+                fields = parse_qs(content)
+                if 'refdet' in fields and 'resultrans' in fields:
+                    return fields['refdet'][0]
+        return None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eopayment-1.8/eopayment/ogone.py` & `eopayment-1.82/eopayment/ogone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,53 @@
-# -*- coding: utf-8 -*-
+# eopayment - online payment library
+# Copyright (C) 2011-2020 Entr'ouvert
+#
+# This program is free software: you can redistribute it and/or modify it
+# under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 import hashlib
-import string
-import urlparse
-from decimal import Decimal, ROUND_HALF_UP
-
-from common import (PaymentCommon, PaymentResponse, FORM, CANCELLED, PAID,
-        ERROR, Form, DENIED, ACCEPTED, ORDERID_TRANSACTION_SEPARATOR,
-        ResponseError)
-def N_(message): return message
+import uuid
+from decimal import ROUND_HALF_UP, Decimal
+from urllib import parse as urlparse
+
+from .common import (
+    ACCEPTED,
+    CANCELLED,
+    DENIED,
+    ERROR,
+    FORM,
+    ORDERID_TRANSACTION_SEPARATOR,
+    PAID,
+    WAITING,
+    Form,
+    PaymentCommon,
+    PaymentResponse,
+    ResponseError,
+    _,
+    force_byte,
+    force_text,
+)
 
 ENVIRONMENT_TEST = 'TEST'
 ENVIRONMENT_TEST_URL = 'https://secure.ogone.com/ncol/test/orderstandard.asp'
 ENVIRONMENT_PROD = 'PROD'
 ENVIRONMENT_PROD_URL = 'https://secure.ogone.com/ncol/prod/orderstandard.asp'
 ENVIRONMENT = [ENVIRONMENT_TEST, ENVIRONMENT_PROD]
 
+# https://payment-services.ingenico.com/ogone/support/~/media/kdb/integration%20guides/sha-in_params.ashx
 SHA_IN_PARAMS = """
 ACCEPTANCE
 ACCEPTURL
 ADDMATCH
 ADDRMATCH
 AIACTIONNUMBER
 AIAGIATA
@@ -334,16 +363,18 @@
 USERTYPE
 VERSION
 WBTU_MSISDN
 WBTU_ORDERID
 WEIGHTUNIT
 WIN3DS
 WITHROOT
+XDL
 """.split()
 
+# https://payment-services.ingenico.com/ogone/support/~/media/kdb/integration%20guides/sha-out_params.ashx
 SHA_OUT_PARAMS = """
 AAVADDRESS
 AAVCHECK
 AAVMAIL
 AAVNAME
 AAVPHONE
 AAVZIP
@@ -387,179 +418,248 @@
 NBREMAILUSAGE
 NBRIPUSAGE
 NBRIPUSAGE_ALLTX
 NBRUSAGE
 NCERROR
 ORDERID
 PAYID
+PAYIDSUB
 PAYMENT_REFERENCE
 PM
 SCO_CATEGORY
 SCORING
 SEQUENCETYPE
 SIGNDATE
 STATUS
 SUBBRAND
 SUBSCRIPTION_ID
 TRXDATE
-VC"""
+VC
+""".split()
+
 
 class Payment(PaymentCommon):
     # See http://payment-services.ingenico.com/fr/fr/ogone/support/guides/integration%20guides/e-commerce
     description = {
-        'caption': N_('Système de paiement Ogone / Ingenico Payment System e-Commerce'),
+        'caption': _('Ogone / Ingenico Payment System e-Commerce'),
         'parameters': [
             {
                 'name': 'normal_return_url',
-                'caption': N_('Normal return URL'),
+                'caption': _('Normal return URL'),
                 'default': '',
                 'required': True,
             },
             {
                 'name': 'automatic_return_url',
-                'caption': N_('Automatic return URL (ignored, must be set in Ogone backoffice)'),
+                'caption': _('Automatic return URL (ignored, must be set in Ogone backoffice)'),
                 'required': False,
             },
-            {'name': 'environment',
+            {
+                'name': 'environment',
                 'default': ENVIRONMENT_TEST,
-                'caption': N_(u'Environnement'),
+                'caption': 'Environnement',
                 'choices': ENVIRONMENT,
             },
-            {'name': 'pspid',
-                'caption': N_(u"Nom d'affiliation dans le système"),
+            {
+                'name': 'pspid',
+                'caption': "Nom d'affiliation dans le système",
                 'required': True,
             },
-            {'name': 'language',
-                'caption': N_(u'Langage'),
+            {
+                'name': 'language',
+                'caption': _('Language'),
                 'default': 'fr_FR',
-                'choices': (('fr_FR', N_('français')),),
+                'choices': (('fr_FR', 'français'),),
+            },
+            {
+                'name': 'encoding',
+                'caption': _('Characters encoding'),
+                'default': 'utf-8',
+                'choices': [
+                    ('iso-8859-1', 'Latin1 (ISO-8859-1)'),
+                    ('utf-8', 'Unicode (UTF-8)'),
+                ],
             },
-            {'name': 'hash_algorithm',
-                'caption': N_(u'Algorithme de hachage'),
+            {
+                'name': 'hash_algorithm',
+                'caption': 'Algorithme de hachage',
                 'default': 'sha1',
             },
-            {'name': 'sha_in',
-                'caption': N_(u'Clé SHA-IN'),
+            {
+                'name': 'sha_in',
+                'caption': 'Clé SHA-IN',
                 'required': True,
             },
-            {'name': 'sha_out',
-                'caption': N_(u'Clé SHA-OUT'),
+            {
+                'name': 'sha_out',
+                'caption': 'Clé SHA-OUT',
                 'required': True,
             },
-            {'name': 'currency',
-                'caption': N_(u'Monnaie'),
+            {
+                'name': 'currency',
+                'caption': 'Monnaie',
                 'default': 'EUR',
                 'choices': ('EUR',),
             },
-        ]
+        ],
     }
 
-    def sha_sign(self, algo, key, params, keep):
+    def __init__(self, options, logger=None):
+        # retro-compatibility with old default of latin1
+        options.setdefault('encoding', 'iso-8859-1')
+        super().__init__(options, logger=logger)
+
+    def sha_sign(self, algo, key, params, keep, encoding='iso-8859-1'):
         '''Ogone signature algorithm of query string'''
         values = params.items()
         values = [(a.upper(), b) for a, b in values]
         values = sorted(values)
-        values = ['%s=%s' % (a, b) for a, b in values if a in keep]
+        values = ['%s=%s' % (a, b) for a, b in values if a in keep and b]
         tosign = key.join(values)
         tosign += key
+        tosign = force_byte(tosign, encoding=encoding)
         hashing = getattr(hashlib, algo)
         return hashing(tosign).hexdigest().upper()
 
-    def sha_sign_in(self, params):
-        return self.sha_sign(self.hash_algorithm, self.sha_in, params, SHA_IN_PARAMS)
+    def sha_sign_in(self, params, encoding='iso-8859-1'):
+        return self.sha_sign(self.hash_algorithm, self.sha_in, params, SHA_IN_PARAMS, encoding=encoding)
 
-    def sha_sign_out(self, params):
-        return self.sha_sign(self.hash_algorithm, self.sha_out, params, SHA_OUT_PARAMS)
+    def sha_sign_out(self, params, encoding='iso-8859-1'):
+        return self.sha_sign(self.hash_algorithm, self.sha_out, params, SHA_OUT_PARAMS, encoding=encoding)
 
     def get_request_url(self):
         if self.environment == ENVIRONMENT_TEST:
             return ENVIRONMENT_TEST_URL
         if self.environment == ENVIRONMENT_PROD:
             return ENVIRONMENT_PROD_URL
         raise NotImplementedError('unknown environment %s' % self.environment)
 
-    def request(self, amount, orderid=None, name=None, email=None,
-            language=None, description=None, **kwargs):
+    def request(
+        self,
+        amount,
+        orderid=None,
+        name=None,
+        email=None,
+        language=None,
+        description=None,
+        transaction_id=None,
+        **kwargs,
+    ):
+        # use complus for transmitting and receiving the transaction_id see
+        # https://epayments-support.ingenico.com/fr/integration/all-sales-channels/integrate-with-e-commerce/guide#variable-feedback-parameters
+        # orderid is now only used for unicity of payments check (it's
+        # garanteed that no payment for the same ORDERID can happen during a 45
+        # days window, see
+        # https://epayments-support.ingenico.com/fr/integration/all-sales-channels/integrate-with-e-commerce/guide#form-parameters)
+        complus = transaction_id or uuid.uuid4().hex
+        if not orderid:
+            orderid = complus
 
-        reference = self.transaction_id(20, string.digits + string.ascii_letters)
-
-        # prepend order id in payment reference
-        if orderid:
-            if len(orderid) > 24:
-                raise ValueError('orderid length exceeds 25 characters')
-            reference = orderid + ORDERID_TRANSACTION_SEPARATOR + self.transaction_id(29-len(orderid), string.digits + string.ascii_letters)
         language = language or self.language
         # convertir en centimes
         amount = Decimal(amount) * 100
         # arrondi comptable francais
         amount = amount.quantize(Decimal('1.'), rounding=ROUND_HALF_UP)
         params = {
-                'AMOUNT': amount,
-                'ORDERID': reference,
-                'PSPID': self.pspid,
-                'LANGUAGE': language,
-                'CURRENCY': self.currency,
+            'AMOUNT': force_text(amount),
+            'ORDERID': orderid,
+            'PSPID': self.pspid,
+            'LANGUAGE': language,
+            'CURRENCY': self.currency,
+            'COMPLUS': complus,
         }
         if self.normal_return_url:
             params['ACCEPTURL'] = self.normal_return_url
             params['BACKURL'] = self.normal_return_url
             params['CANCELURL'] = self.normal_return_url
             params['DECLINEURL'] = self.normal_return_url
             params['EXCEPTIONURL'] = self.normal_return_url
         if name:
             params['CN'] = name
         if email:
             params['EMAIL'] = email
         if description:
             params['COM'] = description
-        for key, value in kwargs.iteritems():
+        for key, value in kwargs.items():
             params[key.upper()] = value
+        params['SHASIGN'] = self.sha_sign_in(params)
         # uniformize all values to UTF-8 string
         for key in params:
-            params[key] = unicode(params[key]).encode('utf-8')
-        params['SHASIGN'] = self.sha_sign_in(params)
+            params[key] = force_text(params[key])
         url = self.get_request_url()
         form = Form(
-                url=url,
-                method='POST',
-                fields=[{'type': 'hidden',
-                         'name': key,
-                         'value': params[key]} for key in params])
-        return reference, FORM, form
+            url=url,
+            method='POST',
+            fields=[{'type': 'hidden', 'name': key, 'value': params[key]} for key in params],
+        )
+        return complus, FORM, form
 
     def response(self, query_string, **kwargs):
-        params = urlparse.parse_qs(query_string, True)
-        params = dict((key.upper(), params[key][0]) for key in params)
-        if not set(params) >= set(['ORDERID', 'PAYID', 'STATUS', 'NCERROR']):
-            raise ResponseError()
-        reference = params['ORDERID']
+        params = urlparse.parse_qs(query_string, True, encoding=self.encoding)
+        params = {key.upper(): params[key][0] for key in params}
+        if not set(params) >= {'ORDERID', 'PAYID', 'STATUS', 'NCERROR'}:
+            raise ResponseError('missing ORDERID, PAYID, STATUS or NCERROR')
+
+        # py2: decode binary strings in query-string
+        for key in params:
+            params[key] = force_text(params[key], self.encoding)
+        orderid = params['ORDERID']
+        complus = params.get('COMPLUS')
         transaction_id = params['PAYID']
         status = params['STATUS']
         error = params['NCERROR']
         signed = False
         if self.sha_in:
             signature = params.get('SHASIGN')
-            expected_signature = self.sha_sign_out(params)
-            signed = signature == expected_signature
-            print 'signed', signature
-            print 'expected', expected_signature
+            # check signature against both encoding
+            for encoding in ('iso-8859-1', 'utf-8'):
+                expected_signature = self.sha_sign_out(params, encoding=encoding)
+                signed = signature == expected_signature
+                if signed:
+                    break
         if status == '1':
             result = CANCELLED
         elif status == '2':
             result = DENIED
         elif status == '5':
             result = ACCEPTED
-        elif status == '9':
+        elif status in ('9', '95'):
             result = PAID
+        elif len(status) == 2 and status[1] == '1':
+            # Statuses with two digits represent either ‘intermediary'
+            # situations or abnormal events. When the second digit is:
+            # 1, this means the payment processing is on hold. (e.g.
+            # status 91: payment waiting/pending)
+            result = WAITING
         else:
-            self.logger.error('response STATUS=%s NCERROR=%s NCERRORPLUS=%s',
-                    status, error, params.get('NCERRORPLUS', ''))
+            self.logger.error(
+                'response STATUS=%s NCERROR=%s NCERRORPLUS=%s', status, error, params.get('NCERRORPLUS', '')
+            )
             result = ERROR
         # extract reference from received order id
-        if ORDERID_TRANSACTION_SEPARATOR in reference:
-            reference, transaction_id = reference.split(ORDERID_TRANSACTION_SEPARATOR, 1)
+
         return PaymentResponse(
-                result=result,
-                signed=signed,
-                bank_data=params,
-                order_id=reference,
-                transaction_id=transaction_id)
+            result=result,
+            signed=signed,
+            bank_data=params,
+            order_id=complus or orderid,
+            transaction_id=transaction_id,
+        )
+
+    @classmethod
+    def guess(self, *, method=None, query_string=None, body=None, headers=None, backends=(), **kwargs):
+        for content in [query_string, body]:
+            if isinstance(content, bytes):
+                try:
+                    content = content.decode()
+                except UnicodeDecodeError:
+                    pass
+            if isinstance(content, str):
+                fields = {key.upper(): values for key, values in urlparse.parse_qs(content).items()}
+                if not set(fields) >= {'ORDERID', 'PAYID', 'STATUS', 'NCERROR'}:
+                    continue
+                orderid = fields.get('ORDERID')
+                complus = fields.get('COMPLUS')
+                if complus:
+                    return complus[0]
+                return orderid[0]
+        return None
```

### Comparing `eopayment-1.8/eopayment.egg-info/SOURCES.txt` & `eopayment-1.82/eopayment.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+COPYING
 MANIFEST.in
 README.txt
+VERSION
 setup.py
-tox.ini
 debian/changelog
-debian/compat
 debian/control
 debian/copyright
+debian/python-eopayment.docs
+debian/python3-eopayment.docs
 debian/rules
 eopayment/__init__.py
+eopayment/__main__.py
 eopayment/cb.py
 eopayment/common.py
 eopayment/dummy.py
+eopayment/keyware.py
+eopayment/mollie.py
 eopayment/ogone.py
 eopayment/paybox.py
+eopayment/payfip_ws.py
 eopayment/payzen.py
-eopayment/request
 eopayment/response
-eopayment/sips.py
+eopayment/saga.py
 eopayment/sips2.py
-eopayment/spplus.py
 eopayment/systempayv2.py
 eopayment/tipi.py
 eopayment.egg-info/PKG-INFO
 eopayment.egg-info/SOURCES.txt
 eopayment.egg-info/dependency_links.txt
 eopayment.egg-info/requires.txt
 eopayment.egg-info/top_level.txt
+eopayment/locale/fr/LC_MESSAGES/django.mo
+eopayment/locale/fr/LC_MESSAGES/django.po
+eopayment/resource/PaiementSecuriseService.wsdl
+eopayment/resource/PaiementSecuriseService1.xsd
+eopayment/resource/PaiementSecuriseService2.xsd
+eopayment/resource/PaiementSecuriseService3.xsd
 tests/__init__.py
+tests/conftest.py
+tests/test_base_payment.py
+tests/test_dummy.py
+tests/test_keyware.py
+tests/test_misc.py
+tests/test_mollie.py
 tests/test_ogone.py
 tests/test_paybox.py
+tests/test_payfip_ws.py
+tests/test_saga.py
 tests/test_sips2.py
-tests/test_spplus.py
-tests/test_systempayv2.py
+tests/test_systempayv2.py
+tests/test_tipi.py
```

