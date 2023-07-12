# Comparing `tmp/dkb_robo-0.8.3.tar.gz` & `tmp/dkb_robo-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dkb_robo-0.8.3.tar", last modified: Thu Aug 29 19:29:19 2019, max compression
+gzip compressed data, was "dist\dkb_robo-0.9.tar", last modified: Sun Mar 29 06:46:40 2020, max compression
```

## Comparing `dkb_robo-0.8.3.tar` & `dkb_robo-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/
-drwxrwxrwx   0        0        0        0 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/dkb_robo/
--rw-rw-rw-   0        0        0    24099 2019-08-29 19:25:02.000000 dkb_robo-0.8.3/dkb_robo/dkb_robo.py
--rw-rw-rw-   0        0        0       29 2018-02-05 07:44:13.000000 dkb_robo-0.8.3/dkb_robo/__init__.py
-drwxrwxrwx   0        0        0        0 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/dkb_robo.egg-info/
--rw-rw-rw-   0        0        0        1 2019-08-29 19:29:18.000000 dkb_robo-0.8.3/dkb_robo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-02-18 06:56:46.000000 dkb_robo-0.8.3/dkb_robo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      715 2019-08-29 19:29:18.000000 dkb_robo-0.8.3/dkb_robo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       32 2019-08-29 19:29:18.000000 dkb_robo-0.8.3/dkb_robo.egg-info/requires.txt
--rw-rw-rw-   0        0        0      272 2019-08-29 19:29:18.000000 dkb_robo-0.8.3/dkb_robo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2019-08-29 19:29:18.000000 dkb_robo-0.8.3/dkb_robo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      715 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     7171 2019-08-29 10:06:53.000000 dkb_robo-0.8.3/README.md
--rw-rw-rw-   0        0        0       42 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0      962 2019-08-29 19:27:26.000000 dkb_robo-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2019-08-29 19:29:19.000000 dkb_robo-0.8.3/test/
--rw-rw-rw-   0        0        0    20011 2019-08-29 19:25:46.000000 dkb_robo-0.8.3/test/test_dkb_robo.py
+drwxrwxrwx   0        0        0        0 2020-03-29 06:46:40.102241 dkb_robo-0.9/
+-rw-rw-rw-   0        0        0      713 2020-03-29 06:46:40.102241 dkb_robo-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8236 2020-03-29 06:40:26.000000 dkb_robo-0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-03-29 06:46:40.039742 dkb_robo-0.9/dkb_robo/
+-rw-rw-rw-   0        0        0       29 2018-02-05 07:44:13.000000 dkb_robo-0.9/dkb_robo/__init__.py
+-rw-rw-rw-   0        0        0    30075 2020-03-29 06:40:26.000000 dkb_robo-0.9/dkb_robo/dkb_robo.py
+drwxrwxrwx   0        0        0        0 2020-03-29 06:46:40.055366 dkb_robo-0.9/dkb_robo.egg-info/
+-rw-rw-rw-   0        0        0      713 2020-03-29 06:46:39.000000 dkb_robo-0.9/dkb_robo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2020-03-29 06:46:40.000000 dkb_robo-0.9/dkb_robo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-03-29 06:46:39.000000 dkb_robo-0.9/dkb_robo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-02-18 06:56:46.000000 dkb_robo-0.9/dkb_robo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2020-03-29 06:46:39.000000 dkb_robo-0.9/dkb_robo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2020-03-29 06:46:39.000000 dkb_robo-0.9/dkb_robo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-03-29 06:46:40.102241 dkb_robo-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      960 2020-03-29 06:40:26.000000 dkb_robo-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-03-29 06:46:40.055366 dkb_robo-0.9/test/
+-rw-rw-rw-   0        0        0    20011 2019-08-29 19:37:20.000000 dkb_robo-0.9/test/test_dkb_robo.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dkb_robo-0.8.3/dkb_robo/dkb_robo.py` & `dkb_robo-0.9/dkb_robo/dkb_robo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """ dkb internet banking automation library """
 
 from __future__ import print_function
 import sys
 import csv
+import random
+import time
 from datetime import datetime
 import re
+from string import digits, ascii_letters
 import mechanicalsoup
-# from bs4 import BeautifulSoup
 
 if sys.version_info > (3, 0):
     import http.cookiejar as cookielib
     import importlib
     importlib.reload(sys)
 else:
     import cookielib
     reload(sys)
     sys.setdefaultencoding('utf8')
 
