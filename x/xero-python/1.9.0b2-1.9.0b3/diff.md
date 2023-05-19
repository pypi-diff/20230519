# Comparing `tmp/xero_python-1.9.0b2.tar.gz` & `tmp/xero_python-1.9.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xero_python-1.9.0b2.tar", last modified: Tue Aug 31 20:30:07 2021, max compression
+gzip compressed data, was "dist/xero_python-1.9.0b3.tar", last modified: Tue Aug 31 21:03:05 2021, max compression
```

## Comparing `xero_python-1.9.0b2.tar` & `xero_python-1.9.0b3.tar`

### file list

```diff
@@ -1,578 +1,578 @@
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.433864 xero_python-1.9.0b2/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      118 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/AUTHORS.md
--rw-r--r--   0 rett.behrens   (501) staff       (20)       60 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/HISTORY.md
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1077 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/LICENSE
--rw-r--r--   0 rett.behrens   (501) staff       (20)      258 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/MANIFEST.in
--rw-r--r--   0 rett.behrens   (501) staff       (20)    27051 2021-08-31 20:30:07.434277 xero_python-1.9.0b2/PKG-INFO
--rw-r--r--   0 rett.behrens   (501) staff       (20)    21898 2021-07-21 20:12:28.000000 xero_python-1.9.0b2/README.md
--rw-r--r--   0 rett.behrens   (501) staff       (20)      111 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/requirements.txt
--rw-r--r--   0 rett.behrens   (501) staff       (20)      293 2021-08-31 20:30:07.435522 xero_python-1.9.0b2/setup.cfg
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1570 2021-08-31 20:16:45.000000 xero_python-1.9.0b2/setup.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.842096 xero_python-1.9.0b2/tests/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      297 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.847101 xero_python-1.9.0b2/tests/accounting/
--rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.857612 xero_python-1.9.0b2/tests/accounting/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/api/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.869192 xero_python-1.9.0b2/tests/accounting/api/cassettes/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3082 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/api/cassettes/test_get_organisations.yaml
--rw-r--r--   0 rett.behrens   (501) staff       (20)   372230 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.881060 xero_python-1.9.0b2/tests/accounting/api/fixtures/
--rw-r--r--   0 rett.behrens   (501) staff       (20)    54574 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/api/fixtures/inv-0032.pdf
--rw-r--r--   0 rett.behrens   (501) staff       (20)    24648 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/accounting/api/test_accounting_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.890200 xero_python-1.9.0b2/tests/cassettes/
--rw-r--r--   0 rett.behrens   (501) staff       (20)    71720 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/cassettes/test_vcr.yaml
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4209 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/conftest.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.900066 xero_python-1.9.0b2/tests/identity/
--rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/identity/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.917089 xero_python-1.9.0b2/tests/identity/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/identity/api/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.922516 xero_python-1.9.0b2/tests/identity/api/cassettes/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1077 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/identity/api/cassettes/test_get_connections.yaml
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1082 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/identity/api/test_identity_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.953077 xero_python-1.9.0b2/tests/test_api_client/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1325 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.963246 xero_python-1.9.0b2/tests/test_api_client/cassettes/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3082 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2891 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11797 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/test_deserializer.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9813 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/test_oauth2.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11877 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_api_client/test_serializer.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      538 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_executor.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2601 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/tests/test_single_dispatch_str.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.967507 xero_python-1.9.0b2/xero_python/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      131 2021-08-31 20:16:45.000000 xero_python-1.9.0b2/xero_python/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.974480 xero_python-1.9.0b2/xero_python/accounting/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9261 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.981614 xero_python-1.9.0b2/xero_python/accounting/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      115 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)   707680 2021-08-31 20:15:59.000000 xero_python-1.9.0b2/xero_python/accounting/api/accounting_api.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      615 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/accounting/api/exception_handler.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.104887 xero_python-1.9.0b2/xero_python/accounting/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9161 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    21659 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1140 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/account_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/accounts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2324 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/accounts_payable.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2354 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/accounts_receivable.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2677 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/action.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/actions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11191 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/address.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11833 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/address_for_organisation.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7779 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/allocation.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:15:38.000000 xero_python-1.9.0b2/xero_python/accounting/models/allocations.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5767 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/attachment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/attachments.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3851 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/balance_details.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2707 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    22262 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/bank_transaction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/bank_transactions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11476 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/bank_transfer.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/bank_transfers.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    19204 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/batch_payment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7359 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/batch_payment_details.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/batch_payments.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2102 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/bill.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6367 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/branding_theme.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/branding_themes.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6165 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/budget.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4213 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/budget_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3376 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/budget_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4177 2021-07-21 19:32:27.000000 xero_python-1.9.0b2/xero_python/accounting/models/budget_lines.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/budgets.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4074 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/cis_org_setting.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1740 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/cis_org_settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2670 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/cis_setting.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1713 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/cis_settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    41029 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/contact.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5186 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/contact_group.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/contact_groups.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4479 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/contact_person.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/contacts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3620 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/conversion_balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2542 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/conversion_date.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3862 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/country_code.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    28233 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/credit_note.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1713 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/credit_notes.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1662 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/currencies.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2287 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/currency.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3172 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/currency_code.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7371 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/element.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8912 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/employee.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1636 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/employees.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3853 2021-08-31 20:15:39.000000 xero_python-1.9.0b2/xero_python/accounting/models/error.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11540 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/expense_claim.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/expense_claims.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3611 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/external_link.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3909 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/history_record.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/history_records.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2475 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/import_summary.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8021 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/import_summary_accounts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1792 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/import_summary_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1662 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/import_summary_organisation.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    37542 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/invoice.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1690 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/invoice_reminder.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/invoice_reminders.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/invoices.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17257 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/item.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1520 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/items.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8857 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/journal.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11322 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/journal_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/journals.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      582 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/line_amount_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14285 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/line_item.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4693 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/line_item_tracking.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14905 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/linked_transaction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1916 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/linked_transactions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14384 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/manual_journal.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7857 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/manual_journal_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/manual_journals.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1907 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/online_invoice.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/online_invoices.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    36482 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/organisation.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1752 2021-08-31 20:15:40.000000 xero_python-1.9.0b2/xero_python/accounting/models/organisations.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17593 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/overpayment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1723 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/overpayments.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    24787 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1785 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment_delete.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7124 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment_service.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1829 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment_services.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2118 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment_term.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      676 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payment_term_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/payments.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5412 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/phone.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    18343 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/prepayment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/prepayments.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4803 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/purchase.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    27432 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/purchase_order.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/purchase_orders.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    21933 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/quote.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      587 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/quote_line_amount_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      647 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/quote_status_codes.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1549 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/quotes.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    15859 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/receipt.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/receipts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14986 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/repeating_invoice.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1887 2021-08-31 20:15:41.000000 xero_python-1.9.0b2/xero_python/accounting/models/repeating_invoices.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6110 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2092 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_attribute.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2256 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_cell.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2913 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_fields.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2771 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_row.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3452 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_rows.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8330 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_with_row.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1641 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/report_with_rows.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/reports.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1717 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/request_empty.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      590 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/row_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3195 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/sales_tracking_category.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7997 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/schedule.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3545 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/setup.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4321 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tax_component.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14871 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tax_rate.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1626 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tax_rates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2230 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tax_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17343 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/accounting/models/ten_ninety_nine_contact.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17370 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/accounting/models/ten_nintey_nine_contact.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5905 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/time_zone.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1913 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tracking_categories.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7202 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tracking_category.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5241 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tracking_option.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1650 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/tracking_options.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7432 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/user.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1520 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/users.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1693 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/accounting/models/validation_error.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.111072 xero_python-1.9.0b2/xero_python/api_client/
--rw-r--r--   0 rett.behrens   (501) staff       (20)    26974 2021-07-21 20:12:28.000000 xero_python-1.9.0b2/xero_python/api_client/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7399 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/api_client/configuration.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9836 2021-08-31 18:09:53.000000 xero_python-1.9.0b2/xero_python/api_client/deserializer.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11982 2021-07-21 20:12:28.000000 xero_python-1.9.0b2/xero_python/api_client/oauth2.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7337 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/api_client/serializer.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.112550 xero_python-1.9.0b2/xero_python/appstore/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      745 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/appstore/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.114861 xero_python-1.9.0b2/xero_python/appstore/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      110 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/appstore/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3768 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/appstore/api/app_store_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.123049 xero_python-1.9.0b2/xero_python/appstore/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      650 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/appstore/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5006 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/appstore/models/plan.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3237 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/appstore/models/price.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4837 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/appstore/models/problem_details.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4357 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/appstore/models/product.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8651 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/appstore/models/subscription.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6168 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/appstore/models/subscription_item.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.123920 xero_python-1.9.0b2/xero_python/assets/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1335 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/assets/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.125727 xero_python-1.9.0b2/xero_python/assets/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      101 2021-08-31 20:15:42.000000 xero_python-1.9.0b2/xero_python/assets/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17938 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/api/asset_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.146326 xero_python-1.9.0b2/xero_python/assets/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1249 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    15830 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/asset.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      655 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/asset_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      665 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/asset_status_query_param.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8812 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/asset_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2284 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/assets.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9196 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/book_depreciation_detail.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11640 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/book_depreciation_setting.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5500 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/error.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6341 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/field_validation_errors_element.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3674 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/pagination.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5539 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/resource_validation_errors_element.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10228 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/assets/models/setting.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.148352 xero_python-1.9.0b2/xero_python/exceptions/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4576 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/exceptions/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2817 2021-07-21 19:32:27.000000 xero_python-1.9.0b2/xero_python/exceptions/http_status_exceptions.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.149422 xero_python-1.9.0b2/xero_python/file/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      820 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/file/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.151733 xero_python-1.9.0b2/xero_python/file/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)       99 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    48802 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/file/api/files_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.164648 xero_python-1.9.0b2/xero_python/file/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      736 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/file/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4100 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/association.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6863 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/file_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3382 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/files.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4619 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/folder.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1513 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/folders.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3536 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/file/models/inline_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3554 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/file/models/inline_object1.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      743 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/object_group.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2188 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/object_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3879 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/upload_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4488 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/file/models/user.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.165529 xero_python-1.9.0b2/xero_python/identity/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      586 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/identity/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.168884 xero_python-1.9.0b2/xero_python/identity/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      109 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/identity/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      750 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/identity/api/exception_handler.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5626 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/identity/api/identity_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.172983 xero_python-1.9.0b2/xero_python/identity/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      492 2021-08-31 20:15:34.000000 xero_python-1.9.0b2/xero_python/identity/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5143 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/identity/models/access_token.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7188 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/identity/models/connection.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4283 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/identity/models/refresh_token.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1832 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/models.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.173871 xero_python-1.9.0b2/xero_python/payrollau/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6229 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.175980 xero_python-1.9.0b2/xero_python/payrollau/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:15:43.000000 xero_python-1.9.0b2/xero_python/payrollau/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    82168 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollau/api/payroll_au_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.255053 xero_python-1.9.0b2/xero_python/payrollau/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6131 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3569 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1144 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/account_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      614 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/allowance_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3119 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/api_exception.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6071 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/bank_account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      625 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/calendar_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5380 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/deduction_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9852 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/deduction_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      549 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/deduction_type_calculation_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9487 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    17461 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/earnings_rate.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      588 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/earnings_rate_calculation_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      817 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/earnings_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    32000 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/employee.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      509 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/employee_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1588 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/employees.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      606 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/employment_basis.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      499 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/employment_termination_payment_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      526 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/entitlement_final_pay_payout_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5716 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/home_address.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3669 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_accrual_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9818 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_application.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1839 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_applications.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4494 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3683 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10136 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      696 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_line_calculation_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1577 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_lines.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4841 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_period.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      516 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_period_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9806 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      596 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/leave_type_contribution_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      634 2021-08-31 20:15:44.000000 xero_python-1.9.0b2/xero_python/payrollau/models/manual_tax_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6856 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/opening_balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4236 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_item.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1560 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_items.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14719 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_run.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      497 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_run_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1549 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_runs.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5064 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/pay_template.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      655 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payment_frequency_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8385 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payroll_calendar.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1810 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payroll_calendars.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    16494 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payslip.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8178 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payslip_lines.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1551 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payslip_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10615 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payslip_summary.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1559 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/payslips.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      541 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/rate_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4936 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1868 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_lines.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5612 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      592 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/residency_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3770 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1580 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/settings_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2995 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3257 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3307 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      570 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/state.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12093 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_fund.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4088 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_fund_product.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_fund_products.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      502 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_fund_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1636 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_funds.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8280 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4068 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/super_membership.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      582 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_calculation_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      601 2021-08-31 20:15:45.000000 xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_contribution_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10003 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    19138 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/tax_declaration.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6143 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/tax_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      563 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/tfn_exemption_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8712 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/timesheet.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4983 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1609 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      586 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1617 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/timesheets.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1645 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollau/models/validation_error.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.255741 xero_python-1.9.0b2/xero_python/payrollnz/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8007 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.257254 xero_python-1.9.0b2/xero_python/payrollnz/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)   197486 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrollnz/api/payroll_nz_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.337598 xero_python-1.9.0b2/xero_python/payrollnz/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7909 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4086 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1552 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/accounts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5999 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/address.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8594 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/bank_account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10860 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/benefit.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      640 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/calendar_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7308 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/deduction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5257 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/deduction_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/deduction_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/deductions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10566 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5493 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_order.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3304 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_order_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3272 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_orders.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12582 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rate.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:15:46.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rate_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3135 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6394 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_template.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3295 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_template_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12710 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3375 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_earnings_templates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7801 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4301 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3271 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2980 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10706 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_setup.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3215 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_setup_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    13344 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3178 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_type_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3146 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2928 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leaves.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2986 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4570 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_opening_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3429 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_opening_balances_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2712 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_template.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3252 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_template_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3182 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_templates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4503 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3442 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8014 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_summary.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    19815 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leave.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3544 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leaves.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    21571 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_tax.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3116 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employee_tax_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2954 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employees.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3885 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3060 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/employment_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2725 2021-08-31 20:15:47.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/gross_earnings_history.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2303 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/invalid_field.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2687 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_accrual_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    10848 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4949 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_period.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2965 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_periods.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6560 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3042 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_type_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3010 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/leave_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3542 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pagination.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11777 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7678 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendar.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3260 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendar_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3228 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendars.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2931 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2899 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_runs.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    28891 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slip.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2968 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slip_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2936 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slips.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5038 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/payment_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2950 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/payment_method.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/payment_method_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5106 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/problem.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11135 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5447 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3171 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursements.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12190 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wage.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3243 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wage_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3191 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wages.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2902 2021-08-31 20:15:48.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5484 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      882 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_category.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4878 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3389 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3357 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deductions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6358 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/superannuation_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3047 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/superannuation_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3015 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/superannuations.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      739 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/tax_code.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5126 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/tax_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6462 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/tax_settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9649 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11016 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5970 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_line_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/timesheets.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3299 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/tracking_categories.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3679 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrollnz/models/tracking_category.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.338491 xero_python-1.9.0b2/xero_python/payrolluk/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7208 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.341066 xero_python-1.9.0b2/xero_python/payrolluk/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      614 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/payrolluk/api/exception_handler.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)   202748 2021-08-31 20:15:55.000000 xero_python-1.9.0b2/xero_python/payrolluk/api/payroll_uk_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.416079 xero_python-1.9.0b2/xero_python/payrolluk/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7110 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4175 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1552 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/accounts.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5284 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/address.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3810 2021-08-31 20:15:49.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/bank_account.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    15279 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/benefit.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5049 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/benefit_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2949 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/benefit_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2917 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/benefits.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2582 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/court_order_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    18040 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/deduction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4352 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/deduction_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/deduction_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/deductions.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9494 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5493 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_order.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3304 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_order_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3272 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_orders.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12977 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rate.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rate_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3135 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6394 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_template.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3295 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_template_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    13825 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     7801 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4301 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3271 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2980 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8210 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3178 2021-08-31 20:15:50.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_type_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3146 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2928 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leaves.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2986 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8493 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_opening_balances.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3414 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_opening_balances_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2712 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_template.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3252 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_template_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3305 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_templates.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4503 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_balance.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3442 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8014 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_summary.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    19815 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leave.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3544 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leaves.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11263 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_tax.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3116 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employee_tax_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2954 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employees.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4935 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employment.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3060 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/employment_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2303 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/invalid_field.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2687 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_accrual_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6705 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4949 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_period.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2965 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_periods.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8352 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3042 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_type_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3010 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/leave_types.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3542 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pagination.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12379 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     8264 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendar.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3260 2021-08-31 20:15:51.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendar_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3228 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendars.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2931 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2899 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/pay_runs.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5038 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payment_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3073 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payment_method.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payment_method_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    26544 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payslip.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2968 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payslip_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2936 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/payslips.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5106 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/problem.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4599 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3578 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3171 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursements.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    11173 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wage.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3243 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wage_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3191 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wages.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2902 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/settings.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5484 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/statutory_deduction.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      978 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/statutory_deduction_category.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6148 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/tax_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9565 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     6869 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_earnings_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5970 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_line.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:15:52.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_line_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_object.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/timesheets.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3299 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/tracking_categories.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3679 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/payrolluk/models/tracking_category.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.416770 xero_python-1.9.0b2/xero_python/project/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1474 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/__init__.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.418263 xero_python-1.9.0b2/xero_python/project/api/
--rw-r--r--   0 rett.behrens   (501) staff       (20)      106 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/api/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    45972 2021-08-31 20:15:54.000000 xero_python-1.9.0b2/xero_python/project/api/project_api.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:07.433356 xero_python-1.9.0b2/xero_python/project/models/
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1383 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/__init__.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2076 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/amount.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      498 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/charge_type.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3047 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/currency_code.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2343 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/error.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4280 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/pagination.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    19641 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4416 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project_create_or_update.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1627 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project_patch.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)      477 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project_status.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2939 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project_user.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2206 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/project_users.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2154 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/projects.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    14338 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/task.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     4437 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/task_create_or_update.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2115 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/tasks.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     2190 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/time_entries.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     9410 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/time_entry.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     5854 2021-08-31 20:15:53.000000 xero_python-1.9.0b2/xero_python/project/models/time_entry_create_or_update.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)    12592 2021-08-31 20:15:54.000000 xero_python-1.9.0b2/xero_python/rest.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     3125 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/single_dispatch_str.py
--rw-r--r--   0 rett.behrens   (501) staff       (20)     1162 2021-04-06 22:02:35.000000 xero_python-1.9.0b2/xero_python/utils.py
-drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 20:30:06.973777 xero_python-1.9.0b2/xero_python.egg-info/
--rw-r--r--   0 rett.behrens   (501) staff       (20)    27051 2021-08-31 20:30:06.000000 xero_python-1.9.0b2/xero_python.egg-info/PKG-INFO
--rw-r--r--   0 rett.behrens   (501) staff       (20)    24542 2021-08-31 20:30:06.000000 xero_python-1.9.0b2/xero_python.egg-info/SOURCES.txt
--rw-r--r--   0 rett.behrens   (501) staff       (20)        1 2021-08-31 20:30:06.000000 xero_python-1.9.0b2/xero_python.egg-info/dependency_links.txt
--rw-r--r--   0 rett.behrens   (501) staff       (20)       37 2021-08-31 20:30:06.000000 xero_python-1.9.0b2/xero_python.egg-info/requires.txt
--rw-r--r--   0 rett.behrens   (501) staff       (20)       12 2021-08-31 20:30:06.000000 xero_python-1.9.0b2/xero_python.egg-info/top_level.txt
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.616903 xero_python-1.9.0b3/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      118 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/AUTHORS.md
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       60 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/HISTORY.md
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1077 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/LICENSE
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      258 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/MANIFEST.in
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    27051 2021-08-31 21:03:05.617200 xero_python-1.9.0b3/PKG-INFO
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    21898 2021-07-21 20:12:28.000000 xero_python-1.9.0b3/README.md
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      111 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/requirements.txt
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      293 2021-08-31 21:03:05.618531 xero_python-1.9.0b3/setup.cfg
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1570 2021-08-31 20:54:15.000000 xero_python-1.9.0b3/setup.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.239310 xero_python-1.9.0b3/tests/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      297 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.239935 xero_python-1.9.0b3/tests/accounting/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.241438 xero_python-1.9.0b3/tests/accounting/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/api/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.244607 xero_python-1.9.0b3/tests/accounting/api/cassettes/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3082 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/api/cassettes/test_get_organisations.yaml
+-rw-r--r--   0 rett.behrens   (501) staff       (20)   372230 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.247264 xero_python-1.9.0b3/tests/accounting/api/fixtures/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    54574 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/api/fixtures/inv-0032.pdf
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    24648 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/accounting/api/test_accounting_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.248316 xero_python-1.9.0b3/tests/cassettes/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    71720 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/cassettes/test_vcr.yaml
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4209 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/conftest.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.249422 xero_python-1.9.0b3/tests/identity/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/identity/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.250808 xero_python-1.9.0b3/tests/identity/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       24 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/identity/api/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.251517 xero_python-1.9.0b3/tests/identity/api/cassettes/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1077 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/identity/api/cassettes/test_get_connections.yaml
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1082 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/identity/api/test_identity_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.254470 xero_python-1.9.0b3/tests/test_api_client/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1325 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.256360 xero_python-1.9.0b3/tests/test_api_client/cassettes/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3082 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2891 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11797 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/test_deserializer.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9813 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/test_oauth2.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11877 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_api_client/test_serializer.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      538 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_executor.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2601 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/tests/test_single_dispatch_str.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.259736 xero_python-1.9.0b3/xero_python/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      131 2021-08-31 20:54:15.000000 xero_python-1.9.0b3/xero_python/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.265051 xero_python-1.9.0b3/xero_python/accounting/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9261 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.267955 xero_python-1.9.0b3/xero_python/accounting/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      115 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)   707680 2021-08-31 20:53:29.000000 xero_python-1.9.0b3/xero_python/accounting/api/accounting_api.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      615 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/accounting/api/exception_handler.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.406277 xero_python-1.9.0b3/xero_python/accounting/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9161 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    21659 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1140 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/account_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/accounts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2324 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/accounts_payable.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2354 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/accounts_receivable.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2677 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/action.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/actions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11191 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/address.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11833 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/address_for_organisation.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7779 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/allocation.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/allocations.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5767 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/attachment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/attachments.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3851 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/balance_details.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2707 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    22262 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/bank_transaction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/bank_transactions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11476 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/bank_transfer.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:52:57.000000 xero_python-1.9.0b3/xero_python/accounting/models/bank_transfers.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    19204 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/batch_payment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7359 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/batch_payment_details.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/batch_payments.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2102 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/bill.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6367 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/branding_theme.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/branding_themes.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6165 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/budget.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4213 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/budget_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3376 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/budget_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4177 2021-07-21 19:32:27.000000 xero_python-1.9.0b3/xero_python/accounting/models/budget_lines.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/budgets.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4074 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/cis_org_setting.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1740 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/cis_org_settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2670 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/cis_setting.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1713 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/cis_settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    41029 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/contact.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5186 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/contact_group.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/contact_groups.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4479 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/contact_person.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/contacts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3620 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/conversion_balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2542 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/conversion_date.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3862 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/country_code.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    28233 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/credit_note.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1713 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/credit_notes.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1662 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/currencies.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2287 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/currency.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3172 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/currency_code.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7371 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/element.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8912 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/employee.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1636 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/employees.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3853 2021-08-31 20:52:58.000000 xero_python-1.9.0b3/xero_python/accounting/models/error.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11540 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/expense_claim.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1771 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/expense_claims.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3611 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/external_link.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3909 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/history_record.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/history_records.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2475 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/import_summary.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8021 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/import_summary_accounts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1792 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/import_summary_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1662 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/import_summary_organisation.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    37542 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/invoice.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1690 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/invoice_reminder.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/invoice_reminders.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/invoices.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17257 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/item.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1520 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/items.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8857 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/journal.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11322 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/journal_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/journals.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      582 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/line_amount_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14285 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/line_item.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4693 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/line_item_tracking.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14905 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/linked_transaction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1916 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/linked_transactions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14384 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/manual_journal.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7857 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/manual_journal_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/manual_journals.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1907 2021-08-31 20:52:59.000000 xero_python-1.9.0b3/xero_python/accounting/models/online_invoice.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/online_invoices.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    36482 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/organisation.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1752 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/organisations.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17593 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/overpayment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1723 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/overpayments.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    24787 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1785 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment_delete.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7124 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment_service.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1829 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment_services.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2118 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment_term.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      676 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payment_term_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/payments.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5412 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/phone.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    18343 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/prepayment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1694 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/prepayments.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4803 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/purchase.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    27432 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/purchase_order.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1800 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/purchase_orders.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    21933 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/quote.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      587 2021-08-31 20:53:00.000000 xero_python-1.9.0b3/xero_python/accounting/models/quote_line_amount_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      647 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/quote_status_codes.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1549 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/quotes.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    15859 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/receipt.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1607 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/receipts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14986 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/repeating_invoice.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1887 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/repeating_invoices.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6110 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/report.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2092 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_attribute.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2256 2021-08-31 20:53:01.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_cell.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2913 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_fields.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2771 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_row.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3452 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_rows.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8330 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_with_row.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1641 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/report_with_rows.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1578 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/reports.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1717 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/request_empty.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      590 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/row_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3195 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/sales_tracking_category.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7997 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/schedule.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3545 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/setup.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4321 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tax_component.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14871 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/accounting/models/tax_rate.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1626 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tax_rates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2230 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tax_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17343 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/accounting/models/ten_ninety_nine_contact.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17370 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/accounting/models/ten_nintey_nine_contact.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5905 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/time_zone.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1913 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tracking_categories.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7202 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/accounting/models/tracking_category.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5241 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tracking_option.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1650 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/tracking_options.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7432 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/accounting/models/user.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1520 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/users.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1693 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/accounting/models/validation_error.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.409669 xero_python-1.9.0b3/xero_python/api_client/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    27018 2021-08-31 20:47:24.000000 xero_python-1.9.0b3/xero_python/api_client/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7399 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/api_client/configuration.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9836 2021-08-31 18:09:53.000000 xero_python-1.9.0b3/xero_python/api_client/deserializer.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12122 2021-08-31 20:49:57.000000 xero_python-1.9.0b3/xero_python/api_client/oauth2.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7337 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/api_client/serializer.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.410273 xero_python-1.9.0b3/xero_python/appstore/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      745 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/appstore/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.411757 xero_python-1.9.0b3/xero_python/appstore/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      110 2021-08-31 20:53:02.000000 xero_python-1.9.0b3/xero_python/appstore/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3768 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/api/app_store_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.415940 xero_python-1.9.0b3/xero_python/appstore/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      650 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/appstore/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5006 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/plan.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3237 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/price.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4837 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/problem_details.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4357 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/product.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8651 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/subscription.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6168 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/appstore/models/subscription_item.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.416678 xero_python-1.9.0b3/xero_python/assets/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1335 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.417990 xero_python-1.9.0b3/xero_python/assets/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      101 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17938 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/api/asset_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.425268 xero_python-1.9.0b3/xero_python/assets/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1249 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    15830 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/asset.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      655 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/models/asset_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      665 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/models/asset_status_query_param.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8812 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/asset_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2284 2021-08-31 20:53:03.000000 xero_python-1.9.0b3/xero_python/assets/models/assets.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9196 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/book_depreciation_detail.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11640 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/book_depreciation_setting.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5500 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/error.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6341 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/field_validation_errors_element.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3674 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/pagination.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5539 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/resource_validation_errors_element.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10228 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/assets/models/setting.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.426018 xero_python-1.9.0b3/xero_python/exceptions/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4576 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/exceptions/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2817 2021-07-21 19:32:27.000000 xero_python-1.9.0b3/xero_python/exceptions/http_status_exceptions.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.426356 xero_python-1.9.0b3/xero_python/file/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      820 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/file/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.427283 xero_python-1.9.0b3/xero_python/file/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       99 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    48802 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/file/api/files_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.434764 xero_python-1.9.0b3/xero_python/file/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      736 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/file/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4100 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/models/association.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6863 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/file/models/file_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3382 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/models/files.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4619 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/models/folder.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1513 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/models/folders.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3536 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/file/models/inline_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3554 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/file/models/inline_object1.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      743 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/file/models/object_group.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2188 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/file/models/object_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3879 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/file/models/upload_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4488 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/file/models/user.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.435406 xero_python-1.9.0b3/xero_python/identity/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      586 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/identity/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.437348 xero_python-1.9.0b3/xero_python/identity/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      109 2021-08-31 20:53:04.000000 xero_python-1.9.0b3/xero_python/identity/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      750 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/identity/api/exception_handler.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5626 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/identity/api/identity_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.439484 xero_python-1.9.0b3/xero_python/identity/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      492 2021-08-31 20:52:55.000000 xero_python-1.9.0b3/xero_python/identity/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5143 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/identity/models/access_token.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7188 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/identity/models/connection.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4283 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/identity/models/refresh_token.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1832 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/models.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.440210 xero_python-1.9.0b3/xero_python/payrollau/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6229 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.441471 xero_python-1.9.0b3/xero_python/payrollau/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    82168 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollau/api/payroll_au_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.498049 xero_python-1.9.0b3/xero_python/payrollau/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6131 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3569 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1144 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/account_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      614 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/allowance_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3119 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/api_exception.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6071 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/bank_account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      625 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/calendar_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5380 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/deduction_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9852 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/deduction_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      549 2021-08-31 20:53:05.000000 xero_python-1.9.0b3/xero_python/payrollau/models/deduction_type_calculation_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9487 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    17461 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/earnings_rate.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      588 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/earnings_rate_calculation_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      817 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/earnings_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    32000 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/employee.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      509 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/employee_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1588 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/employees.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      606 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/employment_basis.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      499 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/employment_termination_payment_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      526 2021-08-31 20:53:06.000000 xero_python-1.9.0b3/xero_python/payrollau/models/entitlement_final_pay_payout_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5716 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/home_address.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3669 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_accrual_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9818 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_application.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1839 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_applications.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4494 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3683 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10136 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      696 2021-08-31 20:53:07.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_line_calculation_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1577 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_lines.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4841 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_period.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      516 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_period_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9806 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      596 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/leave_type_contribution_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      634 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/manual_tax_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6856 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/opening_balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4236 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_item.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1560 2021-08-31 20:53:08.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_items.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14719 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_run.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      497 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_run_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1549 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_runs.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5064 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/pay_template.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      655 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payment_frequency_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8385 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payroll_calendar.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1810 2021-08-31 20:53:09.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payroll_calendars.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    16494 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payslip.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8178 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payslip_lines.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1551 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payslip_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10615 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payslip_summary.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1559 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/payslips.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      541 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/rate_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4936 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1868 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_lines.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5612 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      592 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/residency_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3770 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1580 2021-08-31 20:53:10.000000 xero_python-1.9.0b3/xero_python/payrollau/models/settings_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2995 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3257 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3307 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      570 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/state.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12093 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_fund.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4088 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_fund_product.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1858 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_fund_products.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      502 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_fund_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1636 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_funds.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8280 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4068 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/super_membership.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      582 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_calculation_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      601 2021-08-31 20:53:11.000000 xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_contribution_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10003 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    19138 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollau/models/tax_declaration.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6143 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/tax_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      563 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/tfn_exemption_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8712 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/timesheet.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4983 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1609 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      586 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1617 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/timesheets.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1645 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollau/models/validation_error.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.498437 xero_python-1.9.0b3/xero_python/payrollnz/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8007 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.499276 xero_python-1.9.0b3/xero_python/payrollnz/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollnz/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)   197486 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrollnz/api/payroll_nz_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.548674 xero_python-1.9.0b3/xero_python/payrollnz/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7909 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4086 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1552 2021-08-31 20:53:12.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/accounts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5999 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/address.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8594 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/bank_account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10860 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/benefit.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      640 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/calendar_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7308 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/deduction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5257 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/deduction_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/deduction_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/deductions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10566 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5493 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_order.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3304 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_order_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3272 2021-08-31 20:53:13.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_orders.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12582 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rate.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rate_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3135 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6394 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_template.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3295 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_template_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12710 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3375 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_earnings_templates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7801 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4301 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3271 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2980 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10706 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_setup.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3215 2021-08-31 20:53:14.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_setup_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    13344 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3178 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_type_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3146 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2928 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leaves.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2986 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4570 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_opening_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3429 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_opening_balances_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2712 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_template.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3252 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_template_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3182 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_templates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4503 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3442 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8014 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_summary.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    19815 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leave.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3544 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leaves.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    21571 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_tax.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3116 2021-08-31 20:53:15.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employee_tax_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2954 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employees.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3885 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3060 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/employment_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2725 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/gross_earnings_history.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2303 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/invalid_field.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2687 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_accrual_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    10848 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4949 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_period.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2965 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_periods.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6560 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3042 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_type_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3010 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/leave_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3542 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pagination.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11777 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7678 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendar.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3260 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendar_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3228 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendars.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2931 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2899 2021-08-31 20:53:16.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_runs.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    28891 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slip.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2968 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slip_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2936 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slips.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5038 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/payment_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2950 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/payment_method.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/payment_method_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5106 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/problem.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11135 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5447 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3171 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursements.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12190 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wage.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3243 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wage_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3191 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wages.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2902 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5484 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      882 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_category.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4878 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3389 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3357 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deductions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6358 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/superannuation_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3047 2021-08-31 20:53:17.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/superannuation_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3015 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/superannuations.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      739 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/tax_code.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5126 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/tax_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6462 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/tax_settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9649 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11016 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5970 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_line_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/timesheets.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3299 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/tracking_categories.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3679 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrollnz/models/tracking_category.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.549045 xero_python-1.9.0b3/xero_python/payrolluk/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7208 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.550171 xero_python-1.9.0b3/xero_python/payrolluk/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      113 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      614 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/payrolluk/api/exception_handler.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)   202748 2021-08-31 20:53:25.000000 xero_python-1.9.0b3/xero_python/payrolluk/api/payroll_uk_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.605394 xero_python-1.9.0b3/xero_python/payrolluk/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7110 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4175 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1552 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/accounts.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5284 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/address.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3810 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/bank_account.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    15279 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/benefit.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5049 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/benefit_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2949 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/benefit_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2917 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/benefits.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2582 2021-08-31 20:53:18.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/court_order_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    18040 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/deduction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4352 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/deduction_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/deduction_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/deductions.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9494 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5493 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_order.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3304 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_order_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3272 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_orders.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12977 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rate.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rate_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3135 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6394 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_template.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3295 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_template_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    13825 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     7801 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4301 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3271 2021-08-31 20:53:19.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2980 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8210 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3178 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_type_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3146 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2928 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leaves.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2986 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8493 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_opening_balances.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3414 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_opening_balances_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2712 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_template.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3252 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_template_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3305 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_templates.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4503 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_balance.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3442 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8014 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_summary.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    19815 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leave.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3544 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3492 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leaves.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11263 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_tax.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3116 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employee_tax_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2954 2021-08-31 20:53:20.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employees.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4935 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employment.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3060 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/employment_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2303 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/invalid_field.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2687 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_accrual_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6705 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4949 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_period.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2965 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_periods.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8352 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3042 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_type_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3010 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/leave_types.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3542 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pagination.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12379 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     8264 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendar.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3260 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendar_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3228 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendars.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2931 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2899 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/pay_runs.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5038 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payment_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3073 2021-08-31 20:53:21.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payment_method.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payment_method_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    26544 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payslip.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2968 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payslip_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2936 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/payslips.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5106 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/problem.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4599 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3578 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3171 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3153 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursements.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    11173 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wage.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3243 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wage_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3191 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wages.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2902 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/settings.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5484 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/statutory_deduction.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      978 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/statutory_deduction_category.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6148 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/tax_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9565 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     6869 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_earnings_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5970 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_line.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3204 2021-08-31 20:53:22.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_line_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3023 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_object.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2991 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/timesheets.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3299 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/tracking_categories.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3679 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/payrolluk/models/tracking_category.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.605831 xero_python-1.9.0b3/xero_python/project/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1474 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/__init__.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.606669 xero_python-1.9.0b3/xero_python/project/api/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      106 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/api/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    45972 2021-08-31 20:53:24.000000 xero_python-1.9.0b3/xero_python/project/api/project_api.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.616474 xero_python-1.9.0b3/xero_python/project/models/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1383 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/__init__.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2076 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/amount.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      498 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/charge_type.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3047 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/currency_code.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2343 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/error.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4280 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/pagination.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    19641 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4416 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project_create_or_update.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1627 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project_patch.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)      477 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project_status.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2939 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project_user.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2206 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/project_users.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2154 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/projects.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    14338 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/task.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     4437 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/task_create_or_update.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2115 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/tasks.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     2190 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/time_entries.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     9410 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/time_entry.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     5854 2021-08-31 20:53:23.000000 xero_python-1.9.0b3/xero_python/project/models/time_entry_create_or_update.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    12592 2021-08-31 20:53:24.000000 xero_python-1.9.0b3/xero_python/rest.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     3125 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/single_dispatch_str.py
+-rw-r--r--   0 rett.behrens   (501) staff       (20)     1162 2021-04-06 22:02:35.000000 xero_python-1.9.0b3/xero_python/utils.py
+drwxr-xr-x   0 rett.behrens   (501) staff       (20)        0 2021-08-31 21:03:05.264441 xero_python-1.9.0b3/xero_python.egg-info/
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    27051 2021-08-31 21:03:04.000000 xero_python-1.9.0b3/xero_python.egg-info/PKG-INFO
+-rw-r--r--   0 rett.behrens   (501) staff       (20)    24542 2021-08-31 21:03:04.000000 xero_python-1.9.0b3/xero_python.egg-info/SOURCES.txt
+-rw-r--r--   0 rett.behrens   (501) staff       (20)        1 2021-08-31 21:03:04.000000 xero_python-1.9.0b3/xero_python.egg-info/dependency_links.txt
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       37 2021-08-31 21:03:04.000000 xero_python-1.9.0b3/xero_python.egg-info/requires.txt
+-rw-r--r--   0 rett.behrens   (501) staff       (20)       12 2021-08-31 21:03:04.000000 xero_python-1.9.0b3/xero_python.egg-info/top_level.txt
```

### Comparing `xero_python-1.9.0b2/LICENSE` & `xero_python-1.9.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/PKG-INFO` & `xero_python-1.9.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xero_python
-Version: 1.9.0b2
+Version: 1.9.0b3
 Summary: Official Python sdk for Xero API generated by OpenAPI spec for oAuth2
 Home-page: UNKNOWN
 Author: Xero Developer API
 Author-email: api@xero.com
 License: MIT license
 Description: # xero-python
         [![PyPI version](https://badge.fury.io/py/xero-python.svg)](https://badge.fury.io/py/xero-python)
```

### Comparing `xero_python-1.9.0b2/README.md` & `xero_python-1.9.0b3/README.md`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/setup.py` & `xero_python-1.9.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     license="MIT license",
     long_description="\n\n".join((read_file("README.md"), read_file("HISTORY.md"))),
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="xero python sdk API oAuth",
     name="xero_python",
     packages=find_packages(include=["xero_python", "xero_python.*"]),
-    version="1.9.0b2",
+    version="1.9.0b3",
 )
```

### Comparing `xero_python-1.9.0b2/tests/accounting/api/cassettes/test_get_organisations.yaml` & `xero_python-1.9.0b3/tests/accounting/api/cassettes/test_get_organisations.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml` & `xero_python-1.9.0b3/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/accounting/api/fixtures/inv-0032.pdf` & `xero_python-1.9.0b3/tests/accounting/api/fixtures/inv-0032.pdf`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/accounting/api/test_accounting_api.py` & `xero_python-1.9.0b3/tests/accounting/api/test_accounting_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/cassettes/test_vcr.yaml` & `xero_python-1.9.0b3/tests/cassettes/test_vcr.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/conftest.py` & `xero_python-1.9.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/identity/api/cassettes/test_get_connections.yaml` & `xero_python-1.9.0b3/tests/identity/api/cassettes/test_get_connections.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/identity/api/test_identity_api.py` & `xero_python-1.9.0b3/tests/identity/api/test_identity_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/__init__.py` & `xero_python-1.9.0b3/tests/test_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml` & `xero_python-1.9.0b3/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml` & `xero_python-1.9.0b3/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/test_deserializer.py` & `xero_python-1.9.0b3/tests/test_api_client/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/test_oauth2.py` & `xero_python-1.9.0b3/tests/test_api_client/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_api_client/test_serializer.py` & `xero_python-1.9.0b3/tests/test_api_client/test_serializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_executor.py` & `xero_python-1.9.0b3/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/tests/test_single_dispatch_str.py` & `xero_python-1.9.0b3/tests/test_single_dispatch_str.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/__init__.py` & `xero_python-1.9.0b3/xero_python/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/api/accounting_api.py` & `xero_python-1.9.0b3/xero_python/accounting/api/accounting_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/api/exception_handler.py` & `xero_python-1.9.0b3/xero_python/accounting/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/__init__.py` & `xero_python-1.9.0b3/xero_python/accounting/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/account.py` & `xero_python-1.9.0b3/xero_python/accounting/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/account_type.py` & `xero_python-1.9.0b3/xero_python/accounting/models/account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/accounts.py` & `xero_python-1.9.0b3/xero_python/accounting/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/accounts_payable.py` & `xero_python-1.9.0b3/xero_python/accounting/models/accounts_payable.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/accounts_receivable.py` & `xero_python-1.9.0b3/xero_python/accounting/models/accounts_receivable.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/action.py` & `xero_python-1.9.0b3/xero_python/accounting/models/action.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/actions.py` & `xero_python-1.9.0b3/xero_python/accounting/models/actions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/address.py` & `xero_python-1.9.0b3/xero_python/accounting/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/address_for_organisation.py` & `xero_python-1.9.0b3/xero_python/accounting/models/address_for_organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/allocation.py` & `xero_python-1.9.0b3/xero_python/accounting/models/allocation.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/allocations.py` & `xero_python-1.9.0b3/xero_python/accounting/models/allocations.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/attachment.py` & `xero_python-1.9.0b3/xero_python/accounting/models/attachment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/attachments.py` & `xero_python-1.9.0b3/xero_python/accounting/models/attachments.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/balance_details.py` & `xero_python-1.9.0b3/xero_python/accounting/models/balance_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/balances.py` & `xero_python-1.9.0b3/xero_python/accounting/models/balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/bank_transaction.py` & `xero_python-1.9.0b3/xero_python/accounting/models/bank_transaction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/bank_transactions.py` & `xero_python-1.9.0b3/xero_python/accounting/models/bank_transactions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/bank_transfer.py` & `xero_python-1.9.0b3/xero_python/accounting/models/bank_transfer.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/bank_transfers.py` & `xero_python-1.9.0b3/xero_python/accounting/models/bank_transfers.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/batch_payment.py` & `xero_python-1.9.0b3/xero_python/accounting/models/batch_payment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/batch_payment_details.py` & `xero_python-1.9.0b3/xero_python/accounting/models/batch_payment_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/batch_payments.py` & `xero_python-1.9.0b3/xero_python/accounting/models/batch_payments.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/bill.py` & `xero_python-1.9.0b3/xero_python/accounting/models/bill.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/branding_theme.py` & `xero_python-1.9.0b3/xero_python/accounting/models/branding_theme.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/branding_themes.py` & `xero_python-1.9.0b3/xero_python/accounting/models/branding_themes.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/budget.py` & `xero_python-1.9.0b3/xero_python/accounting/models/budget.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/budget_balance.py` & `xero_python-1.9.0b3/xero_python/accounting/models/budget_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/budget_line.py` & `xero_python-1.9.0b3/xero_python/accounting/models/budget_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/budget_lines.py` & `xero_python-1.9.0b3/xero_python/accounting/models/budget_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/budgets.py` & `xero_python-1.9.0b3/xero_python/accounting/models/budgets.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/cis_org_setting.py` & `xero_python-1.9.0b3/xero_python/accounting/models/cis_org_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/cis_org_settings.py` & `xero_python-1.9.0b3/xero_python/accounting/models/cis_org_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/cis_setting.py` & `xero_python-1.9.0b3/xero_python/accounting/models/cis_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/cis_settings.py` & `xero_python-1.9.0b3/xero_python/accounting/models/cis_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/contact.py` & `xero_python-1.9.0b3/xero_python/accounting/models/contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/contact_group.py` & `xero_python-1.9.0b3/xero_python/accounting/models/contact_group.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/contact_groups.py` & `xero_python-1.9.0b3/xero_python/accounting/models/contact_groups.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/contact_person.py` & `xero_python-1.9.0b3/xero_python/accounting/models/contact_person.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/contacts.py` & `xero_python-1.9.0b3/xero_python/accounting/models/contacts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/conversion_balances.py` & `xero_python-1.9.0b3/xero_python/accounting/models/conversion_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/conversion_date.py` & `xero_python-1.9.0b3/xero_python/accounting/models/conversion_date.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/country_code.py` & `xero_python-1.9.0b3/xero_python/accounting/models/country_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/credit_note.py` & `xero_python-1.9.0b3/xero_python/accounting/models/credit_note.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/credit_notes.py` & `xero_python-1.9.0b3/xero_python/accounting/models/credit_notes.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/currencies.py` & `xero_python-1.9.0b3/xero_python/accounting/models/currencies.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/currency.py` & `xero_python-1.9.0b3/xero_python/accounting/models/currency.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/currency_code.py` & `xero_python-1.9.0b3/xero_python/accounting/models/currency_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/element.py` & `xero_python-1.9.0b3/xero_python/accounting/models/element.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/employee.py` & `xero_python-1.9.0b3/xero_python/accounting/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/employees.py` & `xero_python-1.9.0b3/xero_python/accounting/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/error.py` & `xero_python-1.9.0b3/xero_python/accounting/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/expense_claim.py` & `xero_python-1.9.0b3/xero_python/accounting/models/expense_claim.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/expense_claims.py` & `xero_python-1.9.0b3/xero_python/accounting/models/expense_claims.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/external_link.py` & `xero_python-1.9.0b3/xero_python/accounting/models/external_link.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/history_record.py` & `xero_python-1.9.0b3/xero_python/accounting/models/history_record.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/history_records.py` & `xero_python-1.9.0b3/xero_python/accounting/models/history_records.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/import_summary.py` & `xero_python-1.9.0b3/xero_python/accounting/models/import_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/import_summary_accounts.py` & `xero_python-1.9.0b3/xero_python/accounting/models/import_summary_accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/import_summary_object.py` & `xero_python-1.9.0b3/xero_python/accounting/models/import_summary_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/import_summary_organisation.py` & `xero_python-1.9.0b3/xero_python/accounting/models/import_summary_organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/invoice.py` & `xero_python-1.9.0b3/xero_python/accounting/models/invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/invoice_reminder.py` & `xero_python-1.9.0b3/xero_python/accounting/models/invoice_reminder.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/invoice_reminders.py` & `xero_python-1.9.0b3/xero_python/accounting/models/invoice_reminders.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/invoices.py` & `xero_python-1.9.0b3/xero_python/accounting/models/invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/item.py` & `xero_python-1.9.0b3/xero_python/accounting/models/item.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/items.py` & `xero_python-1.9.0b3/xero_python/accounting/models/items.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/journal.py` & `xero_python-1.9.0b3/xero_python/accounting/models/journal.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/journal_line.py` & `xero_python-1.9.0b3/xero_python/accounting/models/journal_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/journals.py` & `xero_python-1.9.0b3/xero_python/accounting/models/journals.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/line_amount_types.py` & `xero_python-1.9.0b3/xero_python/accounting/models/line_amount_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/line_item.py` & `xero_python-1.9.0b3/xero_python/accounting/models/line_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/line_item_tracking.py` & `xero_python-1.9.0b3/xero_python/accounting/models/line_item_tracking.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/linked_transaction.py` & `xero_python-1.9.0b3/xero_python/accounting/models/linked_transaction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/linked_transactions.py` & `xero_python-1.9.0b3/xero_python/accounting/models/linked_transactions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/manual_journal.py` & `xero_python-1.9.0b3/xero_python/accounting/models/manual_journal.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/manual_journal_line.py` & `xero_python-1.9.0b3/xero_python/accounting/models/manual_journal_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/manual_journals.py` & `xero_python-1.9.0b3/xero_python/accounting/models/manual_journals.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/online_invoice.py` & `xero_python-1.9.0b3/xero_python/accounting/models/online_invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/online_invoices.py` & `xero_python-1.9.0b3/xero_python/accounting/models/online_invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/organisation.py` & `xero_python-1.9.0b3/xero_python/accounting/models/organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/organisations.py` & `xero_python-1.9.0b3/xero_python/accounting/models/organisations.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/overpayment.py` & `xero_python-1.9.0b3/xero_python/accounting/models/overpayment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/overpayments.py` & `xero_python-1.9.0b3/xero_python/accounting/models/overpayments.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment_delete.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment_delete.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment_service.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment_service.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment_services.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment_services.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment_term.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment_term.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payment_term_type.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payment_term_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/payments.py` & `xero_python-1.9.0b3/xero_python/accounting/models/payments.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/phone.py` & `xero_python-1.9.0b3/xero_python/accounting/models/phone.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/prepayment.py` & `xero_python-1.9.0b3/xero_python/accounting/models/prepayment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/prepayments.py` & `xero_python-1.9.0b3/xero_python/accounting/models/prepayments.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/purchase.py` & `xero_python-1.9.0b3/xero_python/accounting/models/purchase.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/purchase_order.py` & `xero_python-1.9.0b3/xero_python/accounting/models/purchase_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/purchase_orders.py` & `xero_python-1.9.0b3/xero_python/accounting/models/purchase_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/quote.py` & `xero_python-1.9.0b3/xero_python/accounting/models/quote.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/quote_line_amount_types.py` & `xero_python-1.9.0b3/xero_python/accounting/models/quote_line_amount_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/quote_status_codes.py` & `xero_python-1.9.0b3/xero_python/accounting/models/quote_status_codes.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/quotes.py` & `xero_python-1.9.0b3/xero_python/accounting/models/quotes.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/receipt.py` & `xero_python-1.9.0b3/xero_python/accounting/models/receipt.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/receipts.py` & `xero_python-1.9.0b3/xero_python/accounting/models/receipts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/repeating_invoice.py` & `xero_python-1.9.0b3/xero_python/accounting/models/repeating_invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/repeating_invoices.py` & `xero_python-1.9.0b3/xero_python/accounting/models/repeating_invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_attribute.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_attribute.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_cell.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_cell.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_fields.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_fields.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_row.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_row.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_rows.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_rows.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_with_row.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_with_row.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/report_with_rows.py` & `xero_python-1.9.0b3/xero_python/accounting/models/report_with_rows.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/reports.py` & `xero_python-1.9.0b3/xero_python/accounting/models/reports.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/request_empty.py` & `xero_python-1.9.0b3/xero_python/accounting/models/request_empty.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/row_type.py` & `xero_python-1.9.0b3/xero_python/accounting/models/row_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/sales_tracking_category.py` & `xero_python-1.9.0b3/xero_python/accounting/models/sales_tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/schedule.py` & `xero_python-1.9.0b3/xero_python/accounting/models/schedule.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/setup.py` & `xero_python-1.9.0b3/xero_python/accounting/models/setup.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tax_component.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tax_component.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tax_rate.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tax_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tax_rates.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tax_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tax_type.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tax_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/ten_ninety_nine_contact.py` & `xero_python-1.9.0b3/xero_python/accounting/models/ten_ninety_nine_contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/ten_nintey_nine_contact.py` & `xero_python-1.9.0b3/xero_python/accounting/models/ten_nintey_nine_contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/time_zone.py` & `xero_python-1.9.0b3/xero_python/accounting/models/time_zone.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tracking_categories.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tracking_category.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tracking_option.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tracking_option.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/tracking_options.py` & `xero_python-1.9.0b3/xero_python/accounting/models/tracking_options.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/user.py` & `xero_python-1.9.0b3/xero_python/accounting/models/user.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/users.py` & `xero_python-1.9.0b3/xero_python/accounting/models/users.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/accounting/models/validation_error.py` & `xero_python-1.9.0b3/xero_python/accounting/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/api_client/__init__.py` & `xero_python-1.9.0b3/xero_python/api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,21 +754,21 @@
         :return: empty oauth2 token
         """
         oauth2_token = self.configuration.oauth2_token
         oauth2_token.update_token(**self.get_oauth2_token())
         if oauth2_token.revoke_access_token(self):
             return self.get_oauth2_token()
 
-    def get_client_credentials_token(self):
+    def get_client_credentials_token(self, app_store_billing=False):
         """
         Obtain oauth2 token using client credentials grant type
         :return: oauth2 token
         """
         oauth2_token = self.configuration.oauth2_token
-        if oauth2_token.get_client_credentials_access_token(self):
+        if oauth2_token.get_client_credentials_access_token(self, app_store_billing):
             return self.get_oauth2_token()
 
     def oauth2_token_getter(self, token_getter):
         """
         A decorator to register a callback function for getting oauth2 token
 
         It is necessary for token synchronisation across the application code.
```

### Comparing `xero_python-1.9.0b2/xero_python/api_client/configuration.py` & `xero_python-1.9.0b3/xero_python/api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/api_client/deserializer.py` & `xero_python-1.9.0b3/xero_python/api_client/deserializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/api_client/oauth2.py` & `xero_python-1.9.0b3/xero_python/api_client/oauth2.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,24 +77,26 @@
         if status != 200:
             # todo improve error handling
             raise Exception(
                 "refresh token status {} {} {!r}".format(status, response, headers)
             )
         return status
 
-    def get_client_credentials_token(self):
+    def get_client_credentials_token(self, app_store_billing):
         """
         Call Xero Identity API to obtain an access token via OAuth2 Client Credentails grant type
         :return: dictionary with new auth2 token
         """
         post_data = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "grant_type": "client_credentials",
         }
+        if app_store_billing:
+            post_data["scope"] = "marketplace.billing"
         response, status, headers = self.api_client.call_api(
             self.client_credentials_token_url,
             "POST",
             header_params={
                 "Accept": "application/json",
                 "Content-Type": "application/x-www-form-urlencoded",
             },
@@ -227,22 +229,22 @@
             return False
         token_api = TokenApi(api_client, self.client_id, self.client_secret)
         new_token = self.fetch_access_token(token_api)
         self.update_token(**new_token)
         api_client.set_oauth2_token(new_token)
         return True
 
-    def get_client_credentials_access_token(self, api_client):
+    def get_client_credentials_access_token(self, api_client, app_store_billing):
         """
         Perform OAuth2 Client Credentials grant token request.
         :param api_client:  ApiClient instance used to perform refresh token API call.
         :return: bool - True if success
         """
         token_api = TokenApi(api_client, self.client_id, self.client_secret)
-        new_token = token_api.get_client_credentials_token()
+        new_token = token_api.get_client_credentials_token(app_store_billing)
         self.update_token(**new_token)
         api_client.set_oauth2_token(new_token)
         return True
 
     def revoke_access_token(self, api_client):
         """
         Perform auth2 revoke token call.
```

### Comparing `xero_python-1.9.0b2/xero_python/api_client/serializer.py` & `xero_python-1.9.0b3/xero_python/api_client/serializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/__init__.py` & `xero_python-1.9.0b3/xero_python/appstore/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/api/app_store_api.py` & `xero_python-1.9.0b3/xero_python/appstore/api/app_store_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/__init__.py` & `xero_python-1.9.0b3/xero_python/appstore/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/plan.py` & `xero_python-1.9.0b3/xero_python/appstore/models/plan.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/price.py` & `xero_python-1.9.0b3/xero_python/appstore/models/price.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/problem_details.py` & `xero_python-1.9.0b3/xero_python/appstore/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/product.py` & `xero_python-1.9.0b3/xero_python/appstore/models/product.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/subscription.py` & `xero_python-1.9.0b3/xero_python/appstore/models/subscription.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/appstore/models/subscription_item.py` & `xero_python-1.9.0b3/xero_python/appstore/models/subscription_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/__init__.py` & `xero_python-1.9.0b3/xero_python/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/api/asset_api.py` & `xero_python-1.9.0b3/xero_python/assets/api/asset_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/__init__.py` & `xero_python-1.9.0b3/xero_python/assets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/asset.py` & `xero_python-1.9.0b3/xero_python/assets/models/asset.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/asset_status.py` & `xero_python-1.9.0b3/xero_python/assets/models/asset_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/asset_status_query_param.py` & `xero_python-1.9.0b3/xero_python/assets/models/asset_status_query_param.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/asset_type.py` & `xero_python-1.9.0b3/xero_python/assets/models/asset_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/assets.py` & `xero_python-1.9.0b3/xero_python/assets/models/assets.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/book_depreciation_detail.py` & `xero_python-1.9.0b3/xero_python/assets/models/book_depreciation_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/book_depreciation_setting.py` & `xero_python-1.9.0b3/xero_python/assets/models/book_depreciation_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/error.py` & `xero_python-1.9.0b3/xero_python/assets/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/field_validation_errors_element.py` & `xero_python-1.9.0b3/xero_python/assets/models/field_validation_errors_element.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/pagination.py` & `xero_python-1.9.0b3/xero_python/assets/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/resource_validation_errors_element.py` & `xero_python-1.9.0b3/xero_python/assets/models/resource_validation_errors_element.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/assets/models/setting.py` & `xero_python-1.9.0b3/xero_python/assets/models/setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/exceptions/__init__.py` & `xero_python-1.9.0b3/xero_python/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/exceptions/http_status_exceptions.py` & `xero_python-1.9.0b3/xero_python/exceptions/http_status_exceptions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/__init__.py` & `xero_python-1.9.0b3/xero_python/file/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/api/files_api.py` & `xero_python-1.9.0b3/xero_python/file/api/files_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/__init__.py` & `xero_python-1.9.0b3/xero_python/file/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/association.py` & `xero_python-1.9.0b3/xero_python/file/models/association.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/file_object.py` & `xero_python-1.9.0b3/xero_python/file/models/file_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/files.py` & `xero_python-1.9.0b3/xero_python/file/models/files.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/folder.py` & `xero_python-1.9.0b3/xero_python/file/models/folder.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/folders.py` & `xero_python-1.9.0b3/xero_python/file/models/folders.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/inline_object.py` & `xero_python-1.9.0b3/xero_python/file/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/inline_object1.py` & `xero_python-1.9.0b3/xero_python/file/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/object_group.py` & `xero_python-1.9.0b3/xero_python/file/models/object_group.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/object_type.py` & `xero_python-1.9.0b3/xero_python/file/models/object_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/upload_object.py` & `xero_python-1.9.0b3/xero_python/file/models/upload_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/file/models/user.py` & `xero_python-1.9.0b3/xero_python/file/models/user.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/__init__.py` & `xero_python-1.9.0b3/xero_python/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/api/exception_handler.py` & `xero_python-1.9.0b3/xero_python/identity/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/api/identity_api.py` & `xero_python-1.9.0b3/xero_python/identity/api/identity_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/models/access_token.py` & `xero_python-1.9.0b3/xero_python/identity/models/access_token.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/models/connection.py` & `xero_python-1.9.0b3/xero_python/identity/models/connection.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/identity/models/refresh_token.py` & `xero_python-1.9.0b3/xero_python/identity/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/models.py` & `xero_python-1.9.0b3/xero_python/models.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/__init__.py` & `xero_python-1.9.0b3/xero_python/payrollau/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/api/payroll_au_api.py` & `xero_python-1.9.0b3/xero_python/payrollau/api/payroll_au_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/__init__.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/account.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/account_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/allowance_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/allowance_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/api_exception.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/api_exception.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/bank_account.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/calendar_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/calendar_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/deduction_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/deduction_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/deduction_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/deduction_type_calculation_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/deduction_type_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/earnings_rate.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/earnings_rate_calculation_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/earnings_rate_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/earnings_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/earnings_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/employee.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/employees.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/employment_basis.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/employment_basis.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/entitlement_final_pay_payout_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/entitlement_final_pay_payout_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/home_address.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/home_address.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_accrual_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_application.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_application.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_applications.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_applications.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_balance.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_line_calculation_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_line_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_lines.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_period.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_period_status.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_period_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/leave_type_contribution_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/leave_type_contribution_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/manual_tax_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/manual_tax_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/opening_balances.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/opening_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/pay_item.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/pay_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/pay_items.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/pay_items.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/pay_run.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/pay_runs.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/pay_template.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payment_frequency_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payment_frequency_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payroll_calendar.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payroll_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payroll_calendars.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payroll_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payslip.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payslip.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payslip_lines.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payslip_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payslip_object.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payslip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payslip_summary.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payslip_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/payslips.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/payslips.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/rate_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/rate_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_lines.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/reimbursement_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/reimbursement_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/residency_status.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/residency_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/settings.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/settings_object.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/settings_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/state.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/state.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_fund.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_fund.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_fund_product.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_fund_product.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_fund_products.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_fund_products.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_funds.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_funds.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/super_membership.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/super_membership.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_calculation_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_contribution_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_contribution_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/superannuation_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/superannuation_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/tax_declaration.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/tax_declaration.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/tax_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/tfn_exemption_type.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/tfn_exemption_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/timesheet.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_line.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_object.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/timesheet_status.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/timesheet_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/timesheets.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollau/models/validation_error.py` & `xero_python-1.9.0b3/xero_python/payrollau/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/__init__.py` & `xero_python-1.9.0b3/xero_python/payrollnz/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/api/payroll_nz_api.py` & `xero_python-1.9.0b3/xero_python/payrollnz/api/payroll_nz_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/__init__.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/account.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/accounts.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/address.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/bank_account.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/benefit.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/benefit.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/calendar_type.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/calendar_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/deduction.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/deduction_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/deduction_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/deductions.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_order.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_order_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_order_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_orders.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rate.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rate_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rate_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_rates.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_template.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/earnings_template_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/earnings_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_earnings_templates.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_earnings_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_balance.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_balances.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_setup.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_setup.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_setup_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_setup_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_type.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_type_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leave_types.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_leaves.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_opening_balance.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_opening_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_opening_balances_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_opening_balances_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_template.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_template_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_pay_templates.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_pay_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_balance.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leave_summary.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leave_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leave.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_statutory_sick_leaves.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_statutory_sick_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_tax.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_tax.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employee_tax_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employee_tax_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employees.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employment.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/employment_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/employment_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/gross_earnings_history.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/gross_earnings_history.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/invalid_field.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/invalid_field.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_accrual_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_period.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_periods.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_periods.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_type.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_type_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/leave_types.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pagination.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendar.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendar_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendar_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_calendars.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_run_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_run_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_runs.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slip.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slip.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slip_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/pay_slips.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/pay_slips.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/payment_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/payment_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/payment_method.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/payment_method_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/payment_method_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/problem.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/problem.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursement_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursement_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/reimbursements.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/reimbursements.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wage.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wage.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wage_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wage_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/salary_and_wages.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/salary_and_wages.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/settings.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_category.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deduction_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/statutory_deductions.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/statutory_deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/superannuation_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/superannuation_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/superannuation_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/superannuation_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/superannuations.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/superannuations.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/tax_code.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/tax_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/tax_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/tax_settings.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/tax_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_line.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_line_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_line_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheet_object.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/timesheets.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/tracking_categories.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrollnz/models/tracking_category.py` & `xero_python-1.9.0b3/xero_python/payrollnz/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/__init__.py` & `xero_python-1.9.0b3/xero_python/payrolluk/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/api/exception_handler.py` & `xero_python-1.9.0b3/xero_python/payrolluk/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/api/payroll_uk_api.py` & `xero_python-1.9.0b3/xero_python/payrolluk/api/payroll_uk_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/__init__.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/account.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/accounts.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/address.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/bank_account.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/benefit.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/benefit.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/benefit_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/benefit_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/benefit_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/benefit_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/benefits.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/benefits.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/court_order_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/court_order_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/deduction.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/deduction_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/deduction_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/deductions.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_order.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_order_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_order_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_orders.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rate.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rate_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rate_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_rates.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_template.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/earnings_template_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/earnings_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_balance.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_balances.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_type.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_type_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leave_types.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_leaves.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_opening_balances.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_opening_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_opening_balances_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_opening_balances_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_template.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_template_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_pay_templates.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_pay_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_balance.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leave_summary.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leave_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leave.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_statutory_sick_leaves.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_statutory_sick_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_tax.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_tax.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employee_tax_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employee_tax_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employees.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employment.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employment.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/employment_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/employment_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/invalid_field.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/invalid_field.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_accrual_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_period.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_periods.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_periods.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_type.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_type_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/leave_types.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pagination.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendar.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendar_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendar_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_calendars.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_run_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_run_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/pay_runs.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payment_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payment_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payment_method.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payment_method_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payment_method_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payslip.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payslip.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payslip_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payslip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/payslips.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/payslips.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/problem.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/problem.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursement_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursement_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/reimbursements.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/reimbursements.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wage.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wage.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wage_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wage_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/salary_and_wages.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/salary_and_wages.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/settings.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/statutory_deduction.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/statutory_deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/statutory_deduction_category.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/statutory_deduction_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/tax_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_earnings_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_line.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_line_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_line_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheet_object.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/timesheets.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/tracking_categories.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/payrolluk/models/tracking_category.py` & `xero_python-1.9.0b3/xero_python/payrolluk/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/__init__.py` & `xero_python-1.9.0b3/xero_python/project/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/api/project_api.py` & `xero_python-1.9.0b3/xero_python/project/api/project_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/__init__.py` & `xero_python-1.9.0b3/xero_python/project/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/amount.py` & `xero_python-1.9.0b3/xero_python/project/models/amount.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/currency_code.py` & `xero_python-1.9.0b3/xero_python/project/models/currency_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/error.py` & `xero_python-1.9.0b3/xero_python/project/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/pagination.py` & `xero_python-1.9.0b3/xero_python/project/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/project.py` & `xero_python-1.9.0b3/xero_python/project/models/project.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/project_create_or_update.py` & `xero_python-1.9.0b3/xero_python/project/models/project_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/project_patch.py` & `xero_python-1.9.0b3/xero_python/project/models/project_patch.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/project_user.py` & `xero_python-1.9.0b3/xero_python/project/models/project_user.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/project_users.py` & `xero_python-1.9.0b3/xero_python/project/models/project_users.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/projects.py` & `xero_python-1.9.0b3/xero_python/project/models/projects.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/task.py` & `xero_python-1.9.0b3/xero_python/project/models/task.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/task_create_or_update.py` & `xero_python-1.9.0b3/xero_python/project/models/task_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/tasks.py` & `xero_python-1.9.0b3/xero_python/project/models/tasks.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/time_entries.py` & `xero_python-1.9.0b3/xero_python/project/models/time_entries.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/time_entry.py` & `xero_python-1.9.0b3/xero_python/project/models/time_entry.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/project/models/time_entry_create_or_update.py` & `xero_python-1.9.0b3/xero_python/project/models/time_entry_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/rest.py` & `xero_python-1.9.0b3/xero_python/rest.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/single_dispatch_str.py` & `xero_python-1.9.0b3/xero_python/single_dispatch_str.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python/utils.py` & `xero_python-1.9.0b3/xero_python/utils.py`

 * *Files identical despite different names*

### Comparing `xero_python-1.9.0b2/xero_python.egg-info/PKG-INFO` & `xero_python-1.9.0b3/xero_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xero-python
-Version: 1.9.0b2
+Version: 1.9.0b3
 Summary: Official Python sdk for Xero API generated by OpenAPI spec for oAuth2
 Home-page: UNKNOWN
 Author: Xero Developer API
 Author-email: api@xero.com
 License: MIT license
 Description: # xero-python
         [![PyPI version](https://badge.fury.io/py/xero-python.svg)](https://badge.fury.io/py/xero-python)
```

### Comparing `xero_python-1.9.0b2/xero_python.egg-info/SOURCES.txt` & `xero_python-1.9.0b3/xero_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

