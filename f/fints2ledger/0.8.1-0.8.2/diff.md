# Comparing `tmp/fints2ledger-0.8.1.tar.gz` & `tmp/fints2ledger-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fints2ledger-0.8.1.tar", last modified: Thu May  5 19:44:40 2022, max compression
+gzip compressed data, was "fints2ledger-0.8.2.tar", last modified: Fri May 19 19:54:14 2023, max compression
```

## Comparing `fints2ledger-0.8.1.tar` & `fints2ledger-0.8.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2022-05-05 19:44:40.463315 fints2ledger-0.8.1/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1051 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/LICENSE
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     7268 2022-05-05 19:44:40.463315 fints2ledger-0.8.1/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     6578 2022-05-05 19:40:47.000000 fints2ledger-0.8.1/README.md
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2022-05-05 19:44:40.463315 fints2ledger-0.8.1/fints2ledger/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        0 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/__init__.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)     1302 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/autocomplete.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     6541 2022-05-05 19:41:43.000000 fints2ledger-0.8.1/fints2ledger/config.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1892 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/csv2ledger.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      952 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/csv_converter.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1158 2022-04-24 18:51:46.000000 fints2ledger-0.8.1/fints2ledger/fints2csv.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)     5117 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/ledger_converter.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)      397 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/main.py
--rwxrwxr-x   0 moritz    (1000) moritz    (1000)      799 2022-04-09 18:53:12.000000 fints2ledger-0.8.1/fints2ledger/transaction_retriever.py
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      390 2022-05-05 19:41:49.000000 fints2ledger-0.8.1/fints2ledger/utils.py
-drwxrwxr-x   0 moritz    (1000) moritz    (1000)        0 2022-05-05 19:44:40.463315 fints2ledger-0.8.1/fints2ledger.egg-info/
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     7268 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/PKG-INFO
--rw-rw-r--   0 moritz    (1000) moritz    (1000)      563 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/SOURCES.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/dependency_links.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       57 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/entry_points.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)        1 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/not-zip-safe
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       38 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/requires.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       13 2022-05-05 19:44:40.000000 fints2ledger-0.8.1/fints2ledger.egg-info/top_level.txt
--rw-rw-r--   0 moritz    (1000) moritz    (1000)       62 2022-05-05 19:44:40.467315 fints2ledger-0.8.1/setup.cfg
--rw-rw-r--   0 moritz    (1000) moritz    (1000)     1090 2022-05-05 19:42:47.000000 fints2ledger-0.8.1/setup.py
+drwxr-xr-x   0 moritz    (1000) moritz    (1000)        0 2023-05-19 19:54:14.126375 fints2ledger-0.8.2/
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     8591 2023-05-19 19:54:14.126375 fints2ledger-0.8.2/PKG-INFO
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     6567 2023-05-19 19:45:13.000000 fints2ledger-0.8.2/README.md
+drwxr-xr-x   0 moritz    (1000) moritz    (1000)        0 2023-05-19 19:54:14.116375 fints2ledger-0.8.2/fints2ledger/
+-rw-r--r--   0 moritz    (1000) moritz    (1000)        0 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/__init__.py
+-rwxr-xr-x   0 moritz    (1000) moritz    (1000)     1302 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/autocomplete.py
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     6592 2023-05-19 19:30:26.000000 fints2ledger-0.8.2/fints2ledger/config.py
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     1892 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/csv2ledger.py
+-rw-r--r--   0 moritz    (1000) moritz    (1000)      952 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/csv_converter.py
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     1558 2023-05-19 19:41:19.000000 fints2ledger-0.8.2/fints2ledger/fints2csv.py
+-rwxr-xr-x   0 moritz    (1000) moritz    (1000)     5117 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/ledger_converter.py
+-rwxr-xr-x   0 moritz    (1000) moritz    (1000)      397 2023-05-19 19:23:16.000000 fints2ledger-0.8.2/fints2ledger/main.py
+-rwxr-xr-x   0 moritz    (1000) moritz    (1000)      799 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/transaction_retriever.py
+-rw-r--r--   0 moritz    (1000) moritz    (1000)      390 2023-05-19 19:13:58.000000 fints2ledger-0.8.2/fints2ledger/utils.py
+drwxr-xr-x   0 moritz    (1000) moritz    (1000)        0 2023-05-19 19:54:14.126375 fints2ledger-0.8.2/fints2ledger.egg-info/
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     8591 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/PKG-INFO
+-rw-r--r--   0 moritz    (1000) moritz    (1000)      555 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 moritz    (1000) moritz    (1000)        1 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 moritz    (1000) moritz    (1000)       57 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/entry_points.txt
+-rw-r--r--   0 moritz    (1000) moritz    (1000)        1 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/not-zip-safe
+-rw-r--r--   0 moritz    (1000) moritz    (1000)       38 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/requires.txt
+-rw-r--r--   0 moritz    (1000) moritz    (1000)       13 2023-05-19 19:54:14.000000 fints2ledger-0.8.2/fints2ledger.egg-info/top_level.txt
+-rw-r--r--   0 moritz    (1000) moritz    (1000)       62 2023-05-19 19:54:14.126375 fints2ledger-0.8.2/setup.cfg
+-rw-r--r--   0 moritz    (1000) moritz    (1000)     1091 2023-05-19 19:46:38.000000 fints2ledger-0.8.2/setup.py
```

### Comparing `fints2ledger-0.8.1/PKG-INFO` & `fints2ledger-0.8.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: fints2ledger
-Version: 0.8.1
-Summary: A tool for downloading transactions from FinTS banking APIs and sorting them into a ledger journal.
-Home-page: https://github.com/MoritzR/fints2ledger
-Author: Moritz Rumpf
-Author-email: moritz.rumpf@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fints2ledger
 [![Build Status](https://github.com/MoritzR/fints2ledger/actions/workflows/main.yml/badge.svg)](https://github.com/MoritzR/fints2ledger/actions) [![Coverage Status](https://coveralls.io/repos/github/MoritzR/fints2ledger/badge.svg?branch=master)](https://coveralls.io/github/MoritzR/fints2ledger?branch=master) [![PyPI version](https://badge.fury.io/py/fints2ledger.svg)](https://badge.fury.io/py/fints2ledger) [![languages](https://img.shields.io/pypi/pyversions/fints2ledger.svg)](https://pypi.org/project/fints2ledger)
 
 A tool for downloading transactions from FinTS banking APIs and sorting them into a [ledger journal](http://hledger.org/).
 
 [pyfints](https://github.com/raphaelm/python-fints) is used to download the transactions. A list of compatible banks can be found there. This tool was tested with [ING][ing-link] and [GLS Bank][gls-link].
 
@@ -40,15 +21,15 @@
 
 Create config file at `~/.config/fints2ledger/config.yml` file with the following contents and replace values in the fints category:
 (This file will also be automatically created if missing)
 ```
 fints:
   blz: "<your bank's BLZ>"
   account: "<your account number>"
-  password: "<your banking password>"
+  password: "<your banking password>  (set to empty string if you prefer being prompted)"
   endpoint: <your bank fints endpoint> # e.g.: https://fints.ing.de/fints for ING
   selectedAccount: "<account number>" # defaults to the value from "account"
                                       # useful when you have multiple accounts for the same login
 
 ledger:
   prompts:
     - credit_account
@@ -169,22 +150,19 @@
 ## Developing
 You can modify the code yourself and run it with:
 ```
 git clone https://github.com/MoritzR/fints2ledger.git
 cd fints2ledger
 python fints2ledger/main.py
 ```
-Don't forget that your python version should be 3.5 or higher.
 
 You can run the tests with:
 ```
 pip install green
 green
 ```
 
 ## Changelog
 The changelog can be found in [CHANGELOG.md](CHANGELOG.md)
 
 [ing-link]: https://www.ing.de
 [gls-link]: https://www.gls.de
-
-
```

### Comparing `fints2ledger-0.8.1/README.md` & `fints2ledger-0.8.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,169 +1,186 @@
-# fints2ledger
-[![Build Status](https://github.com/MoritzR/fints2ledger/actions/workflows/main.yml/badge.svg)](https://github.com/MoritzR/fints2ledger/actions) [![Coverage Status](https://coveralls.io/repos/github/MoritzR/fints2ledger/badge.svg?branch=master)](https://coveralls.io/github/MoritzR/fints2ledger?branch=master) [![PyPI version](https://badge.fury.io/py/fints2ledger.svg)](https://badge.fury.io/py/fints2ledger) [![languages](https://img.shields.io/pypi/pyversions/fints2ledger.svg)](https://pypi.org/project/fints2ledger)
-
-A tool for downloading transactions from FinTS banking APIs and sorting them into a [ledger journal](http://hledger.org/).
-
-[pyfints](https://github.com/raphaelm/python-fints) is used to download the transactions. A list of compatible banks can be found there. This tool was tested with [ING][ing-link] and [GLS Bank][gls-link].
-
-![](demo.gif)
-
-## Contents
-- [Install](#install)
-- [Usage](#usage)
-- [Developing](#developing)
-- [Changelog](#changelog)
-
-## Install
-
-```
-pip install --upgrade fints2ledger
-```
-
-Create config file at `~/.config/fints2ledger/config.yml` file with the following contents and replace values in the fints category:
-(This file will also be automatically created if missing)
-```
-fints:
-  blz: "<your bank's BLZ>"
-  account: "<your account number>"
-  password: "<your banking password>"
-  endpoint: <your bank fints endpoint> # e.g.: https://fints.ing.de/fints for ING
-  selectedAccount: "<account number>" # defaults to the value from "account"
-                                      # useful when you have multiple accounts for the same login
-
-ledger:
-  prompts:
-    - credit_account
-    - debit_account
-  autocomplete:
-    accounts:
-      - credit_account
-      - debit_account
-  defaults:
-    debit_account: assets:bank:checking
-  md5:
-    - date
-    - payee
-    - purpose
-    - amount
-```
-
-## Usage
-Run
-```
-fints2ledger
-```
-This will download the transactions from the last year and tries to convert them to a ledger journal.
-
-A list of available command line arguments:
-```
-usage: fints2ledger [-h] [--no-csv] [--no-ledger] [--csv-file CSVFILE]
-                    [--ledger-file LEDGERFILE] [--files-path FILES_PATH]
-                    [--date START] [--separator SEPARATOR]
-                    [--csv_date_format CSV_DATE_FORMAT]
-
-Converting transactions from fints apis to ledger.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --no-csv              exclude conversion from fints to csv (default: not
-                        excluded)
-  --no-ledger           exclude conversion from csv to ledger (default: not
-                        excluded)
-  --csv-file CSVFILE    file to store/load csv transactions to/from (default:
-                        transactions.csv)
-  --ledger-file LEDGERFILE
-                        file to store ledger entries to (default:
-                        ledger.journal)
-  --files-path FILES_PATH
-                        directory to store fints2ledger files (like
-                        config.yml) (default: ~/.config/fints2ledger/)
-  --date START          start date to pull the FinTS entries from (format:
-                        2017/12/31 or 17/12/31, default: last year)
-  --separator SEPARATOR
-                        character used as separator in csv file (default: ;)
-  --csv_date_format CSV_DATE_FORMAT
-                        Date format used in the donwloaded csv (and
-                        subsequently the ledger file). hledger supports 3 date
-                        formats (https://hledger.org/1.9/journal.html#simple-
-                        dates). Format needs to be compatible with pythons
-                        strftime(), see https://docs.python.org/3/library/date
-                        time.html#strftime-strptime-behavior
-                        (fints.csv_date_format in config.yml) (default:
-                        %Y/%m/%d)
-
-```
-
-### Template File
-A template file with the name `template.txt` will be automatically generated. It will be user to create the ledger entries.
-It looks something like
-```
-{date} {payee} {posting} {purpose}
-    ; md5sum: {md5sum}
-    {debit_account:<60}    {currency} {debit}
-    {credit_account:<60}    {currency} {credit}
-
-```
-Each name inside curly brackets can specify a value that can come from either a named csv column, a default value (from the `config.yml`) or an input prompt (also from the `config.yml`).
-
-If you use [beancount](https://beancount.github.io) instead of (h)ledger use this template instead:
-
-```
-{date} txn "{payee} {posting} {purpose}"
-    ; md5sum: {md5sum}
-    {debit_account:<60}   {debit} {currency}
-    {credit_account:<60}   {credit} {currency}
-```
-
-### Automatically matching transactions
-In the `ledger` category you can use a regex match on any field of the transaction data to automatically fill other fields.
-
-Example: I do not want to enter a `credit_account` and `purpose` for my monthly recurring payments for the rent of my apartment. Same for my music streaming transactions. I can change the `config.yml` like this:
-```
-ledger:
-  ...
-  fills:
-    - match:
-        payee: "The Landlord"
-        purpose: "Rent for apartment B month.*"
-      fill:
-        credit_account: "expenses:monthly:rent"
-        purpose: "monthly rent"
-    - match:
-        payee: "MUSIC COMPANY 123"
-      fill:
-        credit_account: "expenses:monthly:musiccompany"
-        purpose: "Monthly fee for music streaming"
-```
-
-### Converting from csv to ledger without requesting a FinTS API
-With the argument `--no-csv` the program will not create a csv file with banking transactions itself (default is fints -> csv -> ledger).
-Instead, it will convert directly from a csv file to ledger. This is useful when all transactions have already been downloaded or when converting from another source than FinTS to ledger.
-
-The csv file must provide a headline which names the columns. The column names are then used to fill the values in the template file.
-Example:
-```
-date;amount;currency;payee;posting;purpose
-2017/04/26;167.31;EUR;Billy, Bill;bonus;for vacation
-2017/04/27;-130;EUR;John, Smith;debit entry;monthly electricity payment
-```
-
-## Developing
-You can modify the code yourself and run it with:
-```
-git clone https://github.com/MoritzR/fints2ledger.git
-cd fints2ledger
-python fints2ledger/main.py
-```
-Don't forget that your python version should be 3.5 or higher.
-
-You can run the tests with:
-```
-pip install green
-green
-```
-
-## Changelog
-The changelog can be found in [CHANGELOG.md](CHANGELOG.md)
-
-[ing-link]: https://www.ing.de
-[gls-link]: https://www.gls.de
+Metadata-Version: 2.1
+Name: fints2ledger
+Version: 0.8.2
+Summary: A tool for downloading transactions from FinTS banking APIs and sorting them into a ledger journal.
+Home-page: https://github.com/MoritzR/fints2ledger
+Author: Moritz Rumpf
+Author-email: moritz.rumpf@gmail.com
+License: MIT
+Description: # fints2ledger
+        [![Build Status](https://github.com/MoritzR/fints2ledger/actions/workflows/main.yml/badge.svg)](https://github.com/MoritzR/fints2ledger/actions) [![Coverage Status](https://coveralls.io/repos/github/MoritzR/fints2ledger/badge.svg?branch=master)](https://coveralls.io/github/MoritzR/fints2ledger?branch=master) [![PyPI version](https://badge.fury.io/py/fints2ledger.svg)](https://badge.fury.io/py/fints2ledger) [![languages](https://img.shields.io/pypi/pyversions/fints2ledger.svg)](https://pypi.org/project/fints2ledger)
+        
+        A tool for downloading transactions from FinTS banking APIs and sorting them into a [ledger journal](http://hledger.org/).
+        
+        [pyfints](https://github.com/raphaelm/python-fints) is used to download the transactions. A list of compatible banks can be found there. This tool was tested with [ING][ing-link] and [GLS Bank][gls-link].
+        
+        ![](demo.gif)
+        
+        ## Contents
+        - [Install](#install)
+        - [Usage](#usage)
+        - [Developing](#developing)
+        - [Changelog](#changelog)
+        
+        ## Install
+        
+        ```
+        pip install --upgrade fints2ledger
+        ```
+        
+        Create config file at `~/.config/fints2ledger/config.yml` file with the following contents and replace values in the fints category:
+        (This file will also be automatically created if missing)
+        ```
+        fints:
+          blz: "<your bank's BLZ>"
+          account: "<your account number>"
+          password: "<your banking password>  (set to empty string if you prefer being prompted)"
+          endpoint: <your bank fints endpoint> # e.g.: https://fints.ing.de/fints for ING
+          selectedAccount: "<account number>" # defaults to the value from "account"
+                                              # useful when you have multiple accounts for the same login
+        
+        ledger:
+          prompts:
+            - credit_account
+            - debit_account
+          autocomplete:
+            accounts:
+              - credit_account
+              - debit_account
+          defaults:
+            debit_account: assets:bank:checking
+          md5:
+            - date
+            - payee
+            - purpose
+            - amount
+        ```
+        
+        ## Usage
+        Run
+        ```
+        fints2ledger
+        ```
+        This will download the transactions from the last year and tries to convert them to a ledger journal.
+        
+        A list of available command line arguments:
+        ```
+        usage: fints2ledger [-h] [--no-csv] [--no-ledger] [--csv-file CSVFILE]
+                            [--ledger-file LEDGERFILE] [--files-path FILES_PATH]
+                            [--date START] [--separator SEPARATOR]
+                            [--csv_date_format CSV_DATE_FORMAT]
+        
+        Converting transactions from fints apis to ledger.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --no-csv              exclude conversion from fints to csv (default: not
+                                excluded)
+          --no-ledger           exclude conversion from csv to ledger (default: not
+                                excluded)
+          --csv-file CSVFILE    file to store/load csv transactions to/from (default:
+                                transactions.csv)
+          --ledger-file LEDGERFILE
+                                file to store ledger entries to (default:
+                                ledger.journal)
+          --files-path FILES_PATH
+                                directory to store fints2ledger files (like
+                                config.yml) (default: ~/.config/fints2ledger/)
+          --date START          start date to pull the FinTS entries from (format:
+                                2017/12/31 or 17/12/31, default: last year)
+          --separator SEPARATOR
+                                character used as separator in csv file (default: ;)
+          --csv_date_format CSV_DATE_FORMAT
+                                Date format used in the donwloaded csv (and
+                                subsequently the ledger file). hledger supports 3 date
+                                formats (https://hledger.org/1.9/journal.html#simple-
+                                dates). Format needs to be compatible with pythons
+                                strftime(), see https://docs.python.org/3/library/date
+                                time.html#strftime-strptime-behavior
+                                (fints.csv_date_format in config.yml) (default:
+                                %Y/%m/%d)
+        
+        ```
+        
+        ### Template File
+        A template file with the name `template.txt` will be automatically generated. It will be user to create the ledger entries.
+        It looks something like
+        ```
+        {date} {payee} {posting} {purpose}
+            ; md5sum: {md5sum}
+            {debit_account:<60}    {currency} {debit}
+            {credit_account:<60}    {currency} {credit}
+        
+        ```
+        Each name inside curly brackets can specify a value that can come from either a named csv column, a default value (from the `config.yml`) or an input prompt (also from the `config.yml`).
+        
+        If you use [beancount](https://beancount.github.io) instead of (h)ledger use this template instead:
+        
+        ```
+        {date} txn "{payee} {posting} {purpose}"
+            ; md5sum: {md5sum}
+            {debit_account:<60}   {debit} {currency}
+            {credit_account:<60}   {credit} {currency}
+        ```
+        
+        ### Automatically matching transactions
+        In the `ledger` category you can use a regex match on any field of the transaction data to automatically fill other fields.
+        
+        Example: I do not want to enter a `credit_account` and `purpose` for my monthly recurring payments for the rent of my apartment. Same for my music streaming transactions. I can change the `config.yml` like this:
+        ```
+        ledger:
+          ...
+          fills:
+            - match:
+                payee: "The Landlord"
+                purpose: "Rent for apartment B month.*"
+              fill:
+                credit_account: "expenses:monthly:rent"
+                purpose: "monthly rent"
+            - match:
+                payee: "MUSIC COMPANY 123"
+              fill:
+                credit_account: "expenses:monthly:musiccompany"
+                purpose: "Monthly fee for music streaming"
+        ```
+        
+        ### Converting from csv to ledger without requesting a FinTS API
+        With the argument `--no-csv` the program will not create a csv file with banking transactions itself (default is fints -> csv -> ledger).
+        Instead, it will convert directly from a csv file to ledger. This is useful when all transactions have already been downloaded or when converting from another source than FinTS to ledger.
+        
+        The csv file must provide a headline which names the columns. The column names are then used to fill the values in the template file.
+        Example:
+        ```
+        date;amount;currency;payee;posting;purpose
+        2017/04/26;167.31;EUR;Billy, Bill;bonus;for vacation
+        2017/04/27;-130;EUR;John, Smith;debit entry;monthly electricity payment
+        ```
+        
+        ## Developing
+        You can modify the code yourself and run it with:
+        ```
+        git clone https://github.com/MoritzR/fints2ledger.git
+        cd fints2ledger
+        python fints2ledger/main.py
+        ```
+        
+        You can run the tests with:
+        ```
+        pip install green
+        green
+        ```
+        
+        ## Changelog
+        The changelog can be found in [CHANGELOG.md](CHANGELOG.md)
+        
+        [ing-link]: https://www.ing.de
+        [gls-link]: https://www.gls.de
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
```

### Comparing `fints2ledger-0.8.1/fints2ledger/autocomplete.py` & `fints2ledger-0.8.2/fints2ledger/autocomplete.py`

 * *Files identical despite different names*

### Comparing `fints2ledger-0.8.1/fints2ledger/config.py` & `fints2ledger-0.8.2/fints2ledger/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Config:
     DEFAULT_CONFIG = {
         'fints': {
             'blz': "<your bank's BLZ>",
             'account': '<your account number>',
-            'password': '<your banking password>',
+            'password': '<your banking password> (set to empty string if you prefer being prompted)',
             'endpoint': '<your bank fints endpoint>',
         },
         'ledger': {
             'prompts': ['credit_account', 'debit_account'],
             'autocomplete': {'accounts': ['credit_account', 'debit_account']},
             'defaults': {'debit_account': 'assets:bank:checking'},
             'md5': ['date', 'payee', 'purpose', 'amount'],
```

### Comparing `fints2ledger-0.8.1/fints2ledger/csv2ledger.py` & `fints2ledger-0.8.2/fints2ledger/csv2ledger.py`

 * *Files identical despite different names*

### Comparing `fints2ledger-0.8.1/fints2ledger/csv_converter.py` & `fints2ledger-0.8.2/fints2ledger/csv_converter.py`

 * *Files identical despite different names*

### Comparing `fints2ledger-0.8.1/fints2ledger/fints2csv.py` & `fints2ledger-0.8.2/fints2ledger/fints2csv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 from fints2ledger.transaction_retriever import TRetriever
 from fints.client import FinTS3PinTanClient
 from fints2ledger.csv_converter import CsvConverter
 from mt940.models import Date
+from getpass import getpass
 
 
 class Fints2Csv:
     def __init__(self, config):
         self.config = config
 
     def retrieveAndSave(self):
-        client = FinTS3PinTanClient(
-            self.config["fints"]["blz"],  # Your bank's BLZ
-            self.config["fints"]["account"],  # your account number
-            self.config["fints"]["password"],
-            # e.g. 'https://fints.ing-diba.de/fints/'
-            self.config["fints"]["endpoint"]
-        )
-
-        retriever = TRetriever(client, self.config["fints"]["selectedAccount"])
         converter = CsvConverter(self.config["fints"]["csv_separator"], self.config["fints"]["csv_date_format"])
 
-        csv_output = "\n".join(map(lambda transaction: converter.convert(
-            transaction), retriever.get_hbci_transactions(self.config["fints"]["start"], Date.today())))
+        transactions = retrieve_transactions({
+            "blz": self.config["fints"]["blz"],  # Your bank's BLZ
+            "account": self.config["fints"]["account"],  # your account number
+            "password": self.config["fints"]["password"] or getpass("Password: "),
+            # e.g. 'https://fints.ing-diba.de/fints/'
+            "endpoint": self.config["fints"]["endpoint"],
+            "selected_account": self.config["fints"]["selectedAccount"],
+            "start": self.config["fints"]["start"],
+            "end": Date.today()
+        })
+
+        csv_output = "\n".join(map(converter.convert, transactions))
 
         with open(self.config["files"]["csv_file"], 'w') as f:
             f.write(converter.get_headline())
             f.write("\n")
             f.write(csv_output)
+
+def retrieve_transactions(args):
+    client = FinTS3PinTanClient(
+        args["blz"],
+        args["account"],
+        args["password"],
+        args["endpoint"],
+        product_id = "EC449295201FA9BE5040B9154"
+    )
+    return TRetriever(client, args["selected_account"]).get_hbci_transactions(args["start"], args["end"])
```

### Comparing `fints2ledger-0.8.1/fints2ledger/ledger_converter.py` & `fints2ledger-0.8.2/fints2ledger/ledger_converter.py`

 * *Files identical despite different names*

### Comparing `fints2ledger-0.8.1/fints2ledger/transaction_retriever.py` & `fints2ledger-0.8.2/fints2ledger/transaction_retriever.py`

 * *Files identical despite different names*

### Comparing `fints2ledger-0.8.1/fints2ledger.egg-info/PKG-INFO` & `fints2ledger-0.8.2/fints2ledger.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,186 @@
 Metadata-Version: 2.1
 Name: fints2ledger
-Version: 0.8.1
+Version: 0.8.2
 Summary: A tool for downloading transactions from FinTS banking APIs and sorting them into a ledger journal.
 Home-page: https://github.com/MoritzR/fints2ledger
 Author: Moritz Rumpf
 Author-email: moritz.rumpf@gmail.com
 License: MIT
+Description: # fints2ledger
+        [![Build Status](https://github.com/MoritzR/fints2ledger/actions/workflows/main.yml/badge.svg)](https://github.com/MoritzR/fints2ledger/actions) [![Coverage Status](https://coveralls.io/repos/github/MoritzR/fints2ledger/badge.svg?branch=master)](https://coveralls.io/github/MoritzR/fints2ledger?branch=master) [![PyPI version](https://badge.fury.io/py/fints2ledger.svg)](https://badge.fury.io/py/fints2ledger) [![languages](https://img.shields.io/pypi/pyversions/fints2ledger.svg)](https://pypi.org/project/fints2ledger)
+        
+        A tool for downloading transactions from FinTS banking APIs and sorting them into a [ledger journal](http://hledger.org/).
+        
+        [pyfints](https://github.com/raphaelm/python-fints) is used to download the transactions. A list of compatible banks can be found there. This tool was tested with [ING][ing-link] and [GLS Bank][gls-link].
+        
+        ![](demo.gif)
+        
+        ## Contents
+        - [Install](#install)
+        - [Usage](#usage)
+        - [Developing](#developing)
+        - [Changelog](#changelog)
+        
+        ## Install
+        
+        ```
+        pip install --upgrade fints2ledger
+        ```
+        
+        Create config file at `~/.config/fints2ledger/config.yml` file with the following contents and replace values in the fints category:
+        (This file will also be automatically created if missing)
+        ```
+        fints:
+          blz: "<your bank's BLZ>"
+          account: "<your account number>"
+          password: "<your banking password>  (set to empty string if you prefer being prompted)"
+          endpoint: <your bank fints endpoint> # e.g.: https://fints.ing.de/fints for ING
+          selectedAccount: "<account number>" # defaults to the value from "account"
+                                              # useful when you have multiple accounts for the same login
+        
+        ledger:
+          prompts:
+            - credit_account
+            - debit_account
+          autocomplete:
+            accounts:
+              - credit_account
+              - debit_account
+          defaults:
+            debit_account: assets:bank:checking
+          md5:
+            - date
+            - payee
+            - purpose
+            - amount
+        ```
+        
+        ## Usage
+        Run
+        ```
+        fints2ledger
+        ```
+        This will download the transactions from the last year and tries to convert them to a ledger journal.
+        
+        A list of available command line arguments:
+        ```
+        usage: fints2ledger [-h] [--no-csv] [--no-ledger] [--csv-file CSVFILE]
+                            [--ledger-file LEDGERFILE] [--files-path FILES_PATH]
+                            [--date START] [--separator SEPARATOR]
+                            [--csv_date_format CSV_DATE_FORMAT]
+        
+        Converting transactions from fints apis to ledger.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --no-csv              exclude conversion from fints to csv (default: not
+                                excluded)
+          --no-ledger           exclude conversion from csv to ledger (default: not
+                                excluded)
+          --csv-file CSVFILE    file to store/load csv transactions to/from (default:
+                                transactions.csv)
+          --ledger-file LEDGERFILE
+                                file to store ledger entries to (default:
+                                ledger.journal)
+          --files-path FILES_PATH
+                                directory to store fints2ledger files (like
+                                config.yml) (default: ~/.config/fints2ledger/)
+          --date START          start date to pull the FinTS entries from (format:
+                                2017/12/31 or 17/12/31, default: last year)
+          --separator SEPARATOR
+                                character used as separator in csv file (default: ;)
+          --csv_date_format CSV_DATE_FORMAT
+                                Date format used in the donwloaded csv (and
+                                subsequently the ledger file). hledger supports 3 date
+                                formats (https://hledger.org/1.9/journal.html#simple-
+                                dates). Format needs to be compatible with pythons
+                                strftime(), see https://docs.python.org/3/library/date
+                                time.html#strftime-strptime-behavior
+                                (fints.csv_date_format in config.yml) (default:
+                                %Y/%m/%d)
+        
+        ```
+        
+        ### Template File
+        A template file with the name `template.txt` will be automatically generated. It will be user to create the ledger entries.
+        It looks something like
+        ```
+        {date} {payee} {posting} {purpose}
+            ; md5sum: {md5sum}
+            {debit_account:<60}    {currency} {debit}
+            {credit_account:<60}    {currency} {credit}
+        
+        ```
+        Each name inside curly brackets can specify a value that can come from either a named csv column, a default value (from the `config.yml`) or an input prompt (also from the `config.yml`).
+        
+        If you use [beancount](https://beancount.github.io) instead of (h)ledger use this template instead:
+        
+        ```
+        {date} txn "{payee} {posting} {purpose}"
+            ; md5sum: {md5sum}
+            {debit_account:<60}   {debit} {currency}
+            {credit_account:<60}   {credit} {currency}
+        ```
+        
+        ### Automatically matching transactions
+        In the `ledger` category you can use a regex match on any field of the transaction data to automatically fill other fields.
+        
+        Example: I do not want to enter a `credit_account` and `purpose` for my monthly recurring payments for the rent of my apartment. Same for my music streaming transactions. I can change the `config.yml` like this:
+        ```
+        ledger:
+          ...
+          fills:
+            - match:
+                payee: "The Landlord"
+                purpose: "Rent for apartment B month.*"
+              fill:
+                credit_account: "expenses:monthly:rent"
+                purpose: "monthly rent"
+            - match:
+                payee: "MUSIC COMPANY 123"
+              fill:
+                credit_account: "expenses:monthly:musiccompany"
+                purpose: "Monthly fee for music streaming"
+        ```
+        
+        ### Converting from csv to ledger without requesting a FinTS API
+        With the argument `--no-csv` the program will not create a csv file with banking transactions itself (default is fints -> csv -> ledger).
+        Instead, it will convert directly from a csv file to ledger. This is useful when all transactions have already been downloaded or when converting from another source than FinTS to ledger.
+        
+        The csv file must provide a headline which names the columns. The column names are then used to fill the values in the template file.
+        Example:
+        ```
+        date;amount;currency;payee;posting;purpose
+        2017/04/26;167.31;EUR;Billy, Bill;bonus;for vacation
+        2017/04/27;-130;EUR;John, Smith;debit entry;monthly electricity payment
+        ```
+        
+        ## Developing
+        You can modify the code yourself and run it with:
+        ```
+        git clone https://github.com/MoritzR/fints2ledger.git
+        cd fints2ledger
+        python fints2ledger/main.py
+        ```
+        
+        You can run the tests with:
+        ```
+        pip install green
+        green
+        ```
+        
+        ## Changelog
+        The changelog can be found in [CHANGELOG.md](CHANGELOG.md)
+        
+        [ing-link]: https://www.ing.de
+        [gls-link]: https://www.gls.de
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.0
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# fints2ledger
-[![Build Status](https://github.com/MoritzR/fints2ledger/actions/workflows/main.yml/badge.svg)](https://github.com/MoritzR/fints2ledger/actions) [![Coverage Status](https://coveralls.io/repos/github/MoritzR/fints2ledger/badge.svg?branch=master)](https://coveralls.io/github/MoritzR/fints2ledger?branch=master) [![PyPI version](https://badge.fury.io/py/fints2ledger.svg)](https://badge.fury.io/py/fints2ledger) [![languages](https://img.shields.io/pypi/pyversions/fints2ledger.svg)](https://pypi.org/project/fints2ledger)
-
-A tool for downloading transactions from FinTS banking APIs and sorting them into a [ledger journal](http://hledger.org/).
-
-[pyfints](https://github.com/raphaelm/python-fints) is used to download the transactions. A list of compatible banks can be found there. This tool was tested with [ING][ing-link] and [GLS Bank][gls-link].
-
-![](demo.gif)
-
-## Contents
-- [Install](#install)
-- [Usage](#usage)
-- [Developing](#developing)
-- [Changelog](#changelog)
-
-## Install
-
-```
-pip install --upgrade fints2ledger
-```
-
-Create config file at `~/.config/fints2ledger/config.yml` file with the following contents and replace values in the fints category:
-(This file will also be automatically created if missing)
-```
-fints:
-  blz: "<your bank's BLZ>"
-  account: "<your account number>"
-  password: "<your banking password>"
-  endpoint: <your bank fints endpoint> # e.g.: https://fints.ing.de/fints for ING
-  selectedAccount: "<account number>" # defaults to the value from "account"
-                                      # useful when you have multiple accounts for the same login
-
-ledger:
-  prompts:
-    - credit_account
-    - debit_account
-  autocomplete:
-    accounts:
-      - credit_account
-      - debit_account
-  defaults:
-    debit_account: assets:bank:checking
-  md5:
-    - date
-    - payee
-    - purpose
-    - amount
-```
-
-## Usage
-Run
-```
-fints2ledger
-```
-This will download the transactions from the last year and tries to convert them to a ledger journal.
-
-A list of available command line arguments:
-```
-usage: fints2ledger [-h] [--no-csv] [--no-ledger] [--csv-file CSVFILE]
-                    [--ledger-file LEDGERFILE] [--files-path FILES_PATH]
-                    [--date START] [--separator SEPARATOR]
-                    [--csv_date_format CSV_DATE_FORMAT]
-
-Converting transactions from fints apis to ledger.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --no-csv              exclude conversion from fints to csv (default: not
-                        excluded)
-  --no-ledger           exclude conversion from csv to ledger (default: not
-                        excluded)
-  --csv-file CSVFILE    file to store/load csv transactions to/from (default:
-                        transactions.csv)
-  --ledger-file LEDGERFILE
-                        file to store ledger entries to (default:
-                        ledger.journal)
-  --files-path FILES_PATH
-                        directory to store fints2ledger files (like
-                        config.yml) (default: ~/.config/fints2ledger/)
-  --date START          start date to pull the FinTS entries from (format:
-                        2017/12/31 or 17/12/31, default: last year)
-  --separator SEPARATOR
-                        character used as separator in csv file (default: ;)
-  --csv_date_format CSV_DATE_FORMAT
-                        Date format used in the donwloaded csv (and
-                        subsequently the ledger file). hledger supports 3 date
-                        formats (https://hledger.org/1.9/journal.html#simple-
-                        dates). Format needs to be compatible with pythons
-                        strftime(), see https://docs.python.org/3/library/date
-                        time.html#strftime-strptime-behavior
-                        (fints.csv_date_format in config.yml) (default:
-                        %Y/%m/%d)
-
-```
-
-### Template File
-A template file with the name `template.txt` will be automatically generated. It will be user to create the ledger entries.
-It looks something like
-```
-{date} {payee} {posting} {purpose}
-    ; md5sum: {md5sum}
-    {debit_account:<60}    {currency} {debit}
-    {credit_account:<60}    {currency} {credit}
-
-```
-Each name inside curly brackets can specify a value that can come from either a named csv column, a default value (from the `config.yml`) or an input prompt (also from the `config.yml`).
-
-If you use [beancount](https://beancount.github.io) instead of (h)ledger use this template instead:
-
-```
-{date} txn "{payee} {posting} {purpose}"
-    ; md5sum: {md5sum}
-    {debit_account:<60}   {debit} {currency}
-    {credit_account:<60}   {credit} {currency}
-```
-
-### Automatically matching transactions
-In the `ledger` category you can use a regex match on any field of the transaction data to automatically fill other fields.
-
-Example: I do not want to enter a `credit_account` and `purpose` for my monthly recurring payments for the rent of my apartment. Same for my music streaming transactions. I can change the `config.yml` like this:
-```
-ledger:
-  ...
-  fills:
-    - match:
-        payee: "The Landlord"
-        purpose: "Rent for apartment B month.*"
-      fill:
-        credit_account: "expenses:monthly:rent"
-        purpose: "monthly rent"
-    - match:
-        payee: "MUSIC COMPANY 123"
-      fill:
-        credit_account: "expenses:monthly:musiccompany"
-        purpose: "Monthly fee for music streaming"
-```
-
-### Converting from csv to ledger without requesting a FinTS API
-With the argument `--no-csv` the program will not create a csv file with banking transactions itself (default is fints -> csv -> ledger).
-Instead, it will convert directly from a csv file to ledger. This is useful when all transactions have already been downloaded or when converting from another source than FinTS to ledger.
-
-The csv file must provide a headline which names the columns. The column names are then used to fill the values in the template file.
-Example:
-```
-date;amount;currency;payee;posting;purpose
-2017/04/26;167.31;EUR;Billy, Bill;bonus;for vacation
-2017/04/27;-130;EUR;John, Smith;debit entry;monthly electricity payment
-```
-
-## Developing
-You can modify the code yourself and run it with:
-```
-git clone https://github.com/MoritzR/fints2ledger.git
-cd fints2ledger
-python fints2ledger/main.py
-```
-Don't forget that your python version should be 3.5 or higher.
-
-You can run the tests with:
-```
-pip install green
-green
-```
-
-## Changelog
-The changelog can be found in [CHANGELOG.md](CHANGELOG.md)
-
-[ing-link]: https://www.ing.de
-[gls-link]: https://www.gls.de
-
-
```

### Comparing `fints2ledger-0.8.1/fints2ledger.egg-info/SOURCES.txt` & `fints2ledger-0.8.2/fints2ledger.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 fints2ledger/__init__.py
 fints2ledger/autocomplete.py
 fints2ledger/config.py
 fints2ledger/csv2ledger.py
```

### Comparing `fints2ledger-0.8.1/setup.py` & `fints2ledger-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='fints2ledger',
-    version='0.8.1',
+    version='0.8.2',
     description='A tool for downloading transactions from FinTS banking APIs and sorting them into a ledger journal.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/MoritzR/fints2ledger',
     author='Moritz Rumpf',
     author_email='moritz.rumpf@gmail.com',
     license='MIT',
-    python_requires='>=3.6.0',
+    python_requires='>=3.7.0',
     entry_points={
         'console_scripts': ['fints2ledger=fints2ledger.main:main'],
     },
-    install_requires=['mt-940>=4.11,<5', 'fints>=3,<4', 'pyyaml>=6'],
+    install_requires=['mt-940>=4.11,<5', 'fints>=4,<5', 'pyyaml>=6'],
     setup_requires=['green'],
     packages=['fints2ledger'],
     zip_safe=False,
     classifiers=[
         'Development Status :: 3 - Alpha',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