+def generate_random_string(length):
+    """ generate random string to be used as name """
+    char_set = digits + ascii_letters
+    return ''.join(random.choice(char_set) for _ in range(length))
+
+def print_debug(debug, text):
+    """ little helper to print debug messages """
+    if debug:
+        print('{0}: {1}'.format(datetime.now(), text))
+
 class DKBRobo(object):
     """ dkb_robo class """
 
     base_url = 'https://www.dkb.de'
     dkb_user = None
     dkb_password = None
     dkb_br = None
     last_login = None
     account_dic = {}
+    chip_tan = False
+    debug = False
 
-    def __init__(self, dkb_user=None, dkb_password=None):
+    def __init__(self, dkb_user=None, dkb_password=None, chip_tan=False, debug=False):
         self.dkb_user = dkb_user
         self.dkb_password = dkb_password
+        self.chip_tan = chip_tan
+        self.debug = debug
 
     def __enter__(self):
         """
         Makes DKBRobo a Context Manager
 
         with DKBRobo("user","pwd") as dkb:
             print (dkb.lastlogin)
@@ -54,14 +70,15 @@
         """ get transactions from an regular account for a certain amount of time
         args:
             self.dkb_br          - browser object
             transaction_url - link to collect the transactions
             date_from       - transactions starting form
             date_to         - end date
         """
+        print_debug(self.debug, 'DKBRobo.get_account_transactions({0}: {1}/{2})\n'.format(transaction_url, date_from, date_to))
         self.dkb_br.open(transaction_url)
         self.dkb_br.select_form('#form1615473160_1')
 
         self.dkb_br["slTransactionStatus"] = 0
         self.dkb_br["searchPeriodRadio"] = 1
         self.dkb_br["slSearchPeriod"] = 1
         self.dkb_br["transactionDate"] = str(date_from)
@@ -75,14 +92,15 @@
         """ get transactions from an regular account for a certain amount of time
         args:
             self.dkb_br          - browser object
             transaction_url - link to collect the transactions
             date_from       - transactions starting form
             date_to         - end date
         """
+        print_debug(self.debug, 'DKBRobo.get_creditcard_transactions({0}: {1}/{2})\n'.format(transaction_url, date_from, date_to))
         # get credit card transaction form yesterday
         self.dkb_br.open(transaction_url)
         self.dkb_br.select_form('#form1579108072_1')
 
         self.dkb_br["slSearchPeriod"] = 0
         self.dkb_br["filterType"] = 'DATE_RANGE'
         self.dkb_br["postingDate"] = str(date_from)
@@ -97,14 +115,15 @@
 
         args:
             self.dkb_br - browser object
 
         returns:
             dictionary of the accounts and limits
         """
+        print_debug(self.debug, 'DKBRobo.get_credit_limits()\n')
         limit_url = self.base_url + '/DkbTransactionBanking/content/service/CreditcardLimit.xhtml'
         self.dkb_br.open(limit_url)
 
         soup = self.dkb_br.get_current_page()
         form = soup.find('form', attrs={'id':'form597962073_1'})
 
         limit_dic = {}
@@ -139,25 +158,25 @@
                         except IndexError:
                             pass
                         except AttributeError:
                             pass
 
         return limit_dic
 
-
     def get_document_links(self, url):
         """ create a dictionary of the documents stored in a pbost folder
 
         args:
             self.dkb_br - browser object
             url - folder url
 
         returns:
             dictionary of the documents
         """
+        print_debug(self.debug, 'DKBRobo.get_document_links({0})\n'.format(url))
         document_dic = {}
 
         self.dkb_br.open(url)
         soup = self.dkb_br.get_current_page()
         table = soup.find('table', attrs={'class':'widget widget abaxx-table expandableTable expandableTable-with-sort'})
         if table:
             tbody = table.find('tbody')
@@ -173,14 +192,15 @@
         args:
             self.dkb_br - browser object
             url - folder url
 
         returns:
             dictionary of exemption orders
         """
+        print_debug(self.debug, 'DKBRobo.get_exemption_order()\n')
         exo_url = self.base_url + '/DkbTransactionBanking/content/personaldata/ExemptionOrder/ExemptionOrderOverview.xhtml'
         self.dkb_br.open(exo_url)
 
         soup = self.dkb_br.get_current_page()
 
         for lbr in soup.findAll("br"):
             lbr.replace_with("")
@@ -220,23 +240,34 @@
                     except IndexError:
                         pass
                     except AttributeError:
                         pass
 
         return exo_dic
 
+    def get_financial_statement(self):
+        """ get finanical statement """
+        print_debug(self.debug, 'DKBRobo.get_financial_statement()\n')
+        statement_url = self.base_url + '/DkbTransactionBanking/content/LoginWithBoundDevice/LoginWithBoundDeviceProcess/confirmLogin.xhtml'
+
+        # statement_url = self.base_url + '/DkbTransactionBanking/content/banking/financialstatus/FinancialComposite/FinancialStatus.xhtml?$event=init'
+        self.dkb_br.open(statement_url)
+        soup = self.dkb_br.get_current_page()
+        return soup
+
     def get_points(self):
         """ returns the DKB points
 
         args:
             self.dkb_br - browser object
 
         returns:
             points - dkb points
         """
+        print_debug(self.debug, 'DKBRobo.get_points()\n')
         point_url = self.base_url + '/DkbTransactionBanking/content/FavorableWorld/Overview.xhtml?$event=init'
         self.dkb_br.open(point_url)
 
         p_dic = {}
         soup = self.dkb_br.get_current_page()
         table = soup.find('table', attrs={'class':'expandableTable'})
         if table:
@@ -268,14 +299,15 @@
         """ get standing orders
         args:
             self.dkb_br          - browser object
 
         returns:
             so_dic = standing order dic
         """
+        print_debug(self.debug, 'DKBRobo.get_standing_orders()\n')
         so_url = self.base_url + '/banking/finanzstatus/dauerauftraege?$event=infoStandingOrder'
         self.dkb_br.open(so_url)
 
         so_list = []
         soup = self.dkb_br.get_current_page()
         table = soup.find('table', attrs={'class':'expandableTable'})
         if table:
@@ -318,14 +350,15 @@
 
         returns:
             list of transactions; each transaction gets represented as a dictionary containing the following information
             - date   - booking date
             - amount - amount
             - text   - test
         """
+        print_debug(self.debug, 'DKBRobo.get_account_transactions({0}/{1}: {2}/{3})\n'.format(transaction_url, atype, date_from, date_to))
         transaction_list = []
         if atype == 'account':
             transaction_list = self.get_account_transactions(transaction_url, date_from, date_to)
         elif atype == 'creditcard':
             transaction_list = self.get_creditcard_transactions(transaction_url, date_from, date_to)
 
         return transaction_list
@@ -345,14 +378,16 @@
             - account number
             - type (account, creditcard, depot)
             - account balance
             - date of balance
             - link to details
             - link to transactions
         """
+        print_debug(self.debug, 'DKBRobo.login()\n')
+
         # login url
         login_url = self.base_url + '/' + 'banking'
 
         # create browser and login
         self.dkb_br = self.new_instance()
 
         self.dkb_br.open(login_url)
@@ -380,38 +415,136 @@
             # remove crlf
             last_login = last_login.replace('\n', '')
             # format string in a way we need it
             last_login = last_login.replace('  ', '')
             last_login = last_login.replace('Letzte Anmeldung:', '')
             self.last_login = last_login
 
-            # parse account date
-            self.account_dic = self.parse_overview(soup)
+            if soup.find('h1').text.strip() == 'Anmeldung bestätigen':
+                if self.chip_tan:
+                    # chiptan input
+                    login_confirmed = self.ctan_check(soup)
+                else:
+                    # app confirmation needed to continue
+                    login_confirmed = self.login_confirm()
+
+                if login_confirmed:
+                    # login got confirmed get overview and parse data
+                    soup_new = self.get_financial_statement()
+                    self.account_dic = self.parse_overview(soup_new)
+
+    def ctan_check(self, _soup):
+        """ input of chiptan during login """
+        print_debug(self.debug, 'DKBRobo.ctan_check()\n')
+
+        # search form
+        self.dkb_br.select_form('form[name="confirmForm"]')
+        self.dkb_br["$event"] = 'tanVerification'
+        # open page to insert tan
+        self.dkb_br.submit_selected()
+        soup = self.dkb_br.get_current_page()
+
+        login_confirm = False
+
+        # select tan form
+        self.dkb_br.select_form('#next')
+        # print steps to be done
+        olist = soup.find("ol")
+        for li_ in olist.findAll('li'):
+            print(li_.text.strip())
+
+        # ask for TAN
+        self.dkb_br["tan"] = input("TAN: ")
+
+        # submit form and check response
+        self.dkb_br.submit_selected()
+        soup = self.dkb_br.get_current_page()
+
+        # catch tan error
+        if soup.find("div", attrs={'class':'clearfix module text errorMessage'}):
+            print('Login failed due to wrong tan! Aborting...')
+            sys.exit(0)
+        else:
+            print_debug(self.debug, 'TAN is correct...\n')
+            login_confirm = True
+
+        return login_confirm
+
+    def login_confirm(self):
+        """ confirm login to dkb via app
+
+        returns:
+            true/false - depending if login has been confirmed
+        """
+        print_debug(self.debug, 'DKBRobo.login_confirm()\n')
+        print('check your banking app and confirm login...')
+
+        try:
+            # get xsrf token
+            soup = self.dkb_br.get_current_page()
+            xsrf_token = soup.find('input', attrs={'name':'XSRFPreventionToken'}).get('value')
+        except BaseException:
+            # fallback
+            xsrf_token = generate_random_string(25)
+
+        # timestamp in miliseconds for py3 and py2
+        try:
+            poll_id = int(datetime.utcnow().timestamp()*1e3)
+        except BaseException:
+            poll_id = int(round(time.time() * 1000))
+
+        # poll url
+        poll_url = self.base_url + '/DkbTransactionBanking/content/LoginWithBoundDevice/LoginWithBoundDeviceProcess/confirmLogin.xhtml'
+        login_confirmed = False
+        while not login_confirmed:
+            poll_id += 1
+            # add id to pollurl
+            url = poll_url + '?$event=pollingVerification&_=' + str(poll_id)
+            result = self.dkb_br.open(url).json()
+            if 'guiState' in result:
+                print_debug(self.debug, 'poll(id: {0} status: {1}\n'.format(poll_id, result['guiState']))
+                if result['guiState'] == 'MAP_TO_EXIT':
+                    print_debug(self.debug, 'session got confirmed...\n')
+                    login_confirmed = True
+                elif result['guiState'] == 'EXPIRED':
+                    print('Session got expired. Aborting...')
+                    sys.exit(0)
+            else:
+                print('Timeout during session confirmation. Aborting...')
+                sys.exit(0)
+            time.sleep(2)
+
+        post_data = {'$event': 'next', 'XSRFPreventionToken': xsrf_token}
+        self.dkb_br.post(url=poll_url, data=post_data)
+
+        return login_confirmed
 
     def logout(self):
         """ logout from DKB banking area
 
         args:
             self.dkb_br = browser object
 
         returns:
             None
         """
+        print_debug(self.debug, 'DKBRobo.logout()\n')
         logout_url = self.base_url + '/' + 'DkbTransactionBanking/banner.xhtml?$event=logout'
         self.dkb_br.open(logout_url)
 
     def new_instance(self):
         """ creates a new browser instance
 
         args:
            None
 
         returns:
            self.dkb_br - instance
         """
+        print_debug(self.debug, 'DKBRobo.new_instance()\n')
         # create browser and cookiestore objects
         self.dkb_br = mechanicalsoup.StatefulBrowser()
         dkb_cj = cookielib.LWPCookieJar()
         self.dkb_br.set_cookiejar = dkb_cj
 
         # configure browser
         self.dkb_br.set_handle_equiv = True
@@ -438,14 +571,15 @@
 
         returns:
             list of transactions captured. Each transaction gets represented by a hash containing the following values
             - date - booking date
             - amount - amount
             - text - text
         """
+        print_debug(self.debug, 'DKBRobo.parse_account_transactions()\n')
         # create empty list
         transaction_list = []
 
         # parse CSV
         for row in csv.reader(transactions.decode('latin-1').splitlines(), delimiter=';'):
             if len(row) == 12:
                 # skip first line
@@ -488,14 +622,15 @@
         returns:
             list of transactions captured. Each transaction gets represented by a hash containing the following values
             - bdate - booking date
             - vdate - valuta date
             - amount - amount
             - text - text
         """
+        print_debug(self.debug, 'DKBRobo.parse_cc_transactions()\n')
         # parse the lines to get all account infos
         # soup = BeautifulSoup(transactions, "html5lib")
 
         # create empty list
         transaction_list = []
 
         # parse CSV
@@ -528,14 +663,15 @@
             - account number
             - type (account, credit-card, depot)
             - account balance
             - date of balance
             - link to details
             - link to transactions
         """
+        print_debug(self.debug, 'DKBRobo.parse_overview()\n')
         # get account information
         overview_dic = {}
         # to_remove = 0
         counter = 0
         ontop = 0
         for row in soup.findAll("tr", attrs={'class':'mainRow'}):
             overview_dic[counter] = {}
@@ -602,14 +738,15 @@
            dictionary in the following format
 
            - folder name in postbox
                 - details -> link to document overview
                 - documents
                     - name of document -> document link
         """
+        print_debug(self.debug, 'DKBRobo.scan_postbox()\n')
         pb_url = self.base_url + '/banking/postfach'
         self.dkb_br.open(pb_url)
         soup = self.dkb_br.get_current_page()
         table = soup.find('table', attrs={'id':'welcomeMboTable'})
         tbody = table.find('tbody')
 
         pb_dic = {}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dkb_robo-0.8.3/dkb_robo.egg-info/PKG-INFO` & `dkb_robo-0.9/dkb_robo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dkb-robo
-Version: 0.8.3
+Version: 0.9
 Summary: library to access the internet banking area of "Deutsche Kreditbank" to get account information and transactions.
 Home-page: https://github.com/grindsa/dkb-robo
 Author: grindsa
 Author-email: grindelsack@gmail.com
 License: GPL
 Description: UNKNOWN
 Platform: any
```

### Comparing `dkb_robo-0.8.3/PKG-INFO` & `dkb_robo-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dkb_robo
-Version: 0.8.3
+Version: 0.9
 Summary: library to access the internet banking area of "Deutsche Kreditbank" to get account information and transactions.
 Home-page: https://github.com/grindsa/dkb-robo
 Author: grindsa
 Author-email: grindelsack@gmail.com
 License: GPL
 Description: UNKNOWN
 Platform: any
```

### Comparing `dkb_robo-0.8.3/README.md` & `dkb_robo-0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 dkb-robo is a python library to access the internet banking area of  "Deutsche Kreditbank" to fetch 
 - account information and current balances
 - transactions from creditcards and checking accounts (Girokonten)
 - query the content of "DKB Postbox"
 - get standing orders (Dauerauftrag)
 - get information about credit limits and exemption orders (Freistellungsauftrag)
 
+Starting from version 0.9 dkb-robo can handle the 2nd factor DKB introduced to fullfill the [PSD2 obligations](https://en.wikipedia.org/wiki/Payment_Services_Directive). Starting from Septemter 2019 logins must be confirmed by either
+* DKB app
+* Insertion of a TAN created by ChipTan method
+
+TANs created by TAN2go application are not supported as I do not really see a use-case for it. If you need this support feel free to raise an [issue](https://github.com/grindsa/dkb-robo/issues/new) to let me know.
+
+The introduction of a 2nd factor does  limit the usage of dkb-robo for automation purposes. DKB is unfortuately ~~not willing/ not able~~ not allowed to open their PSD2-API for non-Fintechs. I disccues this with them for weeks but some point they stopped responding to my emails.
 
 ## Getting Started
 
 These instructions will get you a copy of the project up and running on your local machine.
 
 ### Prerequisites
 
@@ -49,16 +56,21 @@
 you need to import dkb-robo into your script
 ```
 > from dkb_robo import DKBRobo
 ``` 
 
 create a new DKBRobo context handler and login to DKB portal
 ```
-> with DKBRobo(dkb_user, dkb_password) as dkb:
+> with DKBRobo(dkb_user, dkb_password, tan_insert, debug) as dkb:
 ```
+* dbk_user: username to access the dkb portal
+* dkb_password: corresponding login password
+* tan_insert: (True/**False**) Chiptan usage - dbk-robo will ask for a TAN (generated by ChipTan method) during login
+* debug: (True/**False**) Debug mode
+
 
 After login you can return the 
 * the last login date
 ```
 > print(dkb.last_login)
 14.03.2017, 13:19 Uhr
 ```
```

### Comparing `dkb_robo-0.8.3/setup.py` & `dkb_robo-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='dkb_robo',
-    version='0.8.3',
+    version='0.9',
     description='library to access the internet banking area of "Deutsche Kreditbank" to get account information and transactions.',
     url='https://github.com/grindsa/dkb-robo',
     author='grindsa',
     author_email='grindelsack@gmail.com',
     license='GPL',
     packages=['dkb_robo'],
     platforms='any',
```

### Comparing `dkb_robo-0.8.3/test/test_dkb_robo.py` & `dkb_robo-0.9/test/test_dkb_robo.py`

 * *Files identical despite different names*

