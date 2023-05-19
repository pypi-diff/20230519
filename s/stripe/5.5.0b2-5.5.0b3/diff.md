# Comparing `tmp/stripe-5.5.0b2.tar.gz` & `tmp/stripe-5.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe-5.5.0b2.tar", last modified: Thu Apr 13 16:01:10 2023, max compression
+gzip compressed data, was "stripe-5.5.0b3.tar", last modified: Fri May 19 17:20:18 2023, max compression
```

## Comparing `stripe-5.5.0b2.tar` & `stripe-5.5.0b3.tar`

### file list

```diff
@@ -1,329 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.311277 stripe-5.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 16:00:51.000000 stripe-5.5.0b2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 16:00:51.000000 stripe-5.5.0b2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    47187 2023-04-13 16:00:51.000000 stripe-5.5.0b2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-13 16:00:51.000000 stripe-5.5.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-13 16:00:51.000000 stripe-5.5.0b2/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-13 16:00:51.000000 stripe-5.5.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-13 16:01:10.311277 stripe-5.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-13 16:00:51.000000 stripe-5.5.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 16:00:51.000000 stripe-5.5.0b2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.271277 stripe-5.5.0b2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-13 16:00:51.000000 stripe-5.5.0b2/examples/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 16:00:51.000000 stripe-5.5.0b2/examples/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-13 16:00:51.000000 stripe-5.5.0b2/examples/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-13 16:00:51.000000 stripe-5.5.0b2/examples/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 16:00:51.000000 stripe-5.5.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 16:01:10.311277 stripe-5.5.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-13 16:00:51.000000 stripe-5.5.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.275277 stripe-5.5.0b2/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.283277 stripe-5.5.0b2/stripe/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/abstract/verify_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/account_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/application_fee_refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/apps/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/bank_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/billing_portal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/billing_portal/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/capability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/capital/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/capital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/capital/financing_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/capital/financing_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/capital/financing_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/cash_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/charge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/checkout/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/credit_note_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/customer_cash_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/error_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/file_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/financial_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/account_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/account_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/inferred_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/financial_connections/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/funding_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/gift_cards/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/gift_cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/gift_cards/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/gift_cards/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.287277 stripe-5.5.0b2/stripe/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/identity/verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/identity/verification_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/invoice_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/card_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/card_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/issuing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/login_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/quote_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/radar/early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/radar/value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/radar/value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/recipient_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/reporting/report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/reporting/report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/shipping_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/sigma/scheduled_query_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/subscription_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/terminal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/terminal/connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/terminal/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/terminal/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.291277 stripe-5.5.0b2/stripe/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/test_helpers/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.295277 stripe-5.5.0b2/stripe/api_resources/treasury/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/credit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/debit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/financial_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/inbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/outbound_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/outbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/received_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/received_debit.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/treasury/transaction_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_resources/webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.295277 stripe-5.5.0b2/stripe/data/
--rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/data/ca-certificates.crt
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/request_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-13 16:00:51.000000 stripe-5.5.0b2/stripe/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.275277 stripe-5.5.0b2/stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 16:01:10.000000 stripe-5.5.0b2/stripe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.299277 stripe-5.5.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_test_helpers_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/abstract/test_updateable_api_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/billing_portal/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/billing_portal/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/checkout/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/identity/test_verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/identity/test_verification_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.307277 stripe-5.5.0b2/tests/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/test_cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/issuing/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.311277 stripe-5.5.0b2/tests/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/radar/test_early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/radar/test_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/radar/test_value_list_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.311277 stripe-5.5.0b2/tests/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/reporting/test_report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/reporting/test_report_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.311277 stripe-5.5.0b2/tests/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/sigma/test_scheduled_query_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:01:10.311277 stripe-5.5.0b2/tests/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/terminal/test_connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/terminal/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/terminal/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_application_fee_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_file_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_subscription_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/api_resources/test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/stripe_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    26116 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    94469 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_generated_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 16:00:51.000000 stripe-5.5.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 17:19:54.000000 stripe-5.5.0b3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-19 17:19:54.000000 stripe-5.5.0b3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    47658 2023-05-19 17:19:54.000000 stripe-5.5.0b3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-19 17:19:54.000000 stripe-5.5.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 17:19:54.000000 stripe-5.5.0b3/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 17:19:54.000000 stripe-5.5.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-19 17:20:18.415509 stripe-5.5.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-05-19 17:19:54.000000 stripe-5.5.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 17:19:54.000000 stripe-5.5.0b3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.375510 stripe-5.5.0b3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-19 17:19:54.000000 stripe-5.5.0b3/examples/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-19 17:19:54.000000 stripe-5.5.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 17:20:18.415509 stripe-5.5.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-19 17:19:54.000000 stripe-5.5.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.379510 stripe-5.5.0b3/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.387509 stripe-5.5.0b3/stripe/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/abstract/verify_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/account_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/application_fee_refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/apps/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/bank_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/billing_portal/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/capital/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/capital/financing_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/cash_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/charge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/checkout/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/credit_note_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/customer_cash_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/error_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/file_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/financial_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/account_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/inferred_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/financial_connections/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/funding_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.391509 stripe-5.5.0b3/stripe/api_resources/gift_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/gift_cards/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/identity/verification_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/invoice_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/card_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/issuing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/login_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/quote_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/radar/value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/recipient_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reporting/report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/shipping_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/sigma/scheduled_query_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/subscription_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.395510 stripe-5.5.0b3/stripe/api_resources/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/terminal/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/test_helpers/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/api_resources/treasury/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/credit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/debit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/financial_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/inbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/outbound_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/outbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/received_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/received_debit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/treasury/transaction_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_resources/webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/api_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.399510 stripe-5.5.0b3/stripe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/data/ca-certificates.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/request_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-19 17:19:54.000000 stripe-5.5.0b3/stripe/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.379510 stripe-5.5.0b3/stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 17:20:18.000000 stripe-5.5.0b3/stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.403509 stripe-5.5.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/abstract/test_updateable_api_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/billing_portal/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/checkout/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.411509 stripe-5.5.0b3/tests/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/identity/test_verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/identity/test_verification_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/issuing/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/radar/test_value_list_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/test_report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/reporting/test_report_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/sigma/test_scheduled_query_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:20:18.415509 stripe-5.5.0b3/tests/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/terminal/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_application_fee_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_subscription_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/api_resources/test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/stripe_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25396 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102848 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_generated_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-19 17:19:54.000000 stripe-5.5.0b3/tox.ini
```

### Comparing `stripe-5.5.0b2/CHANGELOG.md` & `stripe-5.5.0b3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # Changelog
 
+## 5.5.0b3 - 2023-05-19
+* [#966](https://github.com/stripe/stripe-python/pull/966) Update generated code for beta
+  * Add support for `subscribe` and `unsubscribe` methods on resource `FinancialConnections.Account`
+* [#965](https://github.com/stripe/stripe-python/pull/965) Add raw_request
+* [#964](https://github.com/stripe/stripe-python/pull/964) Update generated code for beta
+* [#961](https://github.com/stripe/stripe-python/pull/961) Update generated code for beta
+
+
 ## 5.5.0b2 - 2023-04-13
 * [#954](https://github.com/stripe/stripe-python/pull/954) Update generated code for beta
   * Add support for `collect_payment_method` and `confirm_payment_intent` methods on resource `Terminal.Reader`
 * [#953](https://github.com/stripe/stripe-python/pull/953) Update generated code for beta
 
 
 ## 5.5.0b1 - 2023-03-30
 * [#950](https://github.com/stripe/stripe-python/pull/950) Update generated code for beta
 
 
 ## 5.4.0 - 2023-03-30
 * [#951](https://github.com/stripe/stripe-python/pull/951) Update generated code
-  * Remove support for `create` method on resource `Tax.Transaction`
+  * Remove support for `create` method on resource `Tax.Transaction`
     * This is not a breaking change, as this method was deprecated before the Tax Transactions API was released in favor of the `create_from_calculation` method.
 
 ## 5.4.0b1 - 2023-03-23
 * [#941](https://github.com/stripe/stripe-python/pull/941) Update generated code for beta (new)
   * Add support for new resources `Tax.CalculationLineItem` and `Tax.TransactionLineItem`
   * Add support for `collect_inputs` method on resource `Terminal.Reader`
```

### Comparing `stripe-5.5.0b2/LICENSE` & `stripe-5.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/LONG_DESCRIPTION.rst` & `stripe-5.5.0b3/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/PKG-INFO` & `stripe-5.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b2
+Version: 5.5.0b3
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b2/README.md` & `stripe-5.5.0b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Stripe Python Library
 
 [![pypi](https://img.shields.io/pypi/v/stripe.svg)](https://pypi.python.org/pypi/stripe)
-[![Build Status](https://github.com/stripe/stripe-python/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/stripe/stripe-python/actions?query=branch%3Amaster)
+[![Build Status](https://github.com/stripe/stripe-python/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/stripe/stripe-python/actions?query=branch%3Amaster)
 [![Coverage Status](https://coveralls.io/repos/github/stripe/stripe-python/badge.svg?branch=master)](https://coveralls.io/github/stripe/stripe-python?branch=master)
 
 The Stripe Python library provides convenient access to the Stripe API from
 applications written in the Python language. It includes a pre-defined set of
 classes for API resources that initialize themselves dynamically from API
 responses which makes it compatible with a wide range of versions of the Stripe
 API.
@@ -189,14 +189,27 @@
 We would love for you to try these and share feedback with us before these features reach the stable phase.
 To install a beta version use `pip install` with the exact version you'd like to use:
 
 ```
 pip install stripe==5.3.0b3
 ```
 
+### Custom requests
+
+If you would like to send a request to an undocumented API (for example you are in a private beta), or if you prefer to bypass the method definitions in the library and specify your request details directly, you can use the `raw_request` method on `stripe`.
+
+```python
+response = stripe.raw_request(
+    "post", "/v1/beta_endpoint", param=123, stripe_version="2022-11-15; feature_beta=v3"
+)
+
+# (Optional) response is a StripeResponse. You can use `stripe.deserialize` to get a StripeObject.
+deserialized_resp = stripe.deserialize(response)
+```
+
 > **Note**
 > There can be breaking changes between beta versions. Therefore we recommend pinning the package version to a specific beta version in your [requirements file](https://pip.pypa.io/en/stable/user_guide/#requirements-files) or `setup.py`. This way you can install the same version each time without breaking changes unless you are intentionally looking for the latest beta version.
 
 We highly recommend keeping an eye on when the beta feature you are interested in goes from beta to stable so that you can move from using a beta version of the SDK to the stable version.
 
 If your beta feature requires a `Stripe-Version` header to be sent, use the `stripe.api_version` field to set it:
```

### Comparing `stripe-5.5.0b2/examples/oauth.py` & `stripe-5.5.0b3/examples/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/examples/proxy.py` & `stripe-5.5.0b3/examples/proxy.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/examples/webhooks.py` & `stripe-5.5.0b3/examples/webhooks.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/setup.py` & `stripe-5.5.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/__init__.py` & `stripe-5.5.0b3/stripe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 # OAuth
 from stripe.oauth import OAuth  # noqa
 
 # Webhooks
 from stripe.webhook import Webhook, WebhookSignature  # noqa
 
+from stripe.raw_request import _raw_request as raw_request  # noqa
+
+from stripe.raw_request import _deserialize as deserialize  # noqa
+
+from stripe.preview import preview  # noqa
+
 
 # Sets some basic information about the running application that's sent along
 # with API requests. Useful for plugin authors to identify their plugin when
 # communicating with Stripe.
 #
 # Takes a name and optional version and plugin URL.
 def set_app_info(name, partner_id=None, url=None, version=None):
```

### Comparing `stripe-5.5.0b2/stripe/api_requestor.py` & `stripe-5.5.0b3/stripe/api_requestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 def _encode_nested_dict(key, data, fmt="%s[%s]"):
     d = OrderedDict()
     for subkey, subvalue in six.iteritems(data):
         d[fmt % (key, subkey)] = subvalue
     return d
 
 
+def _json_encode_date_callback(value):
+    if isinstance(value, datetime.datetime):
+        return _encode_datetime(value)
+    return value
+
+
 def _api_encode(data):
     for key, value in six.iteritems(data):
         key = util.utf8(key)
         if value is None:
             continue
         elif hasattr(value, "stripe_id"):
             yield (key, value.stripe_id)
@@ -111,24 +117,36 @@
         str = info["name"]
         if info["version"]:
             str += "/%s" % (info["version"],)
         if info["url"]:
             str += " (%s)" % (info["url"],)
         return str
 
-    def request(self, method, url, params=None, headers=None):
+    def request(self, method, url, params=None, headers=None, api_mode=None):
         rbody, rcode, rheaders, my_api_key = self.request_raw(
-            method.lower(), url, params, headers, is_streaming=False
+            method.lower(),
+            url,
+            params,
+            headers,
+            is_streaming=False,
+            api_mode=api_mode,
         )
         resp = self.interpret_response(rbody, rcode, rheaders)
         return resp, my_api_key
 
-    def request_stream(self, method, url, params=None, headers=None):
+    def request_stream(
+        self, method, url, params=None, headers=None, api_mode=None
+    ):
         stream, rcode, rheaders, my_api_key = self.request_raw(
-            method.lower(), url, params, headers, is_streaming=True
+            method.lower(),
+            url,
+            params,
+            headers,
+            is_streaming=True,
+            api_mode=api_mode,
         )
         resp = self.interpret_streaming_response(stream, rcode, rheaders)
         return resp, my_api_key
 
     def handle_error_response(self, rbody, rcode, resp, rheaders):
         try:
             error_data = resp["error"]
@@ -234,15 +252,15 @@
         elif error_code == "unsupported_grant_type":
             return oauth_error.UnsupportedGrantTypeError(*args)
         elif error_code == "unsupported_response_type":
             return oauth_error.UnsupportedResponseTypeError(*args)
 
         return None
 
-    def request_headers(self, api_key, method):
+    def request_headers(self, api_key, method, api_mode):
         user_agent = "Stripe/v1 PythonBindings/%s" % (version.VERSION,)
         if stripe.app_info:
             user_agent += " " + self.format_app_info(stripe.app_info)
 
         ua = {
             "bindings_version": version.VERSION,
             "lang": "python",
@@ -268,29 +286,33 @@
             "Authorization": "Bearer %s" % (api_key,),
         }
 
         if self.stripe_account:
             headers["Stripe-Account"] = self.stripe_account
 
         if method == "post":
-            headers["Content-Type"] = "application/x-www-form-urlencoded"
             headers.setdefault("Idempotency-Key", str(uuid.uuid4()))
+            if api_mode == "preview":
+                headers["Content-Type"] = "application/json"
+            else:
+                headers["Content-Type"] = "application/x-www-form-urlencoded"
 
         if self.api_version is not None:
             headers["Stripe-Version"] = self.api_version
 
         return headers
 
     def request_raw(
         self,
         method,
         url,
         params=None,
         supplied_headers=None,
         is_streaming=False,
+        api_mode=None,
     ):
         """
         Mechanism for issuing an API call
         """
 
         if self.api_key:
             my_api_key = self.api_key
@@ -313,14 +335,21 @@
         encoded_params = urlencode(list(_api_encode(params or {})))
 
         # Don't use strict form encoding by changing the square bracket control
         # characters back to their literals. This is fine by the server, and
         # makes these parameter strings easier to read.
         encoded_params = encoded_params.replace("%5B", "[").replace("%5D", "]")
 
+        if api_mode == "preview":
+            encoded_body = json.dumps(
+                params or {}, default=_json_encode_date_callback
+            )
+        else:
+            encoded_body = encoded_params
+
         if method == "get" or method == "delete":
             if params:
                 abs_url = _build_api_url(abs_url, encoded_params)
             post_data = None
         elif method == "post":
             if (
                 supplied_headers is not None
@@ -330,23 +359,23 @@
                 generator = MultipartDataGenerator()
                 generator.add_params(params or {})
                 post_data = generator.get_post_data()
                 supplied_headers[
                     "Content-Type"
                 ] = "multipart/form-data; boundary=%s" % (generator.boundary,)
             else:
-                post_data = encoded_params
+                post_data = encoded_body
         else:
             raise error.APIConnectionError(
                 "Unrecognized HTTP method %r.  This may indicate a bug in the "
                 "Stripe bindings.  Please contact support@stripe.com for "
                 "assistance." % (method,)
             )
 
-        headers = self.request_headers(my_api_key, method)
+        headers = self.request_headers(my_api_key, method, api_mode)
         if supplied_headers is not None:
             for key, value in six.iteritems(supplied_headers):
                 headers[key] = value
 
         util.log_info("Request to Stripe api", method=method, path=abs_url)
         util.log_debug(
             "Post details",
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/__init__.py` & `stripe-5.5.0b3/stripe/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/__init__.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/createable_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/custom_method.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/deletable_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/listable_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/nested_resource_class_methods.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/searchable_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/singleton_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/test_helpers.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/test_helpers.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/abstract/updateable_api_resource.py` & `stripe-5.5.0b3/stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/account.py` & `stripe-5.5.0b3/stripe/api_resources/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     operations=["create", "retrieve", "update", "delete", "list"],
 )
 @nested_resource_class_methods(
     "capability",
     operations=["retrieve", "update", "list"],
     resource_plural="capabilities",
 )
-@nested_resource_class_methods("login_link", operations=["create"])
+@nested_resource_class_methods(
+    "login_link",
+    operations=["create"],
+)
 @nested_resource_class_methods(
     "person",
     operations=["create", "retrieve", "update", "delete", "list"],
 )
 class Account(
     CreateableAPIResource,
     DeletableAPIResource,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/account_link.py` & `stripe-5.5.0b3/stripe/api_resources/account_link.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 
 
 class AccountLink(CreateableAPIResource):
     """
     Account Links are the means by which a Connect platform grants a connected account permission to access
     Stripe-hosted applications, such as Connect Onboarding.
 
-    Related guide: [Connect Onboarding](https://stripe.com/docs/connect/connect-onboarding).
+    Related guide: [Connect Onboarding](https://stripe.com/docs/connect/connect-onboarding)
     """
 
     OBJECT_NAME = "account_link"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/account_session.py` & `stripe-5.5.0b3/stripe/api_resources/account_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     """
     An AccountSession allows a Connect platform to grant access to a connected account in Connect embedded components.
 
     We recommend that you create an AccountSession each time you need to display an embedded component
     to your user. Do not save AccountSessions to your database as they expire relatively
     quickly, and cannot be used more than once.
 
-    Related guide: [Connect embedded components](https://stripe.com/docs/connect/get-started-connect-embedded-components).
+    Related guide: [Connect embedded components](https://stripe.com/docs/connect/get-started-connect-embedded-components)
     """
 
     OBJECT_NAME = "account_session"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/apple_pay_domain.py` & `stripe-5.5.0b3/stripe/api_resources/apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/application_fee.py` & `stripe-5.5.0b3/stripe/api_resources/application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/application_fee_refund.py` & `stripe-5.5.0b3/stripe/api_resources/application_fee_refund.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class ApplicationFeeRefund(UpdateableAPIResource):
     """
     `Application Fee Refund` objects allow you to refund an application fee that
     has previously been created but not yet refunded. Funds will be refunded to
     the Stripe account from which the fee was originally collected.
 
-    Related guide: [Refunding Application Fees](https://stripe.com/docs/connect/destination-charges#refunding-app-fee).
+    Related guide: [Refunding application fees](https://stripe.com/docs/connect/destination-charges#refunding-app-fee)
     """
 
     OBJECT_NAME = "fee_refund"
 
     @classmethod
     def _build_instance_url(cls, fee, sid):
         fee = util.utf8(fee)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/apps/secret.py` & `stripe-5.5.0b3/stripe/api_resources/apps/secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     The primary resource in Secret Store is a `secret`. Other apps can't view secrets created by an app. Additionally, secrets are scoped to provide further permission control.
 
     All Dashboard users and the app backend share `account` scoped secrets. Use the `account` scope for secrets that don't change per-user, like a third-party API key.
 
     A `user` scoped secret is accessible by the app backend and one specific Dashboard user. Use the `user` scope for per-user secrets like per-user OAuth tokens, where different users might have different permissions.
 
-    Related guide: [Store data between page reloads](https://stripe.com/docs/stripe-apps/store-auth-data-custom-objects).
+    Related guide: [Store data between page reloads](https://stripe.com/docs/stripe-apps/store-auth-data-custom-objects)
     """
 
     OBJECT_NAME = "apps.secret"
 
     @classmethod
     def delete_where(
         cls, api_key=None, stripe_version=None, stripe_account=None, **params
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/balance.py` & `stripe-5.5.0b3/stripe/api_resources/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     You can also retrieve the balance history, which contains a list of
     [transactions](https://stripe.com/docs/reporting/balance-transaction-types) that contributed to the balance
     (charges, payouts, and so forth).
 
     The available and pending amounts for each currency are broken down further by
     payment source types.
 
-    Related guide: [Understanding Connect Account Balances](https://stripe.com/docs/connect/account-balances).
+    Related guide: [Understanding Connect account balances](https://stripe.com/docs/connect/account-balances)
     """
 
     OBJECT_NAME = "balance"
 
     @classmethod
     def class_url(cls):
         return "/v1/balance"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/balance_transaction.py` & `stripe-5.5.0b3/stripe/api_resources/balance_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 
 
 class BalanceTransaction(ListableAPIResource):
     """
     Balance transactions represent funds moving through your Stripe account.
     They're created for every type of transaction that comes into or flows out of your Stripe account balance.
 
-    Related guide: [Balance Transaction Types](https://stripe.com/docs/reports/balance-transaction-types).
+    Related guide: [Balance transaction types](https://stripe.com/docs/reports/balance-transaction-types)
     """
 
     OBJECT_NAME = "balance_transaction"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/bank_account.py` & `stripe-5.5.0b3/stripe/api_resources/bank_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     These bank accounts are payment methods on `Customer` objects.
 
     On the other hand [External Accounts](https://stripe.com/docs/api#external_accounts) are transfer
     destinations on `Account` objects for [Custom accounts](https://stripe.com/docs/connect/custom-accounts).
     They can be bank accounts or debit cards as well, and are documented in the links above.
 
-    Related guide: [Bank Debits and Transfers](https://stripe.com/docs/payments/bank-debits-transfers).
+    Related guide: [Bank debits and transfers](https://stripe.com/docs/payments/bank-debits-transfers)
     """
 
     OBJECT_NAME = "bank_account"
 
     def instance_url(self):
         token = util.utf8(self.id)
         extn = quote_plus(token)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/billing_portal/configuration.py` & `stripe-5.5.0b3/stripe/api_resources/billing_portal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/billing_portal/session.py` & `stripe-5.5.0b3/stripe/api_resources/billing_portal/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/capability.py` & `stripe-5.5.0b3/stripe/api_resources/capability.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from stripe.six.moves.urllib.parse import quote_plus
 
 
 class Capability(UpdateableAPIResource):
     """
     This is an object representing a capability for a Stripe account.
 
-    Related guide: [Account capabilities](https://stripe.com/docs/connect/account-capabilities).
+    Related guide: [Account capabilities](https://stripe.com/docs/connect/account-capabilities)
     """
 
     OBJECT_NAME = "capability"
 
     def instance_url(self):
         token = util.utf8(self.id)
         account = util.utf8(self.account)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/capital/financing_offer.py` & `stripe-5.5.0b3/stripe/api_resources/capital/financing_offer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/capital/financing_summary.py` & `stripe-5.5.0b3/stripe/api_resources/capital/financing_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/card.py` & `stripe-5.5.0b3/stripe/api_resources/card.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class Card(DeletableAPIResource, UpdateableAPIResource):
     """
     You can store multiple cards on a customer in order to charge the customer
     later. You can also store multiple debit cards on a recipient in order to
     transfer to those cards later.
 
-    Related guide: [Card Payments with Sources](https://stripe.com/docs/sources/cards).
+    Related guide: [Card payments with Sources](https://stripe.com/docs/sources/cards)
     """
 
     OBJECT_NAME = "card"
 
     def instance_url(self):
         token = util.utf8(self.id)
         extn = quote_plus(token)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/cash_balance.py` & `stripe-5.5.0b3/stripe/api_resources/cash_balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/charge.py` & `stripe-5.5.0b3/stripe/api_resources/charge.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     UpdateableAPIResource,
 ):
     """
     To charge a credit or a debit card, you create a `Charge` object. You can
     retrieve and refund individual charges as well as list all charges. Charges
     are identified by a unique, random ID.
 
-    Related guide: [Accept a payment with the Charges API](https://stripe.com/docs/payments/accept-a-payment-charges).
+    Related guide: [Accept a payment with the Charges API](https://stripe.com/docs/payments/accept-a-payment-charges)
     """
 
     OBJECT_NAME = "charge"
 
     @classmethod
     def _cls_capture(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/checkout/session.py` & `stripe-5.5.0b3/stripe/api_resources/checkout/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     to the [Customer](https://stripe.com/docs/api/customers), and either the successful
     [PaymentIntent](https://stripe.com/docs/api/payment_intents) or an active
     [Subscription](https://stripe.com/docs/api/subscriptions).
 
     You can create a Checkout Session on your server and redirect to its URL
     to begin Checkout.
 
-    Related guide: [Checkout Quickstart](https://stripe.com/docs/checkout/quickstart).
+    Related guide: [Checkout quickstart](https://stripe.com/docs/checkout/quickstart)
     """
 
     OBJECT_NAME = "checkout.session"
 
     @classmethod
     def _cls_expire(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/country_spec.py` & `stripe-5.5.0b3/stripe/api_resources/country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/coupon.py` & `stripe-5.5.0b3/stripe/api_resources/coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/credit_note.py` & `stripe-5.5.0b3/stripe/api_resources/credit_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     Issue a credit note to adjust an invoice's amount after the invoice is finalized.
 
-    Related guide: [Credit Notes](https://stripe.com/docs/billing/invoices/credit-notes).
+    Related guide: [Credit notes](https://stripe.com/docs/billing/invoices/credit-notes)
     """
 
     OBJECT_NAME = "credit_note"
 
     @classmethod
     def preview(
         cls, api_key=None, stripe_version=None, stripe_account=None, **params
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/customer.py` & `stripe-5.5.0b3/stripe/api_resources/customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ListableAPIResource,
     SearchableAPIResource,
     UpdateableAPIResource,
 ):
     """
     This object represents a customer of your business. It lets you create recurring charges and track payments that belong to the same customer.
 
-    Related guide: [Save a card during payment](https://stripe.com/docs/payments/save-during-payment).
+    Related guide: [Save a card during payment](https://stripe.com/docs/payments/save-during-payment)
     """
 
     OBJECT_NAME = "customer"
 
     @classmethod
     def _cls_create_funding_instructions(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/customer_balance_transaction.py` & `stripe-5.5.0b3/stripe/api_resources/customer_balance_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from stripe.api_resources.abstract import APIResource
 from stripe.api_resources.customer import Customer
 from stripe.six.moves.urllib.parse import quote_plus
 
 
 class CustomerBalanceTransaction(APIResource):
     """
-    Each customer has a [`balance`](https://stripe.com/docs/api/customers/object#customer_object-balance) value,
+    Each customer has a [Balance](https://stripe.com/docs/api/customers/object#customer_object-balance) value,
     which denotes a debit or credit that's automatically applied to their next invoice upon finalization.
     You may modify the value directly by using the [update customer API](https://stripe.com/docs/api/customers/update),
     or by creating a Customer Balance Transaction, which increments or decrements the customer's `balance` by the specified `amount`.
 
-    Related guide: [Customer Balance](https://stripe.com/docs/billing/customer/balance) to learn more.
+    Related guide: [Customer balance](https://stripe.com/docs/billing/customer/balance)
     """
 
     OBJECT_NAME = "customer_balance_transaction"
 
     def instance_url(self):
         token = util.utf8(self.id)
         customer = util.utf8(self.customer)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/customer_cash_balance_transaction.py` & `stripe-5.5.0b3/stripe/api_resources/customer_cash_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/dispute.py` & `stripe-5.5.0b3/stripe/api_resources/dispute.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     A dispute occurs when a customer questions your charge with their card issuer.
     When this happens, you're given the opportunity to respond to the dispute with
     evidence that shows that the charge is legitimate. You can find more
     information about the dispute process in our [Disputes and
     Fraud](https://stripe.com/docs/disputes) documentation.
 
-    Related guide: [Disputes and Fraud](https://stripe.com/docs/disputes).
+    Related guide: [Disputes and fraud](https://stripe.com/docs/disputes)
     """
 
     OBJECT_NAME = "dispute"
 
     @classmethod
     def _cls_close(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/ephemeral_key.py` & `stripe-5.5.0b3/stripe/api_resources/ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/error_object.py` & `stripe-5.5.0b3/stripe/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/event.py` & `stripe-5.5.0b3/stripe/api_resources/event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/exchange_rate.py` & `stripe-5.5.0b3/stripe/api_resources/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/file.py` & `stripe-5.5.0b3/stripe/api_resources/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     This is an object representing a file hosted on Stripe's servers. The
     file may have been uploaded by yourself using the [create file](https://stripe.com/docs/api#create_file)
     request (for example, when uploading dispute evidence) or it may have
     been created by Stripe (for example, the results of a [Sigma scheduled
     query](https://stripe.com/docs/api#scheduled_queries)).
 
-    Related guide: [File Upload Guide](https://stripe.com/docs/file-upload).
+    Related guide: [File upload guide](https://stripe.com/docs/file-upload)
     """
 
     OBJECT_NAME = "file"
 
     # This resource can have two different object names. In latter API
     # versions, only `file` is used, but since stripe-python may be used with
     # any API version, we need to support deserializing the older
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/file_link.py` & `stripe-5.5.0b3/stripe/api_resources/file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/financial_connections/__init__.py` & `stripe-5.5.0b3/stripe/api_resources/financial_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/financial_connections/account.py` & `stripe-5.5.0b3/stripe/api_resources/gift_cards/transaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,87 @@
 # -*- coding: utf-8 -*-
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
+from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import nested_resource_class_methods
+from stripe.api_resources.abstract import UpdateableAPIResource
 
 
-@nested_resource_class_methods("inferred_balance", operations=["list"])
-class Account(ListableAPIResource):
+class Transaction(
+    CreateableAPIResource,
+    ListableAPIResource,
+    UpdateableAPIResource,
+):
     """
-    A Financial Connections Account represents an account that exists outside of Stripe, to which you have been granted some degree of access.
+    A gift card transaction represents a single transaction on a referenced gift card.
+    A transaction is in one of three states, `confirmed`, `held` or `canceled`. A `confirmed`
+    transaction is one that has added/deducted funds. A `held` transaction has created a
+    temporary hold on funds, which can then be cancelled or confirmed. A `held` transaction
+    can be confirmed into a `confirmed` transaction, or canceled into a `canceled` transaction.
+    A `canceled` transaction has no effect on a gift card's balance.
     """
 
-    OBJECT_NAME = "financial_connections.account"
+    OBJECT_NAME = "gift_cards.transaction"
 
     @classmethod
-    def _cls_disconnect(
+    def _cls_cancel(
         cls,
-        account,
+        id,
         api_key=None,
         stripe_version=None,
         stripe_account=None,
         **params
     ):
         return cls._static_request(
             "post",
-            "/v1/financial_connections/accounts/{account}/disconnect".format(
-                account=util.sanitize_id(account)
+            "/v1/gift_cards/transactions/{id}/cancel".format(
+                id=util.sanitize_id(id)
             ),
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @util.class_method_variant("_cls_disconnect")
-    def disconnect(self, idempotency_key=None, **params):
+    @util.class_method_variant("_cls_cancel")
+    def cancel(self, idempotency_key=None, **params):
         return self._request(
             "post",
-            "/v1/financial_connections/accounts/{account}/disconnect".format(
-                account=util.sanitize_id(self.get("id"))
+            "/v1/gift_cards/transactions/{id}/cancel".format(
+                id=util.sanitize_id(self.get("id"))
             ),
             idempotency_key=idempotency_key,
             params=params,
         )
 
     @classmethod
-    def _cls_list_owners(
+    def _cls_confirm(
         cls,
-        account,
-        api_key=None,
-        stripe_version=None,
-        stripe_account=None,
-        **params
-    ):
-        return cls._static_request(
-            "get",
-            "/v1/financial_connections/accounts/{account}/owners".format(
-                account=util.sanitize_id(account)
-            ),
-            api_key=api_key,
-            stripe_version=stripe_version,
-            stripe_account=stripe_account,
-            params=params,
-        )
-
-    @util.class_method_variant("_cls_list_owners")
-    def list_owners(self, idempotency_key=None, **params):
-        return self._request(
-            "get",
-            "/v1/financial_connections/accounts/{account}/owners".format(
-                account=util.sanitize_id(self.get("id"))
-            ),
-            idempotency_key=idempotency_key,
-            params=params,
-        )
-
-    @classmethod
-    def _cls_refresh_account(
-        cls,
-        account,
+        id,
         api_key=None,
         stripe_version=None,
         stripe_account=None,
         **params
     ):
         return cls._static_request(
             "post",
-            "/v1/financial_connections/accounts/{account}/refresh".format(
-                account=util.sanitize_id(account)
+            "/v1/gift_cards/transactions/{id}/confirm".format(
+                id=util.sanitize_id(id)
             ),
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @util.class_method_variant("_cls_refresh_account")
-    def refresh_account(self, idempotency_key=None, **params):
+    @util.class_method_variant("_cls_confirm")
+    def confirm(self, idempotency_key=None, **params):
         return self._request(
             "post",
-            "/v1/financial_connections/accounts/{account}/refresh".format(
-                account=util.sanitize_id(self.get("id"))
+            "/v1/gift_cards/transactions/{id}/confirm".format(
+                id=util.sanitize_id(self.get("id"))
             ),
             idempotency_key=idempotency_key,
             params=params,
         )
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/funding_instructions.py` & `stripe-5.5.0b3/stripe/api_resources/funding_instructions.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 
 class FundingInstructions(StripeObject):
     """
     Each customer has a [`balance`](https://stripe.com/docs/api/customers/object#customer_object-balance) that is
     automatically applied to future invoices and payments using the `customer_balance` payment method.
     Customers can fund this balance by initiating a bank transfer to any account in the
     `financial_addresses` field.
-    Related guide: [Customer Balance - Funding Instructions](https://stripe.com/docs/payments/customer-balance/funding-instructions) to learn more
+    Related guide: [Customer balance funding instructions](https://stripe.com/docs/payments/customer-balance/funding-instructions)
     """
 
     OBJECT_NAME = "funding_instructions"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/gift_cards/card.py` & `stripe-5.5.0b3/stripe/api_resources/gift_cards/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/gift_cards/transaction.py` & `stripe-5.5.0b3/stripe/api_resources/tax/transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,73 @@
 # -*- coding: utf-8 -*-
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
-from stripe.api_resources.abstract import CreateableAPIResource
-from stripe.api_resources.abstract import ListableAPIResource
-from stripe.api_resources.abstract import UpdateableAPIResource
+from stripe.api_resources.abstract import APIResource
 
 
-class Transaction(
-    CreateableAPIResource,
-    ListableAPIResource,
-    UpdateableAPIResource,
-):
+class Transaction(APIResource):
     """
-    A gift card transaction represents a single transaction on a referenced gift card.
-    A transaction is in one of three states, `confirmed`, `held` or `canceled`. A `confirmed`
-    transaction is one that has added/deducted funds. A `held` transaction has created a
-    temporary hold on funds, which can then be cancelled or confirmed. A `held` transaction
-    can be confirmed into a `confirmed` transaction, or canceled into a `canceled` transaction.
-    A `canceled` transaction has no effect on a gift card's balance.
+    A Tax Transaction records the tax collected from or refunded to your customer.
+
+    Related guide: [Calculate tax in your custom payment flow](https://stripe.com/docs/tax/custom#tax-transaction)
     """
 
-    OBJECT_NAME = "gift_cards.transaction"
+    OBJECT_NAME = "tax.transaction"
 
     @classmethod
-    def _cls_cancel(
-        cls,
-        id,
-        api_key=None,
-        stripe_version=None,
-        stripe_account=None,
-        **params
+    def create_from_calculation(
+        cls, api_key=None, stripe_version=None, stripe_account=None, **params
     ):
         return cls._static_request(
             "post",
-            "/v1/gift_cards/transactions/{id}/cancel".format(
-                id=util.sanitize_id(id)
-            ),
+            "/v1/tax/transactions/create_from_calculation",
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @util.class_method_variant("_cls_cancel")
-    def cancel(self, idempotency_key=None, **params):
-        return self._request(
+    @classmethod
+    def create_reversal(
+        cls, api_key=None, stripe_version=None, stripe_account=None, **params
+    ):
+        return cls._static_request(
             "post",
-            "/v1/gift_cards/transactions/{id}/cancel".format(
-                id=util.sanitize_id(self.get("id"))
-            ),
-            idempotency_key=idempotency_key,
+            "/v1/tax/transactions/create_reversal",
+            api_key=api_key,
+            stripe_version=stripe_version,
+            stripe_account=stripe_account,
             params=params,
         )
 
     @classmethod
-    def _cls_confirm(
+    def _cls_list_line_items(
         cls,
-        id,
+        transaction,
         api_key=None,
         stripe_version=None,
         stripe_account=None,
         **params
     ):
         return cls._static_request(
-            "post",
-            "/v1/gift_cards/transactions/{id}/confirm".format(
-                id=util.sanitize_id(id)
+            "get",
+            "/v1/tax/transactions/{transaction}/line_items".format(
+                transaction=util.sanitize_id(transaction)
             ),
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @util.class_method_variant("_cls_confirm")
-    def confirm(self, idempotency_key=None, **params):
+    @util.class_method_variant("_cls_list_line_items")
+    def list_line_items(self, idempotency_key=None, **params):
         return self._request(
-            "post",
-            "/v1/gift_cards/transactions/{id}/confirm".format(
-                id=util.sanitize_id(self.get("id"))
+            "get",
+            "/v1/tax/transactions/{transaction}/line_items".format(
+                transaction=util.sanitize_id(self.get("id"))
             ),
             idempotency_key=idempotency_key,
             params=params,
         )
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/identity/verification_report.py` & `stripe-5.5.0b3/stripe/api_resources/identity/verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/identity/verification_session.py` & `stripe-5.5.0b3/stripe/api_resources/identity/verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/invoice.py` & `stripe-5.5.0b3/stripe/api_resources/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     per currency](https://stripe.com/docs/currencies#minimum-and-maximum-charge-amounts), the
     invoice is automatically marked paid, and we add the amount due to the
     customer's credit balance which is applied to the next invoice.
 
     More details on the customer's credit balance are
     [here](https://stripe.com/docs/billing/customer/balance).
 
-    Related guide: [Send Invoices to Customers](https://stripe.com/docs/billing/invoices/sending).
+    Related guide: [Send invoices to customers](https://stripe.com/docs/billing/invoices/sending)
     """
 
     OBJECT_NAME = "invoice"
 
     @classmethod
     def _cls_finalize_invoice(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/invoice_item.py` & `stripe-5.5.0b3/stripe/api_resources/invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/__init__.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/authorization.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Authorization(ListableAPIResource, UpdateableAPIResource):
     """
     When an [issued card](https://stripe.com/docs/issuing) is used to make a purchase, an Issuing `Authorization`
     object is created. [Authorizations](https://stripe.com/docs/issuing/purchases/authorizations) must be approved for the
     purchase to be completed successfully.
 
-    Related guide: [Issued Card Authorizations](https://stripe.com/docs/issuing/purchases/authorizations).
+    Related guide: [Issued card authorizations](https://stripe.com/docs/issuing/purchases/authorizations)
     """
 
     OBJECT_NAME = "issuing.authorization"
 
     @classmethod
     def _cls_approve(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/card.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/card_design.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/card_design.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/cardholder.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/cardholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     An Issuing `Cardholder` object represents an individual or business entity who is [issued](https://stripe.com/docs/issuing) cards.
 
-    Related guide: [How to create a Cardholder](https://stripe.com/docs/issuing/cards#create-cardholder)
+    Related guide: [How to create a cardholder](https://stripe.com/docs/issuing/cards#create-cardholder)
     """
 
     OBJECT_NAME = "issuing.cardholder"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/dispute.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/dispute.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     As a [card issuer](https://stripe.com/docs/issuing), you can dispute transactions that the cardholder does not recognize, suspects to be fraudulent, or has other issues with.
 
-    Related guide: [Disputing Transactions](https://stripe.com/docs/issuing/purchases/disputes)
+    Related guide: [Issuing disputes](https://stripe.com/docs/issuing/purchases/disputes)
     """
 
     OBJECT_NAME = "issuing.dispute"
 
     @classmethod
     def _cls_submit(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/issuing/transaction.py` & `stripe-5.5.0b3/stripe/api_resources/issuing/transaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 class Transaction(ListableAPIResource, UpdateableAPIResource):
     """
     Any use of an [issued card](https://stripe.com/docs/issuing) that results in funds entering or leaving
     your Stripe account, such as a completed purchase or refund, is represented by an Issuing
     `Transaction` object.
 
-    Related guide: [Issued Card Transactions](https://stripe.com/docs/issuing/purchases/transactions).
+    Related guide: [Issued card transactions](https://stripe.com/docs/issuing/purchases/transactions)
     """
 
     OBJECT_NAME = "issuing.transaction"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/list_object.py` & `stripe-5.5.0b3/stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/order.py` & `stripe-5.5.0b3/stripe/api_resources/order.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/payment_intent.py` & `stripe-5.5.0b3/stripe/api_resources/payment_intent.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     see the history of payment attempts for a particular session.
 
     A PaymentIntent transitions through
     [multiple statuses](https://stripe.com/docs/payments/intents#intent-statuses)
     throughout its lifetime as it interfaces with Stripe.js to perform
     authentication flows and ultimately creates at most one successful charge.
 
-    Related guide: [Payment Intents API](https://stripe.com/docs/payments/payment-intents).
+    Related guide: [Payment Intents API](https://stripe.com/docs/payments/payment-intents)
     """
 
     OBJECT_NAME = "payment_intent"
 
     @classmethod
     def _cls_apply_customer_balance(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/payment_link.py` & `stripe-5.5.0b3/stripe/api_resources/payment_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/payment_method.py` & `stripe-5.5.0b3/stripe/api_resources/payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/payout.py` & `stripe-5.5.0b3/stripe/api_resources/payout.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     A `Payout` object is created when you receive funds from Stripe, or when you
     initiate a payout to either a bank account or debit card of a [connected
     Stripe account](https://stripe.com/docs/connect/bank-debit-card-payouts). You can retrieve individual payouts,
     as well as list all payouts. Payouts are made on [varying
     schedules](https://stripe.com/docs/connect/manage-payout-schedule), depending on your country and
     industry.
 
-    Related guide: [Receiving Payouts](https://stripe.com/docs/payouts).
+    Related guide: [Receiving payouts](https://stripe.com/docs/payouts)
     """
 
     OBJECT_NAME = "payout"
 
     @classmethod
     def _cls_cancel(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/person.py` & `stripe-5.5.0b3/stripe/api_resources/person.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Person(UpdateableAPIResource):
     """
     This is an object representing a person associated with a Stripe account.
 
     A platform cannot access a Standard or Express account's persons after the account starts onboarding, such as after generating an account link for the account.
     See the [Standard onboarding](https://stripe.com/docs/connect/standard-accounts) or [Express onboarding documentation](https://stripe.com/docs/connect/express-accounts) for information about platform pre-filling and account onboarding steps.
 
-    Related guide: [Handling Identity Verification with the API](https://stripe.com/docs/connect/identity-verification-api#person-information).
+    Related guide: [Handling identity verification with the API](https://stripe.com/docs/connect/identity-verification-api#person-information)
     """
 
     OBJECT_NAME = "person"
 
     def instance_url(self):
         token = util.utf8(self.id)
         account = util.utf8(self.account)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/plan.py` & `stripe-5.5.0b3/stripe/api_resources/plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/price.py` & `stripe-5.5.0b3/stripe/api_resources/price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/product.py` & `stripe-5.5.0b3/stripe/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/promotion_code.py` & `stripe-5.5.0b3/stripe/api_resources/promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/quote.py` & `stripe-5.5.0b3/stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/quote_phase.py` & `stripe-5.5.0b3/stripe/api_resources/quote_phase.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/radar/early_fraud_warning.py` & `stripe-5.5.0b3/stripe/api_resources/radar/early_fraud_warning.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 
 
 class EarlyFraudWarning(ListableAPIResource):
     """
     An early fraud warning indicates that the card issuer has notified us that a
     charge may be fraudulent.
 
-    Related guide: [Early Fraud Warnings](https://stripe.com/docs/disputes/measuring#early-fraud-warnings).
+    Related guide: [Early fraud warnings](https://stripe.com/docs/disputes/measuring#early-fraud-warnings)
     """
 
     OBJECT_NAME = "radar.early_fraud_warning"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/radar/value_list.py` & `stripe-5.5.0b3/stripe/api_resources/radar/value_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     DeletableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     Value lists allow you to group values together which can then be referenced in rules.
 
-    Related guide: [Default Stripe Lists](https://stripe.com/docs/radar/lists#managing-list-items).
+    Related guide: [Default Stripe lists](https://stripe.com/docs/radar/lists#managing-list-items)
     """
 
     OBJECT_NAME = "radar.value_list"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/radar/value_list_item.py` & `stripe-5.5.0b3/stripe/api_resources/radar/value_list_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     CreateableAPIResource,
     DeletableAPIResource,
     ListableAPIResource,
 ):
     """
     Value list items allow you to add specific values to a given Radar value list, which can then be used in rules.
 
-    Related guide: [Managing List Items](https://stripe.com/docs/radar/lists#managing-list-items).
+    Related guide: [Managing list items](https://stripe.com/docs/radar/lists#managing-list-items)
     """
 
     OBJECT_NAME = "radar.value_list_item"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/refund.py` & `stripe-5.5.0b3/stripe/api_resources/refund.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     CreateableAPIResource, ListableAPIResource, UpdateableAPIResource
 ):
     """
     `Refund` objects allow you to refund a charge that has previously been created
     but not yet refunded. Funds will be refunded to the credit or debit card that
     was originally charged.
 
-    Related guide: [Refunds](https://stripe.com/docs/refunds).
+    Related guide: [Refunds](https://stripe.com/docs/refunds)
     """
 
     OBJECT_NAME = "refund"
 
     @classmethod
     def _cls_cancel(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/reporting/report_run.py` & `stripe-5.5.0b3/stripe/api_resources/reporting/report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/reporting/report_type.py` & `stripe-5.5.0b3/stripe/api_resources/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/reversal.py` & `stripe-5.5.0b3/stripe/api_resources/reversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Reversing a transfer that was made for a [destination
     charge](https://stripe.com/docs/connect/destination-charges) is allowed only up to the amount of
     the charge. It is possible to reverse a
     [transfer_group](https://stripe.com/docs/connect/charges-transfers#transfer-options)
     transfer only if the destination account has enough balance to cover the
     reversal.
 
-    Related guide: [Reversing Transfers](https://stripe.com/docs/connect/charges-transfers#reversing-transfers).
+    Related guide: [Reversing transfers](https://stripe.com/docs/connect/charges-transfers#reversing-transfers)
     """
 
     OBJECT_NAME = "transfer_reversal"
 
     def instance_url(self):
         token = util.utf8(self.id)
         transfer = util.utf8(self.transfer)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/review.py` & `stripe-5.5.0b3/stripe/api_resources/review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/search_result_object.py` & `stripe-5.5.0b3/stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/setup_attempt.py` & `stripe-5.5.0b3/stripe/api_resources/setup_attempt.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/setup_intent.py` & `stripe-5.5.0b3/stripe/api_resources/setup_intent.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     it will automatically attach the resulting payment method to that Customer.
     We recommend using SetupIntents or [setup_future_usage](https://stripe.com/docs/api#payment_intent_object-setup_future_usage) on
     PaymentIntents to save payment methods in order to prevent saving invalid or unoptimized payment methods.
 
     By using SetupIntents, you ensure that your customers experience the minimum set of required friction,
     even as regulations change over time.
 
-    Related guide: [Setup Intents API](https://stripe.com/docs/payments/setup-intents).
+    Related guide: [Setup Intents API](https://stripe.com/docs/payments/setup-intents)
     """
 
     OBJECT_NAME = "setup_intent"
 
     @classmethod
     def _cls_cancel(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/shipping_rate.py` & `stripe-5.5.0b3/stripe/api_resources/shipping_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/sigma/scheduled_query_run.py` & `stripe-5.5.0b3/stripe/api_resources/sigma/scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/source.py` & `stripe-5.5.0b3/stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/source_transaction.py` & `stripe-5.5.0b3/stripe/api_resources/source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/subscription.py` & `stripe-5.5.0b3/stripe/api_resources/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ListableAPIResource,
     SearchableAPIResource,
     UpdateableAPIResource,
 ):
     """
     Subscriptions allow you to charge a customer on a recurring basis.
 
-    Related guide: [Creating Subscriptions](https://stripe.com/docs/billing/subscriptions/creating).
+    Related guide: [Creating subscriptions](https://stripe.com/docs/billing/subscriptions/creating)
     """
 
     OBJECT_NAME = "subscription"
 
     @classmethod
     def _cls_cancel(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/subscription_item.py` & `stripe-5.5.0b3/stripe/api_resources/subscription_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import DeletableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
 from stripe.api_resources.abstract import nested_resource_class_methods
 
 
-@nested_resource_class_methods("usage_record", operations=["create"])
+@nested_resource_class_methods(
+    "usage_record",
+    operations=["create"],
+)
 @nested_resource_class_methods(
     "usage_record_summary",
     operations=["list"],
     resource_plural="usage_record_summaries",
 )
 class SubscriptionItem(
     CreateableAPIResource,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/subscription_schedule.py` & `stripe-5.5.0b3/stripe/api_resources/subscription_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     A subscription schedule allows you to create and manage the lifecycle of a subscription by predefining expected changes.
 
-    Related guide: [Subscription Schedules](https://stripe.com/docs/billing/subscriptions/subscription-schedules).
+    Related guide: [Subscription schedules](https://stripe.com/docs/billing/subscriptions/subscription-schedules)
     """
 
     OBJECT_NAME = "subscription_schedule"
 
     @classmethod
     def _cls_amend(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax/calculation.py` & `stripe-5.5.0b3/stripe/api_resources/tax/calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from stripe.api_resources.abstract import CreateableAPIResource
 
 
 class Calculation(CreateableAPIResource):
     """
     A Tax Calculation allows you to calculate the tax to collect from your customer.
 
-    Related guide: [Calculate tax in your custom payment flow](https://stripe.com/docs/tax/custom).
+    Related guide: [Calculate tax in your custom payment flow](https://stripe.com/docs/tax/custom)
     """
 
     OBJECT_NAME = "tax.calculation"
 
     @classmethod
     def _cls_list_line_items(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax/registration.py` & `stripe-5.5.0b3/stripe/api_resources/tax/registration.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,13 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     A Tax `Registration` lets us know that your business is registered to collect tax on payments within a region, enabling you to [automatically collect tax](https://stripe.com/docs/tax).
 
-    Stripe will not register on your behalf with the relevant authorities when you create a Tax `Registration` object. For more information on how to register to collect tax, see [our guide](https://stripe.com/docs/tax/registering).
+    Stripe doesn't register on your behalf with the relevant authorities when you create a Tax `Registration` object. For more information on how to register to collect tax, see [our guide](https://stripe.com/docs/tax/registering).
+
+    Related guide: [Using the Registrations API](https://stripe.com/docs/tax/registrations-api)
     """
 
     OBJECT_NAME = "tax.registration"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax/settings.py` & `stripe-5.5.0b3/stripe/api_resources/tax/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from stripe.api_resources.abstract import UpdateableAPIResource
 
 
 class Settings(SingletonAPIResource, UpdateableAPIResource):
     """
     You can use Tax `Settings` to manage configurations used by Stripe Tax calculations.
 
-    Related guide: [Account settings](https://stripe.com/docs/tax/connect/settings).
+    Related guide: [Using the Settings API](https://stripe.com/docs/tax/settings-api)
     """
 
     OBJECT_NAME = "tax.settings"
 
     @classmethod
     def class_url(cls):
         return "/v1/tax/settings"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax/transaction.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/financial_account.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 # -*- coding: utf-8 -*-
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
-from stripe.api_resources.abstract import APIResource
+from stripe.api_resources.abstract import CreateableAPIResource
+from stripe.api_resources.abstract import ListableAPIResource
+from stripe.api_resources.abstract import UpdateableAPIResource
 
 
-class Transaction(APIResource):
+class FinancialAccount(
+    CreateableAPIResource,
+    ListableAPIResource,
+    UpdateableAPIResource,
+):
     """
-    A Tax Transaction records the tax collected from or refunded to your customer.
-
-    Related guide: [Calculate tax in your custom payment flow](https://stripe.com/docs/tax/custom#tax-transaction).
+    Stripe Treasury provides users with a container for money called a FinancialAccount that is separate from their Payments balance.
+    FinancialAccounts serve as the source and destination of Treasury's money movement APIs.
     """
 
-    OBJECT_NAME = "tax.transaction"
+    OBJECT_NAME = "treasury.financial_account"
 
     @classmethod
-    def create_from_calculation(
-        cls, api_key=None, stripe_version=None, stripe_account=None, **params
+    def _cls_retrieve_features(
+        cls,
+        financial_account,
+        api_key=None,
+        stripe_version=None,
+        stripe_account=None,
+        **params
     ):
         return cls._static_request(
-            "post",
-            "/v1/tax/transactions/create_from_calculation",
+            "get",
+            "/v1/treasury/financial_accounts/{financial_account}/features".format(
+                financial_account=util.sanitize_id(financial_account)
+            ),
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @classmethod
-    def create_reversal(
-        cls, api_key=None, stripe_version=None, stripe_account=None, **params
-    ):
-        return cls._static_request(
-            "post",
-            "/v1/tax/transactions/create_reversal",
-            api_key=api_key,
-            stripe_version=stripe_version,
-            stripe_account=stripe_account,
+    @util.class_method_variant("_cls_retrieve_features")
+    def retrieve_features(self, idempotency_key=None, **params):
+        return self._request(
+            "get",
+            "/v1/treasury/financial_accounts/{financial_account}/features".format(
+                financial_account=util.sanitize_id(self.get("id"))
+            ),
+            idempotency_key=idempotency_key,
             params=params,
         )
 
     @classmethod
-    def _cls_list_line_items(
+    def _cls_update_features(
         cls,
-        transaction,
+        financial_account,
         api_key=None,
         stripe_version=None,
         stripe_account=None,
         **params
     ):
         return cls._static_request(
-            "get",
-            "/v1/tax/transactions/{transaction}/line_items".format(
-                transaction=util.sanitize_id(transaction)
+            "post",
+            "/v1/treasury/financial_accounts/{financial_account}/features".format(
+                financial_account=util.sanitize_id(financial_account)
             ),
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
-    @util.class_method_variant("_cls_list_line_items")
-    def list_line_items(self, idempotency_key=None, **params):
+    @util.class_method_variant("_cls_update_features")
+    def update_features(self, idempotency_key=None, **params):
         return self._request(
-            "get",
-            "/v1/tax/transactions/{transaction}/line_items".format(
-                transaction=util.sanitize_id(self.get("id"))
+            "post",
+            "/v1/treasury/financial_accounts/{financial_account}/features".format(
+                financial_account=util.sanitize_id(self.get("id"))
             ),
             idempotency_key=idempotency_key,
             params=params,
         )
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax_id.py` & `stripe-5.5.0b3/stripe/api_resources/tax_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class TaxId(APIResource):
     """
     You can add one or multiple tax IDs to a [customer](https://stripe.com/docs/api/customers).
     A customer's tax IDs are displayed on invoices and credit notes issued for the customer.
 
-    Related guide: [Customer Tax Identification Numbers](https://stripe.com/docs/billing/taxes/tax-ids).
+    Related guide: [Customer tax identification numbers](https://stripe.com/docs/billing/taxes/tax-ids)
     """
 
     OBJECT_NAME = "tax_id"
 
     def instance_url(self):
         token = util.utf8(self.id)
         customer = util.utf8(self.customer)
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/tax_rate.py` & `stripe-5.5.0b3/stripe/api_resources/tax_rate.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     Tax rates can be applied to [invoices](https://stripe.com/docs/billing/invoices/tax-rates), [subscriptions](https://stripe.com/docs/billing/subscriptions/taxes) and [Checkout Sessions](https://stripe.com/docs/payments/checkout/set-up-a-subscription#tax-rates) to collect tax.
 
-    Related guide: [Tax Rates](https://stripe.com/docs/billing/taxes/tax-rates).
+    Related guide: [Tax rates](https://stripe.com/docs/billing/taxes/tax-rates)
     """
 
     OBJECT_NAME = "tax_rate"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/terminal/configuration.py` & `stripe-5.5.0b3/stripe/api_resources/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/terminal/location.py` & `stripe-5.5.0b3/stripe/api_resources/terminal/location.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     DeletableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     A Location represents a grouping of readers.
 
-    Related guide: [Fleet Management](https://stripe.com/docs/terminal/fleet/locations).
+    Related guide: [Fleet management](https://stripe.com/docs/terminal/fleet/locations)
     """
 
     OBJECT_NAME = "terminal.location"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/terminal/reader.py` & `stripe-5.5.0b3/stripe/api_resources/terminal/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     DeletableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     A Reader represents a physical device for accepting payment details.
 
-    Related guide: [Connecting to a Reader](https://stripe.com/docs/terminal/payments/connect-reader).
+    Related guide: [Connecting to a reader](https://stripe.com/docs/terminal/payments/connect-reader)
     """
 
     OBJECT_NAME = "terminal.reader"
 
     @classmethod
     def _cls_cancel_action(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/test_helpers/test_clock.py` & `stripe-5.5.0b3/stripe/api_resources/test_helpers/test_clock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/token.py` & `stripe-5.5.0b3/stripe/api_resources/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 
     Tokens cannot be stored or used more than once. To store card or bank account
     information for later use, you can create [Customer](https://stripe.com/docs/api#customers)
     objects or [Custom accounts](https://stripe.com/docs/api#external_accounts). Note that
     [Radar](https://stripe.com/docs/radar), our integrated solution for automatic fraud protection,
     performs best with integrations that use client-side tokenization.
 
-    Related guide: [Accept a payment](https://stripe.com/docs/payments/accept-a-payment-charges#web-create-token)
+    Related guide: [Accept a payment with Charges and Tokens](https://stripe.com/docs/payments/accept-a-payment-charges#web-create-token)
     """
 
     OBJECT_NAME = "token"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/topup.py` & `stripe-5.5.0b3/stripe/api_resources/topup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Topup(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     """
     To top up your Stripe balance, you create a top-up object. You can retrieve
     individual top-ups, as well as list all top-ups. Top-ups are identified by a
     unique, random ID.
 
-    Related guide: [Topping Up your Platform Account](https://stripe.com/docs/connect/top-ups).
+    Related guide: [Topping up your platform account](https://stripe.com/docs/connect/top-ups)
     """
 
     OBJECT_NAME = "topup"
 
     @classmethod
     def _cls_cancel(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/transfer.py` & `stripe-5.5.0b3/stripe/api_resources/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 
     Before April 6, 2017, transfers also represented movement of funds from a
     Stripe account to a card or bank account. This behavior has since been split
     out into a [Payout](https://stripe.com/docs/api#payout_object) object, with corresponding payout endpoints. For more
     information, read about the
     [transfer/payout split](https://stripe.com/docs/transfer-payout-split).
 
-    Related guide: [Creating Separate Charges and Transfers](https://stripe.com/docs/connect/charges-transfers).
+    Related guide: [Creating separate charges and transfers](https://stripe.com/docs/connect/charges-transfers)
     """
 
     OBJECT_NAME = "transfer"
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/__init__.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/credit_reversal.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/credit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/debit_reversal.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/debit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/inbound_transfer.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/outbound_payment.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/outbound_payment.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/outbound_transfer.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/received_credit.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/received_credit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/received_debit.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/received_debit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/treasury/transaction_entry.py` & `stripe-5.5.0b3/stripe/api_resources/treasury/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/api_resources/usage_record.py` & `stripe-5.5.0b3/stripe/api_resources/usage_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class UsageRecord(APIResource):
     """
     Usage records allow you to report customer usage and metrics to Stripe for
     metered billing of subscription prices.
 
-    Related guide: [Metered Billing](https://stripe.com/docs/billing/subscriptions/metered-billing).
+    Related guide: [Metered billing](https://stripe.com/docs/billing/subscriptions/metered-billing)
     """
 
     OBJECT_NAME = "usage_record"
 
     @classmethod
     def create(
         cls,
```

### Comparing `stripe-5.5.0b2/stripe/api_resources/webhook_endpoint.py` & `stripe-5.5.0b3/stripe/api_resources/webhook_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,11 @@
     """
     You can configure [webhook endpoints](https://stripe.com/docs/webhooks/) via the API to be
     notified about events that happen in your Stripe account or connected
     accounts.
 
     Most users configure webhooks from [the dashboard](https://dashboard.stripe.com/webhooks), which provides a user interface for registering and testing your webhook endpoints.
 
-    Related guide: [Setting up Webhooks](https://stripe.com/docs/webhooks/configure).
+    Related guide: [Setting up webhooks](https://stripe.com/docs/webhooks/configure)
     """
 
     OBJECT_NAME = "webhook_endpoint"
```

### Comparing `stripe-5.5.0b2/stripe/data/ca-certificates.crt` & `stripe-5.5.0b3/stripe/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/error.py` & `stripe-5.5.0b3/stripe/error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/http_client.py` & `stripe-5.5.0b3/stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/multipart_data_generator.py` & `stripe-5.5.0b3/stripe/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/oauth.py` & `stripe-5.5.0b3/stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/oauth_error.py` & `stripe-5.5.0b3/stripe/oauth_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/object_classes.py` & `stripe-5.5.0b3/stripe/object_classes.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/six.py` & `stripe-5.5.0b3/stripe/six.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/stripe_object.py` & `stripe-5.5.0b3/stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/stripe_response.py` & `stripe-5.5.0b3/stripe/stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/util.py` & `stripe-5.5.0b3/stripe/util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe/webhook.py` & `stripe-5.5.0b3/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/stripe.egg-info/PKG-INFO` & `stripe-5.5.0b3/stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b2
+Version: 5.5.0b3
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b2/stripe.egg-info/SOURCES.txt` & `stripe-5.5.0b3/stripe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 stripe/api_version.py
 stripe/error.py
 stripe/http_client.py
 stripe/multipart_data_generator.py
 stripe/oauth.py
 stripe/oauth_error.py
 stripe/object_classes.py
+stripe/preview.py
+stripe/raw_request.py
 stripe/request_metrics.py
 stripe/six.py
 stripe/stripe_object.py
 stripe/stripe_response.py
 stripe/util.py
 stripe/version.py
 stripe/webhook.py
@@ -191,14 +193,16 @@
 tests/test_error.py
 tests/test_generated_examples.py
 tests/test_http_client.py
 tests/test_integration.py
 tests/test_multipart_data_generator.py
 tests/test_oauth.py
 tests/test_oauth_error.py
+tests/test_preview.py
+tests/test_raw_request.py
 tests/test_stripe_object.py
 tests/test_stripe_response.py
 tests/test_util.py
 tests/test_webhook.py
 tests/api_resources/__init__.py
 tests/api_resources/test_account.py
 tests/api_resources/test_account_link.py
```

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_createable_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_custom_method.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_deletable_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_listable_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_nested_resource_class_methods.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_searchable_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_singleton_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_test_helpers_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_test_helpers_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/abstract/test_updateable_api_resource.py` & `stripe-5.5.0b3/tests/api_resources/abstract/test_updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/billing_portal/test_configuration.py` & `stripe-5.5.0b3/tests/api_resources/billing_portal/test_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/checkout/test_session.py` & `stripe-5.5.0b3/tests/api_resources/checkout/test_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/identity/test_verification_report.py` & `stripe-5.5.0b3/tests/api_resources/identity/test_verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/identity/test_verification_session.py` & `stripe-5.5.0b3/tests/api_resources/identity/test_verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/issuing/test_authorization.py` & `stripe-5.5.0b3/tests/api_resources/issuing/test_authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/issuing/test_card.py` & `stripe-5.5.0b3/tests/api_resources/issuing/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/issuing/test_cardholder.py` & `stripe-5.5.0b3/tests/api_resources/issuing/test_cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/issuing/test_dispute.py` & `stripe-5.5.0b3/tests/api_resources/issuing/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/issuing/test_transaction.py` & `stripe-5.5.0b3/tests/api_resources/issuing/test_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/radar/test_early_fraud_warning.py` & `stripe-5.5.0b3/tests/api_resources/radar/test_early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/radar/test_value_list.py` & `stripe-5.5.0b3/tests/api_resources/radar/test_value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/radar/test_value_list_item.py` & `stripe-5.5.0b3/tests/api_resources/radar/test_value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/reporting/test_report_run.py` & `stripe-5.5.0b3/tests/api_resources/reporting/test_report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/reporting/test_report_type.py` & `stripe-5.5.0b3/tests/api_resources/reporting/test_report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/sigma/test_scheduled_query_run.py` & `stripe-5.5.0b3/tests/api_resources/sigma/test_scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/terminal/test_location.py` & `stripe-5.5.0b3/tests/api_resources/terminal/test_location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/terminal/test_reader.py` & `stripe-5.5.0b3/tests/api_resources/terminal/test_reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_account.py` & `stripe-5.5.0b3/tests/api_resources/test_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_account_link.py` & `stripe-5.5.0b3/tests/api_resources/test_account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_apple_pay_domain.py` & `stripe-5.5.0b3/tests/api_resources/test_apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_application_fee.py` & `stripe-5.5.0b3/tests/api_resources/test_application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_application_fee_refund.py` & `stripe-5.5.0b3/tests/api_resources/test_application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_balance_transaction.py` & `stripe-5.5.0b3/tests/api_resources/test_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_bank_account.py` & `stripe-5.5.0b3/tests/api_resources/test_bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_capability.py` & `stripe-5.5.0b3/tests/api_resources/test_capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_card.py` & `stripe-5.5.0b3/tests/api_resources/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_charge.py` & `stripe-5.5.0b3/tests/api_resources/test_charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_country_spec.py` & `stripe-5.5.0b3/tests/api_resources/test_country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_coupon.py` & `stripe-5.5.0b3/tests/api_resources/test_coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_credit_note.py` & `stripe-5.5.0b3/tests/api_resources/test_credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_customer.py` & `stripe-5.5.0b3/tests/api_resources/test_customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_customer_balance_transaction.py` & `stripe-5.5.0b3/tests/api_resources/test_customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_dispute.py` & `stripe-5.5.0b3/tests/api_resources/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_ephemeral_key.py` & `stripe-5.5.0b3/tests/api_resources/test_ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_event.py` & `stripe-5.5.0b3/tests/api_resources/test_event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_exchange_rate.py` & `stripe-5.5.0b3/tests/api_resources/test_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_file.py` & `stripe-5.5.0b3/tests/api_resources/test_file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_file_link.py` & `stripe-5.5.0b3/tests/api_resources/test_file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_file_upload.py` & `stripe-5.5.0b3/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_invoice.py` & `stripe-5.5.0b3/tests/api_resources/test_invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_invoice_item.py` & `stripe-5.5.0b3/tests/api_resources/test_invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_list_object.py` & `stripe-5.5.0b3/tests/api_resources/test_list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_payment_intent.py` & `stripe-5.5.0b3/tests/api_resources/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_payment_method.py` & `stripe-5.5.0b3/tests/api_resources/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_payout.py` & `stripe-5.5.0b3/tests/api_resources/test_payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_person.py` & `stripe-5.5.0b3/tests/api_resources/test_person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_plan.py` & `stripe-5.5.0b3/tests/api_resources/test_plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_price.py` & `stripe-5.5.0b3/tests/api_resources/test_price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_product.py` & `stripe-5.5.0b3/tests/api_resources/test_product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_promotion_code.py` & `stripe-5.5.0b3/tests/api_resources/test_promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_quote.py` & `stripe-5.5.0b3/tests/api_resources/test_quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_refund.py` & `stripe-5.5.0b3/tests/api_resources/test_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_reversal.py` & `stripe-5.5.0b3/tests/api_resources/test_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_review.py` & `stripe-5.5.0b3/tests/api_resources/test_review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_search_result_object.py` & `stripe-5.5.0b3/tests/api_resources/test_search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_setup_intent.py` & `stripe-5.5.0b3/tests/api_resources/test_setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_source.py` & `stripe-5.5.0b3/tests/api_resources/test_source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_source_transaction.py` & `stripe-5.5.0b3/tests/api_resources/test_source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_subscription.py` & `stripe-5.5.0b3/tests/api_resources/test_subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_subscription_item.py` & `stripe-5.5.0b3/tests/api_resources/test_subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_subscription_schedule.py` & `stripe-5.5.0b3/tests/api_resources/test_subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_tax_code.py` & `stripe-5.5.0b3/tests/api_resources/test_tax_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_tax_id.py` & `stripe-5.5.0b3/tests/api_resources/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_tax_rate.py` & `stripe-5.5.0b3/tests/api_resources/test_tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_topup.py` & `stripe-5.5.0b3/tests/api_resources/test_topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_transfer.py` & `stripe-5.5.0b3/tests/api_resources/test_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_usage_record.py` & `stripe-5.5.0b3/tests/api_resources/test_usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_usage_record_summary.py` & `stripe-5.5.0b3/tests/api_resources/test_usage_record_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/api_resources/test_webhook_endpoint.py` & `stripe-5.5.0b3/tests/api_resources/test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/request_mock.py` & `stripe-5.5.0b3/tests/request_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,36 +108,44 @@
             msg = (
                 "Expected APIRequestor to have been constructed with "
                 "api_version='%s'. Constructed with api_version='%s' "
                 "instead." % (expected_api_version, actual_api_version)
             )
             raise AssertionError(msg)
 
-    def assert_requested(self, method, url, params=None, headers=None):
+    def assert_requested(
+        self, method, url, params=None, headers=None, api_mode=None
+    ):
         self.assert_requested_internal(
-            self.request_patcher, method, url, params, headers
+            self.request_patcher, method, url, params, headers, api_mode
         )
 
-    def assert_requested_stream(self, method, url, params=None, headers=None):
+    def assert_requested_stream(
+        self, method, url, params=None, headers=None, api_mode=None
+    ):
         self.assert_requested_internal(
-            self.request_stream_patcher, method, url, params, headers
+            self.request_stream_patcher, method, url, params, headers, api_mode
         )
 
-    def assert_requested_internal(self, patcher, method, url, params, headers):
+    def assert_requested_internal(
+        self, patcher, method, url, params, headers, api_mode
+    ):
         params = params or self._mocker.ANY
         headers = headers or self._mocker.ANY
+        api_mode = api_mode or self._mocker.ANY
         called = False
         exception = None
 
         # Sadly, ANY does not match a missing optional argument, so we
         # check all the possible signatures of the request method
         possible_called_args = [
             (self._mocker.ANY, method, url),
             (self._mocker.ANY, method, url, params),
             (self._mocker.ANY, method, url, params, headers),
+            (self._mocker.ANY, method, url, params, headers, api_mode),
         ]
 
         for args in possible_called_args:
             try:
                 patcher.assert_called_with(*args)
             except AssertionError as e:
                 exception = e
```

### Comparing `stripe-5.5.0b2/tests/stripe_mock.py` & `stripe-5.5.0b3/tests/stripe_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_api_requestor.py` & `stripe-5.5.0b3/tests/test_api_requestor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import uuid
 from collections import OrderedDict
 
 import pytest
 
 import stripe
 from stripe import six, util
+from stripe.api_requestor import _json_encode_date_callback
 from stripe.stripe_response import StripeResponse, StripeStreamResponse
 
 from stripe.six.moves.urllib.parse import urlsplit
 
 import urllib3
 
 VALID_API_METHODS = ("get", "post", "delete")
@@ -42,43 +43,47 @@
     def __init__(
         self,
         api_key=None,
         extra={},
         request_method=None,
         user_agent=None,
         app_info=None,
+        content_type=None,
         idempotency_key=None,
         fail_platform_call=False,
     ):
         self.request_method = request_method
         self.api_key = api_key or stripe.api_key
         self.extra = extra
         self.user_agent = user_agent
         self.app_info = app_info
+        self.content_type = content_type
         self.idempotency_key = idempotency_key
         self.fail_platform_call = fail_platform_call
 
     def __eq__(self, other):
         return (
             self._keys_match(other)
             and self._auth_match(other)
             and self._user_agent_match(other)
             and self._x_stripe_ua_contains_app_info(other)
             and self._x_stripe_ua_handles_failed_platform_function(other)
+            and self._content_type_match(other)
             and self._idempotency_key_match(other)
             and self._extra_match(other)
         )
 
     def __repr__(self):
-        return "APIHeaderMatcher(request_method=%s, api_key=%s, extra=%s, " "user_agent=%s, app_info=%s, idempotency_key=%s, fail_platform_call=%s)" % (
+        return "APIHeaderMatcher(request_method=%s, api_key=%s, extra=%s, " "user_agent=%s, app_info=%s, content_type=%s, idempotency_key=%s, fail_platform_call=%s)" % (
             repr(self.request_method),
             repr(self.api_key),
             repr(self.extra),
             repr(self.user_agent),
             repr(self.app_info),
+            repr(self.content_type),
             repr(self.idempotency_key),
             repr(self.fail_platform_call),
         )
 
     def _keys_match(self, other):
         expected_keys = list(set(self.EXP_KEYS + list(self.extra.keys())))
         if (
@@ -93,14 +98,20 @@
 
     def _user_agent_match(self, other):
         if self.user_agent is not None:
             return other["User-Agent"] == self.user_agent
 
         return True
 
+    def _content_type_match(self, other):
+        if self.content_type is not None:
+            return other["Content-Type"] == self.content_type
+
+        return True
+
     def _idempotency_key_match(self, other):
         if self.idempotency_key is not None:
             return other["Idempotency-Key"] == self.idempotency_key
         return True
 
     def _x_stripe_ua_contains_app_info(self, other):
         if self.app_info:
@@ -226,68 +237,18 @@
         yield
         stripe.api_key = orig_attrs["api_key"]
         stripe.api_version = orig_attrs["api_version"]
         stripe.default_http_client = orig_attrs["default_http_client"]
         stripe.enable_telemetry = orig_attrs["enable_telemetry"]
 
     @pytest.fixture
-    def http_client(self, mocker):
-        http_client = mocker.Mock(stripe.http_client.HTTPClient)
-        http_client._verify_ssl_certs = True
-        http_client.name = "mockclient"
-        return http_client
-
-    @pytest.fixture
     def requestor(self, http_client):
         requestor = stripe.api_requestor.APIRequestor(client=http_client)
         return requestor
 
-    @pytest.fixture
-    def mock_response(self, mocker, http_client):
-        def mock_response(return_body, return_code, headers=None):
-            http_client.request_with_retries = mocker.Mock(
-                return_value=(return_body, return_code, headers or {})
-            )
-
-        return mock_response
-
-    @pytest.fixture
-    def mock_streaming_response(self, mocker, http_client):
-        def mock_streaming_response(return_body, return_code, headers=None):
-            http_client.request_stream_with_retries = mocker.Mock(
-                return_value=(return_body, return_code, headers or {})
-            )
-
-        return mock_streaming_response
-
-    @pytest.fixture
-    def check_call(self, http_client):
-        def check_call(
-            method,
-            abs_url=None,
-            headers=None,
-            post_data=None,
-            is_streaming=False,
-        ):
-            if not abs_url:
-                abs_url = "%s%s" % (stripe.api_base, self.valid_path)
-            if not headers:
-                headers = APIHeaderMatcher(request_method=method)
-
-            if is_streaming:
-                http_client.request_stream_with_retries.assert_called_with(
-                    method, abs_url, headers, post_data
-                )
-            else:
-                http_client.request_with_retries.assert_called_with(
-                    method, abs_url, headers, post_data
-                )
-
-        return check_call
-
     @property
     def valid_path(self):
         return "/foo"
 
     def encoder_check(self, key):
         stk_key = "my%s" % (key,)
 
@@ -325,14 +286,35 @@
 
         expectation = []
         for type_, values in six.iteritems(self.ENCODE_EXPECTATIONS):
             expectation.extend([(k % (type_,), str(v)) for k, v in values])
 
         check_call("get", QueryMatcher(expectation))
 
+    def test_param_api_mode_preview(
+        self, requestor, mock_response, check_call
+    ):
+        mock_response("{}", 200)
+
+        requestor.request(
+            "post", self.valid_path, self.ENCODE_INPUTS, api_mode="preview"
+        )
+
+        expectation = json.dumps(
+            self.ENCODE_INPUTS, default=_json_encode_date_callback
+        )
+
+        check_call(
+            "post",
+            headers=APIHeaderMatcher(
+                content_type="application/json", request_method="post"
+            ),
+            post_data=expectation,
+        )
+
     def test_dictionary_list_encoding(self):
         params = {"foo": {"0": {"bar": "bat"}}}
         encoded = list(stripe.api_requestor._api_encode(params))
         key, value = encoded[0]
 
         assert key == "foo[0][bar]"
         assert value == "bat"
```

### Comparing `stripe-5.5.0b2/tests/test_error.py` & `stripe-5.5.0b3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_generated_examples.py` & `stripe-5.5.0b3/tests/test_generated_examples.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 import stripe
 
 
 class TestGeneratedExamples(object):
     def test_apps_secret_list(self, request_mock):
-        stripe.apps.Secret.list(scope={"type": "account"}, limit=2)
-        request_mock.assert_requested("get", "/v1/apps/secrets")
+        stripe.apps.Secret.list(
+            scope={"type": "account"},
+            limit=2,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/apps/secrets",
+        )
 
     def test_apps_secret_create(self, request_mock):
         stripe.apps.Secret.create(
             name="sec_123",
             payload="very secret string",
             scope={"type": "account"},
         )
-        request_mock.assert_requested("post", "/v1/apps/secrets")
+        request_mock.assert_requested(
+            "post",
+            "/v1/apps/secrets",
+        )
 
     def test_apps_secret_delete_where(self, request_mock):
         stripe.apps.Secret.delete_where(
             name="my-api-key",
             scope={"type": "account"},
         )
-        request_mock.assert_requested("post", "/v1/apps/secrets/delete")
+        request_mock.assert_requested(
+            "post",
+            "/v1/apps/secrets/delete",
+        )
 
     def test_apps_secret_find(self, request_mock):
-        stripe.apps.Secret.find(name="sec_123", scope={"type": "account"})
-        request_mock.assert_requested("get", "/v1/apps/secrets/find")
+        stripe.apps.Secret.find(
+            name="sec_123",
+            scope={"type": "account"},
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/apps/secrets/find",
+        )
 
     def test_checkout_session_create(self, request_mock):
         stripe.checkout.Session.create(
             success_url="https://example.com/success",
             cancel_url="https://example.com/cancel",
             mode="payment",
             shipping_options=[
@@ -41,15 +59,18 @@
                             "minimum": {"unit": "day", "value": 5},
                             "maximum": {"unit": "day", "value": 7},
                         },
                     },
                 },
             ],
         )
-        request_mock.assert_requested("post", "/v1/checkout/sessions")
+        request_mock.assert_requested(
+            "post",
+            "/v1/checkout/sessions",
+        )
 
     def test_checkout_session_expire(self, request_mock):
         stripe.checkout.Session.expire("sess_xyz")
         request_mock.assert_requested(
             "post",
             "/v1/checkout/sessions/sess_xyz/expire",
         )
@@ -60,24 +81,26 @@
             "get",
             "/v1/checkout/sessions/sess_xyz/line_items",
         )
 
     def test_customer_cashbalance_retrieve(self, request_mock):
         stripe.Customer.retrieve_cash_balance("cus_123")
         request_mock.assert_requested(
-            "get", "/v1/customers/cus_123/cash_balance"
+            "get",
+            "/v1/customers/cus_123/cash_balance",
         )
 
     def test_customer_cashbalance_update(self, request_mock):
         stripe.Customer.modify_cash_balance(
             "cus_123",
             settings={"reconciliation_mode": "manual"},
         )
         request_mock.assert_requested(
-            "post", "/v1/customers/cus_123/cash_balance"
+            "post",
+            "/v1/customers/cus_123/cash_balance",
         )
 
     def test_customer_create_funding_instructions(self, request_mock):
         stripe.Customer.create_funding_instructions(
             "cus_123",
             bank_transfer={
                 "requested_address_types": ["zengin"],
@@ -88,24 +111,28 @@
         )
         request_mock.assert_requested(
             "post",
             "/v1/customers/cus_123/funding_instructions",
         )
 
     def test_customer_list_payment_methods(self, request_mock):
-        stripe.Customer.list_payment_methods("cus_xyz", type="card")
+        stripe.Customer.list_payment_methods(
+            "cus_xyz",
+            type="card",
+        )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xyz/payment_methods",
         )
 
     def test_financial_connections_account_list(self, request_mock):
         stripe.financial_connections.Account.list()
         request_mock.assert_requested(
-            "get", "/v1/financial_connections/accounts"
+            "get",
+            "/v1/financial_connections/accounts",
         )
 
     def test_financial_connections_account_retrieve(self, request_mock):
         stripe.financial_connections.Account.retrieve("fca_xyz")
         request_mock.assert_requested(
             "get",
             "/v1/financial_connections/accounts/fca_xyz",
@@ -140,123 +167,160 @@
 
     def test_financial_connections_session_create(self, request_mock):
         stripe.financial_connections.Session.create(
             account_holder={"type": "customer", "customer": "cus_123"},
             permissions=["balances"],
         )
         request_mock.assert_requested(
-            "post", "/v1/financial_connections/sessions"
+            "post",
+            "/v1/financial_connections/sessions",
         )
 
     def test_financial_connections_session_retrieve(self, request_mock):
         stripe.financial_connections.Session.retrieve("fcsess_xyz")
         request_mock.assert_requested(
             "get",
             "/v1/financial_connections/sessions/fcsess_xyz",
         )
 
     def test_invoice_upcoming(self, request_mock):
         stripe.Invoice.upcoming(customer="cus_9utnxg47pWjV1e")
-        request_mock.assert_requested("get", "/v1/invoices/upcoming")
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoices/upcoming",
+        )
 
     def test_paymentintent_create(self, request_mock):
         stripe.PaymentIntent.create(
             amount=1099,
             currency="eur",
             automatic_payment_methods={"enabled": True},
         )
-        request_mock.assert_requested("post", "/v1/payment_intents")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_intents",
+        )
 
     def test_paymentintent_verify_microdeposits(self, request_mock):
         stripe.PaymentIntent.verify_microdeposits("pi_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/payment_intents/pi_xxxxxxxxxxxxx/verify_microdeposits",
         )
 
     def test_paymentlink_create(self, request_mock):
         stripe.PaymentLink.create(
             line_items=[{"price": "price_xxxxxxxxxxxxx", "quantity": 1}],
         )
-        request_mock.assert_requested("post", "/v1/payment_links")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_links",
+        )
 
     def test_paymentlink_retrieve(self, request_mock):
         stripe.PaymentLink.retrieve("pl_xyz")
-        request_mock.assert_requested("get", "/v1/payment_links/pl_xyz")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payment_links/pl_xyz",
+        )
 
     def test_paymentlink_list_line_items(self, request_mock):
         stripe.PaymentLink.list_line_items("pl_xyz")
         request_mock.assert_requested(
-            "get", "/v1/payment_links/pl_xyz/line_items"
+            "get",
+            "/v1/payment_links/pl_xyz/line_items",
         )
 
     def test_price_create(self, request_mock):
         stripe.Price.create(
             unit_amount=2000,
             currency="usd",
             currency_options={
                 "uah": {"unit_amount": 5000},
                 "eur": {"unit_amount": 1800},
             },
             recurring={"interval": "month"},
             product="prod_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/prices")
+        request_mock.assert_requested(
+            "post",
+            "/v1/prices",
+        )
 
     def test_setupattempt_list(self, request_mock):
-        stripe.SetupAttempt.list(limit=3, setup_intent="si_xyz")
-        request_mock.assert_requested("get", "/v1/setup_attempts")
+        stripe.SetupAttempt.list(
+            limit=3,
+            setup_intent="si_xyz",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/setup_attempts",
+        )
 
     def test_setupintent_verify_microdeposits(self, request_mock):
         stripe.SetupIntent.verify_microdeposits("seti_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/setup_intents/seti_xxxxxxxxxxxxx/verify_microdeposits",
         )
 
     def test_shippingrate_list(self, request_mock):
         stripe.ShippingRate.list()
-        request_mock.assert_requested("get", "/v1/shipping_rates")
+        request_mock.assert_requested(
+            "get",
+            "/v1/shipping_rates",
+        )
 
     def test_shippingrate_create(self, request_mock):
         stripe.ShippingRate.create(
             display_name="Sample Shipper",
             fixed_amount={"currency": "usd", "amount": 400},
             type="fixed_amount",
         )
-        request_mock.assert_requested("post", "/v1/shipping_rates")
+        request_mock.assert_requested(
+            "post",
+            "/v1/shipping_rates",
+        )
 
     def test_terminal_configuration_list(self, request_mock):
         stripe.terminal.Configuration.list()
-        request_mock.assert_requested("get", "/v1/terminal/configurations")
+        request_mock.assert_requested(
+            "get",
+            "/v1/terminal/configurations",
+        )
 
     def test_terminal_configuration_create(self, request_mock):
         stripe.terminal.Configuration.create()
-        request_mock.assert_requested("post", "/v1/terminal/configurations")
+        request_mock.assert_requested(
+            "post",
+            "/v1/terminal/configurations",
+        )
 
     def test_terminal_configuration_delete(self, request_mock):
         stripe.terminal.Configuration.delete("uc_123")
         request_mock.assert_requested(
             "delete",
             "/v1/terminal/configurations/uc_123",
         )
 
     def test_terminal_configuration_retrieve(self, request_mock):
         stripe.terminal.Configuration.retrieve("uc_123")
         request_mock.assert_requested(
-            "get", "/v1/terminal/configurations/uc_123"
+            "get",
+            "/v1/terminal/configurations/uc_123",
         )
 
     def test_terminal_configuration_update(self, request_mock):
         stripe.terminal.Configuration.modify(
             "uc_123",
             tipping={"usd": {"fixed_amounts": [10]}},
         )
         request_mock.assert_requested(
-            "post", "/v1/terminal/configurations/uc_123"
+            "post",
+            "/v1/terminal/configurations/uc_123",
         )
 
     def test_customer_fund_cash_balance(self, request_mock):
         stripe.Customer.TestHelpers.fund_cash_balance(
             "cus_123",
             amount=30,
             currency="eur",
@@ -299,19 +363,28 @@
         request_mock.assert_requested(
             "post",
             "/v1/test_helpers/refunds/re_123/expire",
         )
 
     def test_test_helpers_testclock_list(self, request_mock):
         stripe.test_helpers.TestClock.list()
-        request_mock.assert_requested("get", "/v1/test_helpers/test_clocks")
+        request_mock.assert_requested(
+            "get",
+            "/v1/test_helpers/test_clocks",
+        )
 
     def test_test_helpers_testclock_create(self, request_mock):
-        stripe.test_helpers.TestClock.create(frozen_time=123, name="cogsworth")
-        request_mock.assert_requested("post", "/v1/test_helpers/test_clocks")
+        stripe.test_helpers.TestClock.create(
+            frozen_time=123,
+            name="cogsworth",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/test_helpers/test_clocks",
+        )
 
     def test_test_helpers_testclock_delete(self, request_mock):
         stripe.test_helpers.TestClock.delete("clock_xyz")
         request_mock.assert_requested(
             "delete",
             "/v1/test_helpers/test_clocks/clock_xyz",
         )
@@ -320,15 +393,18 @@
         stripe.test_helpers.TestClock.retrieve("clock_xyz")
         request_mock.assert_requested(
             "get",
             "/v1/test_helpers/test_clocks/clock_xyz",
         )
 
     def test_test_helpers_testclock_advance(self, request_mock):
-        stripe.test_helpers.TestClock.advance("clock_xyz", frozen_time=142)
+        stripe.test_helpers.TestClock.advance(
+            "clock_xyz",
+            frozen_time=142,
+        )
         request_mock.assert_requested(
             "post",
             "/v1/test_helpers/test_clocks/clock_xyz/advance",
         )
 
     def test_treasury_inboundtransfer_fail(self, request_mock):
         stripe.treasury.InboundTransfer.TestHelpers.fail(
@@ -413,69 +489,91 @@
             card={
                 "number": "4242424242424242",
                 "exp_month": "5",
                 "exp_year": "2023",
                 "cvc": "314",
             },
         )
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_accountlink_create(self, request_mock):
         stripe.AccountLink.create(
             account="acct_xxxxxxxxxxxxx",
             refresh_url="https://example.com/reauth",
             return_url="https://example.com/return",
             type="account_onboarding",
         )
-        request_mock.assert_requested("post", "/v1/account_links")
+        request_mock.assert_requested(
+            "post",
+            "/v1/account_links",
+        )
 
     def test_account_list(self, request_mock):
         stripe.Account.list(limit=3)
-        request_mock.assert_requested("get", "/v1/accounts")
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts",
+        )
 
     def test_account_create(self, request_mock):
         stripe.Account.create(
             type="custom",
             country="US",
             email="jenny.rosen@example.com",
             capabilities={
                 "card_payments": {"requested": True},
                 "transfers": {"requested": True},
             },
         )
-        request_mock.assert_requested("post", "/v1/accounts")
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts",
+        )
 
     def test_account_delete(self, request_mock):
         stripe.Account.delete("acct_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/accounts/acct_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/accounts/acct_xxxxxxxxxxxxx",
         )
 
     def test_account_retrieve(self, request_mock):
         stripe.Account.retrieve("acct_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/accounts/acct_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx",
+        )
 
     def test_account_update(self, request_mock):
         stripe.Account.modify(
-            "acct_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "acct_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/accounts/acct_xxxxxxxxxxxxx"
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx",
         )
 
     def test_account_reject(self, request_mock):
-        stripe.Account.reject("acct_xxxxxxxxxxxxx", reason="fraud")
+        stripe.Account.reject(
+            "acct_xxxxxxxxxxxxx",
+            reason="fraud",
+        )
         request_mock.assert_requested(
             "post",
             "/v1/accounts/acct_xxxxxxxxxxxxx/reject",
         )
 
     def test_account_capability_retrieve(self, request_mock):
         stripe.Account.retrieve_capability(
-            "acct_xxxxxxxxxxxxx", "card_payments"
+            "acct_xxxxxxxxxxxxx",
+            "card_payments",
         )
         request_mock.assert_requested(
             "get",
             "/v1/accounts/acct_xxxxxxxxxxxxx/capabilities/card_payments",
         )
 
     def test_account_capability_update(self, request_mock):
@@ -487,15 +585,16 @@
         request_mock.assert_requested(
             "post",
             "/v1/accounts/acct_xxxxxxxxxxxxx/capabilities/card_payments",
         )
 
     def test_account_person_retrieve(self, request_mock):
         stripe.Account.retrieve_person(
-            "acct_xxxxxxxxxxxxx", "person_xxxxxxxxxxxxx"
+            "acct_xxxxxxxxxxxxx",
+            "person_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
             "/v1/accounts/acct_xxxxxxxxxxxxx/persons/person_xxxxxxxxxxxxx",
         )
 
     def test_account_person_update(self, request_mock):
@@ -507,15 +606,18 @@
         request_mock.assert_requested(
             "post",
             "/v1/accounts/acct_xxxxxxxxxxxxx/persons/person_xxxxxxxxxxxxx",
         )
 
     def test_applicationfee_list(self, request_mock):
         stripe.ApplicationFee.list(limit=3)
-        request_mock.assert_requested("get", "/v1/application_fees")
+        request_mock.assert_requested(
+            "get",
+            "/v1/application_fees",
+        )
 
     def test_applicationfee_retrieve(self, request_mock):
         stripe.ApplicationFee.retrieve("fee_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/application_fees/fee_xxxxxxxxxxxxx",
         )
@@ -538,40 +640,53 @@
         )
         request_mock.assert_requested(
             "post",
             "/v1/application_fees/fee_xxxxxxxxxxxxx/refunds/fr_xxxxxxxxxxxxx",
         )
 
     def test_apps_secret_list2(self, request_mock):
-        stripe.apps.Secret.list(scope={"type": "account"}, limit=2)
-        request_mock.assert_requested("get", "/v1/apps/secrets")
+        stripe.apps.Secret.list(
+            scope={"type": "account"},
+            limit=2,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/apps/secrets",
+        )
 
     def test_apps_secret_create2(self, request_mock):
         stripe.apps.Secret.create(
             name="my-api-key",
             payload="secret_key_xxxxxx",
             scope={"type": "account"},
         )
-        request_mock.assert_requested("post", "/v1/apps/secrets")
+        request_mock.assert_requested(
+            "post",
+            "/v1/apps/secrets",
+        )
 
     def test_balancetransaction_list(self, request_mock):
         stripe.BalanceTransaction.list(limit=3)
-        request_mock.assert_requested("get", "/v1/balance_transactions")
+        request_mock.assert_requested(
+            "get",
+            "/v1/balance_transactions",
+        )
 
     def test_balancetransaction_retrieve(self, request_mock):
         stripe.BalanceTransaction.retrieve("txn_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/balance_transactions/txn_xxxxxxxxxxxxx",
         )
 
     def test_billing_portal_configuration_list(self, request_mock):
         stripe.billing_portal.Configuration.list(limit=3)
         request_mock.assert_requested(
-            "get", "/v1/billing_portal/configurations"
+            "get",
+            "/v1/billing_portal/configurations",
         )
 
     def test_billing_portal_configuration_create(self, request_mock):
         stripe.billing_portal.Configuration.create(
             features={
                 "customer_update": {
                     "allowed_updates": ["email", "tax_id"],
@@ -581,15 +696,16 @@
             },
             business_profile={
                 "privacy_policy_url": "https://example.com/privacy",
                 "terms_of_service_url": "https://example.com/terms",
             },
         )
         request_mock.assert_requested(
-            "post", "/v1/billing_portal/configurations"
+            "post",
+            "/v1/billing_portal/configurations",
         )
 
     def test_billing_portal_configuration_retrieve(self, request_mock):
         stripe.billing_portal.Configuration.retrieve("bpc_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/billing_portal/configurations/bpc_xxxxxxxxxxxxx",
@@ -609,61 +725,88 @@
         )
 
     def test_billing_portal_session_create(self, request_mock):
         stripe.billing_portal.Session.create(
             customer="cus_xxxxxxxxxxxxx",
             return_url="https://example.com/account",
         )
-        request_mock.assert_requested("post", "/v1/billing_portal/sessions")
+        request_mock.assert_requested(
+            "post",
+            "/v1/billing_portal/sessions",
+        )
 
     def test_charge_list(self, request_mock):
         stripe.Charge.list(limit=3)
-        request_mock.assert_requested("get", "/v1/charges")
+        request_mock.assert_requested(
+            "get",
+            "/v1/charges",
+        )
 
     def test_charge_create(self, request_mock):
         stripe.Charge.create(
             amount=2000,
             currency="usd",
             source="tok_xxxx",
             description="My First Test Charge (created for API docs at https://www.stripe.com/docs/api)",
         )
-        request_mock.assert_requested("post", "/v1/charges")
+        request_mock.assert_requested(
+            "post",
+            "/v1/charges",
+        )
 
     def test_charge_retrieve(self, request_mock):
         stripe.Charge.retrieve("ch_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/charges/ch_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/charges/ch_xxxxxxxxxxxxx",
+        )
 
     def test_charge_update(self, request_mock):
-        stripe.Charge.modify("ch_xxxxxxxxxxxxx", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/charges/ch_xxxxxxxxxxxxx")
+        stripe.Charge.modify(
+            "ch_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/charges/ch_xxxxxxxxxxxxx",
+        )
 
     def test_charge_capture(self, request_mock):
         stripe.Charge.capture("ch_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/charges/ch_xxxxxxxxxxxxx/capture",
         )
 
     def test_charge_search(self, request_mock):
         stripe.Charge.search(
             query="amount>999 AND metadata['order_id']:'6735'"
         )
-        request_mock.assert_requested("get", "/v1/charges/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/charges/search",
+        )
 
     def test_checkout_session_list(self, request_mock):
         stripe.checkout.Session.list(limit=3)
-        request_mock.assert_requested("get", "/v1/checkout/sessions")
+        request_mock.assert_requested(
+            "get",
+            "/v1/checkout/sessions",
+        )
 
     def test_checkout_session_create2(self, request_mock):
         stripe.checkout.Session.create(
             success_url="https://example.com/success",
             line_items=[{"price": "price_xxxxxxxxxxxxx", "quantity": 2}],
             mode="payment",
         )
-        request_mock.assert_requested("post", "/v1/checkout/sessions")
+        request_mock.assert_requested(
+            "post",
+            "/v1/checkout/sessions",
+        )
 
     def test_checkout_session_retrieve(self, request_mock):
         stripe.checkout.Session.retrieve("cs_test_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/checkout/sessions/cs_test_xxxxxxxxxxxxx",
         )
@@ -673,60 +816,90 @@
         request_mock.assert_requested(
             "post",
             "/v1/checkout/sessions/cs_test_xxxxxxxxxxxxx/expire",
         )
 
     def test_countryspec_list(self, request_mock):
         stripe.CountrySpec.list(limit=3)
-        request_mock.assert_requested("get", "/v1/country_specs")
+        request_mock.assert_requested(
+            "get",
+            "/v1/country_specs",
+        )
 
     def test_countryspec_retrieve(self, request_mock):
         stripe.CountrySpec.retrieve("US")
-        request_mock.assert_requested("get", "/v1/country_specs/US")
+        request_mock.assert_requested(
+            "get",
+            "/v1/country_specs/US",
+        )
 
     def test_coupon_list(self, request_mock):
         stripe.Coupon.list(limit=3)
-        request_mock.assert_requested("get", "/v1/coupons")
+        request_mock.assert_requested(
+            "get",
+            "/v1/coupons",
+        )
 
     def test_coupon_create(self, request_mock):
         stripe.Coupon.create(
             percent_off=25.5,
             duration="repeating",
             duration_in_months=3,
         )
-        request_mock.assert_requested("post", "/v1/coupons")
+        request_mock.assert_requested(
+            "post",
+            "/v1/coupons",
+        )
 
     def test_coupon_delete(self, request_mock):
         stripe.Coupon.delete("Z4OV52SU")
-        request_mock.assert_requested("delete", "/v1/coupons/Z4OV52SU")
+        request_mock.assert_requested(
+            "delete",
+            "/v1/coupons/Z4OV52SU",
+        )
 
     def test_coupon_retrieve(self, request_mock):
         stripe.Coupon.retrieve("Z4OV52SU")
-        request_mock.assert_requested("get", "/v1/coupons/Z4OV52SU")
+        request_mock.assert_requested(
+            "get",
+            "/v1/coupons/Z4OV52SU",
+        )
 
     def test_coupon_update(self, request_mock):
-        stripe.Coupon.modify("Z4OV52SU", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/coupons/Z4OV52SU")
+        stripe.Coupon.modify(
+            "Z4OV52SU",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/coupons/Z4OV52SU",
+        )
 
     def test_creditnote_list(self, request_mock):
         stripe.CreditNote.list(limit=3)
-        request_mock.assert_requested("get", "/v1/credit_notes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/credit_notes",
+        )
 
     def test_creditnote_create(self, request_mock):
         stripe.CreditNote.create(
             invoice="in_xxxxxxxxxxxxx",
             lines=[
                 {
                     "type": "invoice_line_item",
                     "invoice_line_item": "il_xxxxxxxxxxxxx",
                     "quantity": 1,
                 },
             ],
         )
-        request_mock.assert_requested("post", "/v1/credit_notes")
+        request_mock.assert_requested(
+            "post",
+            "/v1/credit_notes",
+        )
 
     def test_creditnote_void_credit_note(self, request_mock):
         stripe.CreditNote.void_credit_note("cn_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/credit_notes/cn_xxxxxxxxxxxxx/void",
         )
@@ -738,150 +911,211 @@
                 {
                     "type": "invoice_line_item",
                     "invoice_line_item": "il_xxxxxxxxxxxxx",
                     "quantity": 1,
                 },
             ],
         )
-        request_mock.assert_requested("get", "/v1/credit_notes/preview")
+        request_mock.assert_requested(
+            "get",
+            "/v1/credit_notes/preview",
+        )
 
     def test_customer_list(self, request_mock):
         stripe.Customer.list(limit=3)
-        request_mock.assert_requested("get", "/v1/customers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers",
+        )
 
     def test_customer_list2(self, request_mock):
         stripe.Customer.list(limit=3)
-        request_mock.assert_requested("get", "/v1/customers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers",
+        )
 
     def test_customer_create(self, request_mock):
         stripe.Customer.create(
             description="My First Test Customer (created for API docs at https://www.stripe.com/docs/api)",
         )
-        request_mock.assert_requested("post", "/v1/customers")
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers",
+        )
 
     def test_customer_delete(self, request_mock):
         stripe.Customer.delete("cus_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/customers/cus_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/customers/cus_xxxxxxxxxxxxx",
         )
 
     def test_customer_retrieve(self, request_mock):
         stripe.Customer.retrieve("cus_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/customers/cus_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx",
+        )
 
     def test_customer_update(self, request_mock):
         stripe.Customer.modify(
-            "cus_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "cus_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/customers/cus_xxxxxxxxxxxxx"
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx",
         )
 
     def test_customer_customerbalancetransaction_retrieve(self, request_mock):
         stripe.Customer.retrieve_balance_transaction(
             "cus_xxxxxxxxxxxxx",
             "cbtxn_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xxxxxxxxxxxxx/balance_transactions/cbtxn_xxxxxxxxxxxxx",
         )
 
     def test_customer_list_payment_methods2(self, request_mock):
-        stripe.Customer.list_payment_methods("cus_xxxxxxxxxxxxx", type="card")
+        stripe.Customer.list_payment_methods(
+            "cus_xxxxxxxxxxxxx",
+            type="card",
+        )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xxxxxxxxxxxxx/payment_methods",
         )
 
     def test_customer_taxid_retrieve(self, request_mock):
         stripe.Customer.retrieve_tax_id(
-            "cus_xxxxxxxxxxxxx", "txi_xxxxxxxxxxxxx"
+            "cus_xxxxxxxxxxxxx",
+            "txi_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xxxxxxxxxxxxx/tax_ids/txi_xxxxxxxxxxxxx",
         )
 
     def test_customer_search(self, request_mock):
         stripe.Customer.search(
             query="name:'fakename' AND metadata['foo']:'bar'"
         )
-        request_mock.assert_requested("get", "/v1/customers/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/search",
+        )
 
     def test_customer_search2(self, request_mock):
         stripe.Customer.search(
             query="name:'fakename' AND metadata['foo']:'bar'"
         )
-        request_mock.assert_requested("get", "/v1/customers/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/search",
+        )
 
     def test_dispute_list(self, request_mock):
         stripe.Dispute.list(limit=3)
-        request_mock.assert_requested("get", "/v1/disputes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/disputes",
+        )
 
     def test_dispute_retrieve(self, request_mock):
         stripe.Dispute.retrieve("dp_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/disputes/dp_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/disputes/dp_xxxxxxxxxxxxx",
+        )
 
     def test_dispute_update(self, request_mock):
         stripe.Dispute.modify(
-            "dp_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "dp_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/disputes/dp_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/disputes/dp_xxxxxxxxxxxxx")
 
     def test_dispute_close(self, request_mock):
         stripe.Dispute.close("dp_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/disputes/dp_xxxxxxxxxxxxx/close"
+            "post",
+            "/v1/disputes/dp_xxxxxxxxxxxxx/close",
         )
 
     def test_event_list(self, request_mock):
         stripe.Event.list(limit=3)
-        request_mock.assert_requested("get", "/v1/events")
+        request_mock.assert_requested(
+            "get",
+            "/v1/events",
+        )
 
     def test_event_retrieve(self, request_mock):
         stripe.Event.retrieve("evt_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/events/evt_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/events/evt_xxxxxxxxxxxxx",
+        )
 
     def test_filelink_list(self, request_mock):
         stripe.FileLink.list(limit=3)
-        request_mock.assert_requested("get", "/v1/file_links")
+        request_mock.assert_requested(
+            "get",
+            "/v1/file_links",
+        )
 
     def test_filelink_create(self, request_mock):
         stripe.FileLink.create(file="file_xxxxxxxxxxxxx")
-        request_mock.assert_requested("post", "/v1/file_links")
+        request_mock.assert_requested(
+            "post",
+            "/v1/file_links",
+        )
 
     def test_filelink_retrieve(self, request_mock):
         stripe.FileLink.retrieve("link_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/file_links/link_xxxxxxxxxxxxx"
+            "get",
+            "/v1/file_links/link_xxxxxxxxxxxxx",
         )
 
     def test_filelink_update(self, request_mock):
         stripe.FileLink.modify(
-            "link_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "link_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/file_links/link_xxxxxxxxxxxxx"
+            "post",
+            "/v1/file_links/link_xxxxxxxxxxxxx",
         )
 
     def test_file_list(self, request_mock):
         stripe.File.list(limit=3)
-        request_mock.assert_requested("get", "/v1/files")
+        request_mock.assert_requested(
+            "get",
+            "/v1/files",
+        )
 
     def test_file_retrieve(self, request_mock):
         stripe.File.retrieve("file_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/files/file_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/files/file_xxxxxxxxxxxxx",
+        )
 
     def test_financial_connections_account_list2(self, request_mock):
         stripe.financial_connections.Account.list(
             account_holder={"customer": "cus_xxxxxxxxxxxxx"},
         )
         request_mock.assert_requested(
-            "get", "/v1/financial_connections/accounts"
+            "get",
+            "/v1/financial_connections/accounts",
         )
 
     def test_financial_connections_account_retrieve2(self, request_mock):
         stripe.financial_connections.Account.retrieve("fca_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/financial_connections/accounts/fca_xxxxxxxxxxxxx",
@@ -911,47 +1145,51 @@
                 "type": "customer",
                 "customer": "cus_xxxxxxxxxxxxx",
             },
             permissions=["payment_method", "balances"],
             filters={"countries": ["US"]},
         )
         request_mock.assert_requested(
-            "post", "/v1/financial_connections/sessions"
+            "post",
+            "/v1/financial_connections/sessions",
         )
 
     def test_financial_connections_session_retrieve2(self, request_mock):
         stripe.financial_connections.Session.retrieve("fcsess_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/financial_connections/sessions/fcsess_xxxxxxxxxxxxx",
         )
 
     def test_identity_verificationreport_list(self, request_mock):
         stripe.identity.VerificationReport.list(limit=3)
         request_mock.assert_requested(
-            "get", "/v1/identity/verification_reports"
+            "get",
+            "/v1/identity/verification_reports",
         )
 
     def test_identity_verificationreport_retrieve(self, request_mock):
         stripe.identity.VerificationReport.retrieve("vr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/identity/verification_reports/vr_xxxxxxxxxxxxx",
         )
 
     def test_identity_verificationsession_list(self, request_mock):
         stripe.identity.VerificationSession.list(limit=3)
         request_mock.assert_requested(
-            "get", "/v1/identity/verification_sessions"
+            "get",
+            "/v1/identity/verification_sessions",
         )
 
     def test_identity_verificationsession_create(self, request_mock):
         stripe.identity.VerificationSession.create(type="document")
         request_mock.assert_requested(
-            "post", "/v1/identity/verification_sessions"
+            "post",
+            "/v1/identity/verification_sessions",
         )
 
     def test_identity_verificationsession_retrieve(self, request_mock):
         stripe.identity.VerificationSession.retrieve("vs_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/identity/verification_sessions/vs_xxxxxxxxxxxxx",
@@ -979,70 +1217,100 @@
         request_mock.assert_requested(
             "post",
             "/v1/identity/verification_sessions/vs_xxxxxxxxxxxxx/redact",
         )
 
     def test_invoiceitem_list(self, request_mock):
         stripe.InvoiceItem.list(limit=3)
-        request_mock.assert_requested("get", "/v1/invoiceitems")
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoiceitems",
+        )
 
     def test_invoiceitem_create(self, request_mock):
         stripe.InvoiceItem.create(
             customer="cus_xxxxxxxxxxxxx",
             price="price_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/invoiceitems")
+        request_mock.assert_requested(
+            "post",
+            "/v1/invoiceitems",
+        )
 
     def test_invoiceitem_delete(self, request_mock):
         stripe.InvoiceItem.delete("ii_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/invoiceitems/ii_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/invoiceitems/ii_xxxxxxxxxxxxx",
         )
 
     def test_invoiceitem_retrieve(self, request_mock):
         stripe.InvoiceItem.retrieve("ii_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/invoiceitems/ii_xxxxxxxxxxxxx"
+            "get",
+            "/v1/invoiceitems/ii_xxxxxxxxxxxxx",
         )
 
     def test_invoiceitem_update(self, request_mock):
         stripe.InvoiceItem.modify(
-            "ii_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "ii_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/invoiceitems/ii_xxxxxxxxxxxxx"
+            "post",
+            "/v1/invoiceitems/ii_xxxxxxxxxxxxx",
         )
 
     def test_invoice_list(self, request_mock):
         stripe.Invoice.list(limit=3)
-        request_mock.assert_requested("get", "/v1/invoices")
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoices",
+        )
 
     def test_invoice_create(self, request_mock):
         stripe.Invoice.create(customer="cus_xxxxxxxxxxxxx")
-        request_mock.assert_requested("post", "/v1/invoices")
+        request_mock.assert_requested(
+            "post",
+            "/v1/invoices",
+        )
 
     def test_invoice_delete(self, request_mock):
         stripe.Invoice.delete("in_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/invoices/in_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/invoices/in_xxxxxxxxxxxxx",
         )
 
     def test_invoice_retrieve(self, request_mock):
         stripe.Invoice.retrieve("in_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/invoices/in_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoices/in_xxxxxxxxxxxxx",
+        )
 
     def test_invoice_retrieve2(self, request_mock):
-        stripe.Invoice.retrieve("in_xxxxxxxxxxxxx", expand=["customer"])
-        request_mock.assert_requested("get", "/v1/invoices/in_xxxxxxxxxxxxx")
+        stripe.Invoice.retrieve(
+            "in_xxxxxxxxxxxxx",
+            expand=["customer"],
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoices/in_xxxxxxxxxxxxx",
+        )
 
     def test_invoice_update(self, request_mock):
         stripe.Invoice.modify(
-            "in_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "in_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/invoices/in_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/invoices/in_xxxxxxxxxxxxx")
 
     def test_invoice_finalize_invoice(self, request_mock):
         stripe.Invoice.finalize_invoice("in_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/invoices/in_xxxxxxxxxxxxx/finalize",
         )
@@ -1053,38 +1321,47 @@
             "post",
             "/v1/invoices/in_xxxxxxxxxxxxx/mark_uncollectible",
         )
 
     def test_invoice_pay(self, request_mock):
         stripe.Invoice.pay("in_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/invoices/in_xxxxxxxxxxxxx/pay"
+            "post",
+            "/v1/invoices/in_xxxxxxxxxxxxx/pay",
         )
 
     def test_invoice_send_invoice(self, request_mock):
         stripe.Invoice.send_invoice("in_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/invoices/in_xxxxxxxxxxxxx/send"
+            "post",
+            "/v1/invoices/in_xxxxxxxxxxxxx/send",
         )
 
     def test_invoice_void_invoice(self, request_mock):
         stripe.Invoice.void_invoice("in_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/invoices/in_xxxxxxxxxxxxx/void"
+            "post",
+            "/v1/invoices/in_xxxxxxxxxxxxx/void",
         )
 
     def test_invoice_search(self, request_mock):
         stripe.Invoice.search(
             query="total>999 AND metadata['order_id']:'6735'"
         )
-        request_mock.assert_requested("get", "/v1/invoices/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/invoices/search",
+        )
 
     def test_issuing_authorization_list(self, request_mock):
         stripe.issuing.Authorization.list(limit=3)
-        request_mock.assert_requested("get", "/v1/issuing/authorizations")
+        request_mock.assert_requested(
+            "get",
+            "/v1/issuing/authorizations",
+        )
 
     def test_issuing_authorization_retrieve(self, request_mock):
         stripe.issuing.Authorization.retrieve("iauth_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/issuing/authorizations/iauth_xxxxxxxxxxxxx",
         )
@@ -1111,15 +1388,18 @@
         request_mock.assert_requested(
             "post",
             "/v1/issuing/authorizations/iauth_xxxxxxxxxxxxx/decline",
         )
 
     def test_issuing_cardholder_list(self, request_mock):
         stripe.issuing.Cardholder.list(limit=3)
-        request_mock.assert_requested("get", "/v1/issuing/cardholders")
+        request_mock.assert_requested(
+            "get",
+            "/v1/issuing/cardholders",
+        )
 
     def test_issuing_cardholder_create(self, request_mock):
         stripe.issuing.Cardholder.create(
             type="individual",
             name="Jenny Rosen",
             email="jenny.rosen@example.com",
             phone_number="+18888675309",
@@ -1129,15 +1409,18 @@
                     "city": "San Francisco",
                     "state": "CA",
                     "country": "US",
                     "postal_code": "94111",
                 },
             },
         )
-        request_mock.assert_requested("post", "/v1/issuing/cardholders")
+        request_mock.assert_requested(
+            "post",
+            "/v1/issuing/cardholders",
+        )
 
     def test_issuing_cardholder_retrieve(self, request_mock):
         stripe.issuing.Cardholder.retrieve("ich_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/issuing/cardholders/ich_xxxxxxxxxxxxx",
         )
@@ -1150,52 +1433,66 @@
         request_mock.assert_requested(
             "post",
             "/v1/issuing/cardholders/ich_xxxxxxxxxxxxx",
         )
 
     def test_issuing_card_list(self, request_mock):
         stripe.issuing.Card.list(limit=3)
-        request_mock.assert_requested("get", "/v1/issuing/cards")
+        request_mock.assert_requested(
+            "get",
+            "/v1/issuing/cards",
+        )
 
     def test_issuing_card_create(self, request_mock):
         stripe.issuing.Card.create(
             cardholder="ich_xxxxxxxxxxxxx",
             currency="usd",
             type="virtual",
         )
-        request_mock.assert_requested("post", "/v1/issuing/cards")
+        request_mock.assert_requested(
+            "post",
+            "/v1/issuing/cards",
+        )
 
     def test_issuing_card_retrieve(self, request_mock):
         stripe.issuing.Card.retrieve("ic_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/issuing/cards/ic_xxxxxxxxxxxxx"
+            "get",
+            "/v1/issuing/cards/ic_xxxxxxxxxxxxx",
         )
 
     def test_issuing_card_update(self, request_mock):
         stripe.issuing.Card.modify(
             "ic_xxxxxxxxxxxxx",
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/issuing/cards/ic_xxxxxxxxxxxxx"
+            "post",
+            "/v1/issuing/cards/ic_xxxxxxxxxxxxx",
         )
 
     def test_issuing_dispute_list(self, request_mock):
         stripe.issuing.Dispute.list(limit=3)
-        request_mock.assert_requested("get", "/v1/issuing/disputes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/issuing/disputes",
+        )
 
     def test_issuing_dispute_create(self, request_mock):
         stripe.issuing.Dispute.create(
             transaction="ipi_xxxxxxxxxxxxx",
             evidence={
                 "reason": "fraudulent",
                 "fraudulent": {"explanation": "Purchase was unrecognized."},
             },
         )
-        request_mock.assert_requested("post", "/v1/issuing/disputes")
+        request_mock.assert_requested(
+            "post",
+            "/v1/issuing/disputes",
+        )
 
     def test_issuing_dispute_retrieve(self, request_mock):
         stripe.issuing.Dispute.retrieve("idp_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/issuing/disputes/idp_xxxxxxxxxxxxx",
         )
@@ -1205,15 +1502,18 @@
         request_mock.assert_requested(
             "post",
             "/v1/issuing/disputes/idp_xxxxxxxxxxxxx/submit",
         )
 
     def test_issuing_transaction_list(self, request_mock):
         stripe.issuing.Transaction.list(limit=3)
-        request_mock.assert_requested("get", "/v1/issuing/transactions")
+        request_mock.assert_requested(
+            "get",
+            "/v1/issuing/transactions",
+        )
 
     def test_issuing_transaction_retrieve(self, request_mock):
         stripe.issuing.Transaction.retrieve("ipi_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/issuing/transactions/ipi_xxxxxxxxxxxxx",
         )
@@ -1227,33 +1527,41 @@
             "post",
             "/v1/issuing/transactions/ipi_xxxxxxxxxxxxx",
         )
 
     def test_mandate_retrieve(self, request_mock):
         stripe.Mandate.retrieve("mandate_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/mandates/mandate_xxxxxxxxxxxxx"
+            "get",
+            "/v1/mandates/mandate_xxxxxxxxxxxxx",
         )
 
     def test_paymentintent_list(self, request_mock):
         stripe.PaymentIntent.list(limit=3)
-        request_mock.assert_requested("get", "/v1/payment_intents")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payment_intents",
+        )
 
     def test_paymentintent_create2(self, request_mock):
         stripe.PaymentIntent.create(
             amount=2000,
             currency="usd",
             automatic_payment_methods={"enabled": True},
         )
-        request_mock.assert_requested("post", "/v1/payment_intents")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_intents",
+        )
 
     def test_paymentintent_retrieve(self, request_mock):
         stripe.PaymentIntent.retrieve("pi_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/payment_intents/pi_xxxxxxxxxxxxx"
+            "get",
+            "/v1/payment_intents/pi_xxxxxxxxxxxxx",
         )
 
     def test_paymentintent_update(self, request_mock):
         stripe.PaymentIntent.modify(
             "pi_xxxxxxxxxxxxx",
             metadata={"order_id": "6735"},
         )
@@ -1313,60 +1621,82 @@
             "/v1/payment_intents/pi_xxxxxxxxxxxxx/verify_microdeposits",
         )
 
     def test_paymentintent_search(self, request_mock):
         stripe.PaymentIntent.search(
             query="status:'succeeded' AND metadata['order_id']:'6735'",
         )
-        request_mock.assert_requested("get", "/v1/payment_intents/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payment_intents/search",
+        )
 
     def test_paymentlink_list(self, request_mock):
         stripe.PaymentLink.list(limit=3)
-        request_mock.assert_requested("get", "/v1/payment_links")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payment_links",
+        )
 
     def test_paymentlink_create2(self, request_mock):
         stripe.PaymentLink.create(
             line_items=[{"price": "price_xxxxxxxxxxxxx", "quantity": 1}],
         )
-        request_mock.assert_requested("post", "/v1/payment_links")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_links",
+        )
 
     def test_paymentlink_retrieve2(self, request_mock):
         stripe.PaymentLink.retrieve("plink_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/payment_links/plink_xxxxxxxxxxxxx",
         )
 
     def test_paymentlink_update(self, request_mock):
-        stripe.PaymentLink.modify("plink_xxxxxxxxxxxxx", active=False)
+        stripe.PaymentLink.modify(
+            "plink_xxxxxxxxxxxxx",
+            active=False,
+        )
         request_mock.assert_requested(
             "post",
             "/v1/payment_links/plink_xxxxxxxxxxxxx",
         )
 
     def test_paymentmethod_list(self, request_mock):
-        stripe.PaymentMethod.list(customer="cus_xxxxxxxxxxxxx", type="card")
-        request_mock.assert_requested("get", "/v1/payment_methods")
+        stripe.PaymentMethod.list(
+            customer="cus_xxxxxxxxxxxxx",
+            type="card",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/payment_methods",
+        )
 
     def test_paymentmethod_create(self, request_mock):
         stripe.PaymentMethod.create(
             type="card",
             card={
                 "number": "4242424242424242",
                 "exp_month": 8,
                 "exp_year": 2024,
                 "cvc": "314",
             },
         )
-        request_mock.assert_requested("post", "/v1/payment_methods")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_methods",
+        )
 
     def test_paymentmethod_retrieve(self, request_mock):
         stripe.PaymentMethod.retrieve("pm_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/payment_methods/pm_xxxxxxxxxxxxx"
+            "get",
+            "/v1/payment_methods/pm_xxxxxxxxxxxxx",
         )
 
     def test_paymentmethod_update(self, request_mock):
         stripe.PaymentMethod.modify(
             "pm_xxxxxxxxxxxxx",
             metadata={"order_id": "6735"},
         )
@@ -1390,138 +1720,220 @@
         request_mock.assert_requested(
             "post",
             "/v1/payment_methods/pm_xxxxxxxxxxxxx/detach",
         )
 
     def test_payout_list(self, request_mock):
         stripe.Payout.list(limit=3)
-        request_mock.assert_requested("get", "/v1/payouts")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payouts",
+        )
 
     def test_payout_create(self, request_mock):
-        stripe.Payout.create(amount=1100, currency="usd")
-        request_mock.assert_requested("post", "/v1/payouts")
+        stripe.Payout.create(
+            amount=1100,
+            currency="usd",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/payouts",
+        )
 
     def test_payout_retrieve(self, request_mock):
         stripe.Payout.retrieve("po_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/payouts/po_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/payouts/po_xxxxxxxxxxxxx",
+        )
 
     def test_payout_update(self, request_mock):
-        stripe.Payout.modify("po_xxxxxxxxxxxxx", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/payouts/po_xxxxxxxxxxxxx")
+        stripe.Payout.modify(
+            "po_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/payouts/po_xxxxxxxxxxxxx",
+        )
 
     def test_payout_cancel(self, request_mock):
         stripe.Payout.cancel("po_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/payouts/po_xxxxxxxxxxxxx/cancel"
+            "post",
+            "/v1/payouts/po_xxxxxxxxxxxxx/cancel",
         )
 
     def test_payout_reverse(self, request_mock):
         stripe.Payout.reverse("po_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/payouts/po_xxxxxxxxxxxxx/reverse",
         )
 
     def test_plan_list(self, request_mock):
         stripe.Plan.list(limit=3)
-        request_mock.assert_requested("get", "/v1/plans")
+        request_mock.assert_requested(
+            "get",
+            "/v1/plans",
+        )
 
     def test_plan_create(self, request_mock):
         stripe.Plan.create(
             amount=2000,
             currency="usd",
             interval="month",
             product="prod_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/plans")
+        request_mock.assert_requested(
+            "post",
+            "/v1/plans",
+        )
+
+    def test_plan_create2(self, request_mock):
+        stripe.Plan.create(
+            amount=2000,
+            currency="usd",
+            interval="month",
+            product={"name": "My product"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/plans",
+        )
 
     def test_plan_delete(self, request_mock):
         stripe.Plan.delete("price_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/plans/price_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/plans/price_xxxxxxxxxxxxx",
         )
 
     def test_plan_retrieve(self, request_mock):
         stripe.Plan.retrieve("price_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/plans/price_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/plans/price_xxxxxxxxxxxxx",
+        )
 
     def test_plan_update(self, request_mock):
         stripe.Plan.modify(
-            "price_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "price_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/plans/price_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/plans/price_xxxxxxxxxxxxx")
 
     def test_price_list(self, request_mock):
         stripe.Price.list(limit=3)
-        request_mock.assert_requested("get", "/v1/prices")
+        request_mock.assert_requested(
+            "get",
+            "/v1/prices",
+        )
 
     def test_price_create2(self, request_mock):
         stripe.Price.create(
             unit_amount=2000,
             currency="usd",
             recurring={"interval": "month"},
             product="prod_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/prices")
+        request_mock.assert_requested(
+            "post",
+            "/v1/prices",
+        )
 
     def test_price_retrieve(self, request_mock):
         stripe.Price.retrieve("price_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/prices/price_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/prices/price_xxxxxxxxxxxxx",
+        )
 
     def test_price_update(self, request_mock):
         stripe.Price.modify(
-            "price_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "price_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/prices/price_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/prices/price_xxxxxxxxxxxxx")
 
     def test_price_search(self, request_mock):
         stripe.Price.search(
             query="active:'true' AND metadata['order_id']:'6735'"
         )
-        request_mock.assert_requested("get", "/v1/prices/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/prices/search",
+        )
 
     def test_product_list(self, request_mock):
         stripe.Product.list(limit=3)
-        request_mock.assert_requested("get", "/v1/products")
+        request_mock.assert_requested(
+            "get",
+            "/v1/products",
+        )
 
     def test_product_create(self, request_mock):
         stripe.Product.create(name="Gold Special")
-        request_mock.assert_requested("post", "/v1/products")
+        request_mock.assert_requested(
+            "post",
+            "/v1/products",
+        )
 
     def test_product_delete(self, request_mock):
         stripe.Product.delete("prod_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "delete", "/v1/products/prod_xxxxxxxxxxxxx"
+            "delete",
+            "/v1/products/prod_xxxxxxxxxxxxx",
         )
 
     def test_product_retrieve(self, request_mock):
         stripe.Product.retrieve("prod_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/products/prod_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/products/prod_xxxxxxxxxxxxx",
+        )
 
     def test_product_update(self, request_mock):
         stripe.Product.modify(
-            "prod_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "prod_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/products/prod_xxxxxxxxxxxxx"
+            "post",
+            "/v1/products/prod_xxxxxxxxxxxxx",
         )
 
     def test_product_search(self, request_mock):
         stripe.Product.search(
             query="active:'true' AND metadata['order_id']:'6735'"
         )
-        request_mock.assert_requested("get", "/v1/products/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/products/search",
+        )
 
     def test_promotioncode_list(self, request_mock):
         stripe.PromotionCode.list(limit=3)
-        request_mock.assert_requested("get", "/v1/promotion_codes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/promotion_codes",
+        )
 
     def test_promotioncode_create(self, request_mock):
         stripe.PromotionCode.create(coupon="Z4OV52SU")
-        request_mock.assert_requested("post", "/v1/promotion_codes")
+        request_mock.assert_requested(
+            "post",
+            "/v1/promotion_codes",
+        )
 
     def test_promotioncode_retrieve(self, request_mock):
         stripe.PromotionCode.retrieve("promo_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/promotion_codes/promo_xxxxxxxxxxxxx",
         )
@@ -1534,73 +1946,100 @@
         request_mock.assert_requested(
             "post",
             "/v1/promotion_codes/promo_xxxxxxxxxxxxx",
         )
 
     def test_quote_list(self, request_mock):
         stripe.Quote.list(limit=3)
-        request_mock.assert_requested("get", "/v1/quotes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/quotes",
+        )
 
     def test_quote_create(self, request_mock):
         stripe.Quote.create(
             customer="cus_xxxxxxxxxxxxx",
             line_items=[{"price": "price_xxxxxxxxxxxxx", "quantity": 2}],
         )
-        request_mock.assert_requested("post", "/v1/quotes")
+        request_mock.assert_requested(
+            "post",
+            "/v1/quotes",
+        )
 
     def test_quote_retrieve(self, request_mock):
         stripe.Quote.retrieve("qt_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/quotes/qt_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/quotes/qt_xxxxxxxxxxxxx",
+        )
 
     def test_quote_update(self, request_mock):
-        stripe.Quote.modify("qt_xxxxxxxxxxxxx", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/quotes/qt_xxxxxxxxxxxxx")
+        stripe.Quote.modify(
+            "qt_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/quotes/qt_xxxxxxxxxxxxx",
+        )
 
     def test_quote_accept(self, request_mock):
         stripe.Quote.accept("qt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/quotes/qt_xxxxxxxxxxxxx/accept"
+            "post",
+            "/v1/quotes/qt_xxxxxxxxxxxxx/accept",
         )
 
     def test_quote_cancel(self, request_mock):
         stripe.Quote.cancel("qt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/quotes/qt_xxxxxxxxxxxxx/cancel"
+            "post",
+            "/v1/quotes/qt_xxxxxxxxxxxxx/cancel",
         )
 
     def test_quote_finalize_quote(self, request_mock):
         stripe.Quote.finalize_quote("qt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/quotes/qt_xxxxxxxxxxxxx/finalize",
         )
 
     def test_radar_earlyfraudwarning_list(self, request_mock):
         stripe.radar.EarlyFraudWarning.list(limit=3)
-        request_mock.assert_requested("get", "/v1/radar/early_fraud_warnings")
+        request_mock.assert_requested(
+            "get",
+            "/v1/radar/early_fraud_warnings",
+        )
 
     def test_radar_earlyfraudwarning_retrieve(self, request_mock):
         stripe.radar.EarlyFraudWarning.retrieve("issfr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/radar/early_fraud_warnings/issfr_xxxxxxxxxxxxx",
         )
 
     def test_radar_valuelistitem_list(self, request_mock):
         stripe.radar.ValueListItem.list(
-            limit=3, value_list="rsl_xxxxxxxxxxxxx"
+            limit=3,
+            value_list="rsl_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/radar/value_list_items",
         )
-        request_mock.assert_requested("get", "/v1/radar/value_list_items")
 
     def test_radar_valuelistitem_create(self, request_mock):
         stripe.radar.ValueListItem.create(
             value_list="rsl_xxxxxxxxxxxxx",
             value="1.2.3.4",
         )
-        request_mock.assert_requested("post", "/v1/radar/value_list_items")
+        request_mock.assert_requested(
+            "post",
+            "/v1/radar/value_list_items",
+        )
 
     def test_radar_valuelistitem_delete(self, request_mock):
         stripe.radar.ValueListItem.delete("rsli_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/radar/value_list_items/rsli_xxxxxxxxxxxxx",
         )
@@ -1610,23 +2049,29 @@
         request_mock.assert_requested(
             "get",
             "/v1/radar/value_list_items/rsli_xxxxxxxxxxxxx",
         )
 
     def test_radar_valuelist_list(self, request_mock):
         stripe.radar.ValueList.list(limit=3)
-        request_mock.assert_requested("get", "/v1/radar/value_lists")
+        request_mock.assert_requested(
+            "get",
+            "/v1/radar/value_lists",
+        )
 
     def test_radar_valuelist_create(self, request_mock):
         stripe.radar.ValueList.create(
             alias="custom_ip_xxxxxxxxxxxxx",
             name="Custom IP Blocklist",
             item_type="ip_address",
         )
-        request_mock.assert_requested("post", "/v1/radar/value_lists")
+        request_mock.assert_requested(
+            "post",
+            "/v1/radar/value_lists",
+        )
 
     def test_radar_valuelist_delete(self, request_mock):
         stripe.radar.ValueList.delete("rsl_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/radar/value_lists/rsl_xxxxxxxxxxxxx",
         )
@@ -1646,93 +2091,131 @@
         request_mock.assert_requested(
             "post",
             "/v1/radar/value_lists/rsl_xxxxxxxxxxxxx",
         )
 
     def test_refund_list(self, request_mock):
         stripe.Refund.list(limit=3)
-        request_mock.assert_requested("get", "/v1/refunds")
+        request_mock.assert_requested(
+            "get",
+            "/v1/refunds",
+        )
 
     def test_refund_create(self, request_mock):
         stripe.Refund.create(charge="ch_xxxxxxxxxxxxx")
-        request_mock.assert_requested("post", "/v1/refunds")
+        request_mock.assert_requested(
+            "post",
+            "/v1/refunds",
+        )
 
     def test_refund_retrieve(self, request_mock):
         stripe.Refund.retrieve("re_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/refunds/re_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/refunds/re_xxxxxxxxxxxxx",
+        )
 
     def test_refund_update(self, request_mock):
-        stripe.Refund.modify("re_xxxxxxxxxxxxx", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/refunds/re_xxxxxxxxxxxxx")
+        stripe.Refund.modify(
+            "re_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/refunds/re_xxxxxxxxxxxxx",
+        )
 
     def test_refund_cancel(self, request_mock):
         stripe.Refund.cancel("re_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/refunds/re_xxxxxxxxxxxxx/cancel"
+            "post",
+            "/v1/refunds/re_xxxxxxxxxxxxx/cancel",
         )
 
     def test_reporting_reportrun_list(self, request_mock):
         stripe.reporting.ReportRun.list(limit=3)
-        request_mock.assert_requested("get", "/v1/reporting/report_runs")
+        request_mock.assert_requested(
+            "get",
+            "/v1/reporting/report_runs",
+        )
 
     def test_reporting_reportrun_create(self, request_mock):
         stripe.reporting.ReportRun.create(
             report_type="balance.summary.1",
             parameters={
                 "interval_start": 1522540800,
                 "interval_end": 1525132800,
             },
         )
-        request_mock.assert_requested("post", "/v1/reporting/report_runs")
+        request_mock.assert_requested(
+            "post",
+            "/v1/reporting/report_runs",
+        )
 
     def test_reporting_reportrun_retrieve(self, request_mock):
         stripe.reporting.ReportRun.retrieve("frr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/reporting/report_runs/frr_xxxxxxxxxxxxx",
         )
 
     def test_reporting_reporttype_list(self, request_mock):
         stripe.reporting.ReportType.list()
-        request_mock.assert_requested("get", "/v1/reporting/report_types")
+        request_mock.assert_requested(
+            "get",
+            "/v1/reporting/report_types",
+        )
 
     def test_reporting_reporttype_retrieve(self, request_mock):
         stripe.reporting.ReportType.retrieve("balance.summary.1")
         request_mock.assert_requested(
             "get",
             "/v1/reporting/report_types/balance.summary.1",
         )
 
     def test_review_list(self, request_mock):
         stripe.Review.list(limit=3)
-        request_mock.assert_requested("get", "/v1/reviews")
+        request_mock.assert_requested(
+            "get",
+            "/v1/reviews",
+        )
 
     def test_review_retrieve(self, request_mock):
         stripe.Review.retrieve("prv_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/reviews/prv_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/reviews/prv_xxxxxxxxxxxxx",
+        )
 
     def test_review_approve(self, request_mock):
         stripe.Review.approve("prv_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/reviews/prv_xxxxxxxxxxxxx/approve",
         )
 
     def test_setupintent_list(self, request_mock):
         stripe.SetupIntent.list(limit=3)
-        request_mock.assert_requested("get", "/v1/setup_intents")
+        request_mock.assert_requested(
+            "get",
+            "/v1/setup_intents",
+        )
 
     def test_setupintent_create(self, request_mock):
         stripe.SetupIntent.create(payment_method_types=["card"])
-        request_mock.assert_requested("post", "/v1/setup_intents")
+        request_mock.assert_requested(
+            "post",
+            "/v1/setup_intents",
+        )
 
     def test_setupintent_retrieve(self, request_mock):
         stripe.SetupIntent.retrieve("seti_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/setup_intents/seti_xxxxxxxxxxxxx"
+            "get",
+            "/v1/setup_intents/seti_xxxxxxxxxxxxx",
         )
 
     def test_setupintent_update(self, request_mock):
         stripe.SetupIntent.modify(
             "seti_xxxxxxxxxxxxx",
             metadata={"user_id": "3435453"},
         )
@@ -1766,76 +2249,102 @@
         request_mock.assert_requested(
             "post",
             "/v1/setup_intents/seti_xxxxxxxxxxxxx/verify_microdeposits",
         )
 
     def test_shippingrate_list2(self, request_mock):
         stripe.ShippingRate.list(limit=3)
-        request_mock.assert_requested("get", "/v1/shipping_rates")
+        request_mock.assert_requested(
+            "get",
+            "/v1/shipping_rates",
+        )
 
     def test_shippingrate_create2(self, request_mock):
         stripe.ShippingRate.create(
             display_name="Ground shipping",
             type="fixed_amount",
             fixed_amount={"amount": 500, "currency": "usd"},
         )
-        request_mock.assert_requested("post", "/v1/shipping_rates")
+        request_mock.assert_requested(
+            "post",
+            "/v1/shipping_rates",
+        )
 
     def test_shippingrate_retrieve(self, request_mock):
         stripe.ShippingRate.retrieve("shr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/shipping_rates/shr_xxxxxxxxxxxxx"
+            "get",
+            "/v1/shipping_rates/shr_xxxxxxxxxxxxx",
         )
 
     def test_shippingrate_update(self, request_mock):
         stripe.ShippingRate.modify(
             "shr_xxxxxxxxxxxxx",
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
             "post",
             "/v1/shipping_rates/shr_xxxxxxxxxxxxx",
         )
 
     def test_sigma_scheduledqueryrun_list(self, request_mock):
         stripe.sigma.ScheduledQueryRun.list(limit=3)
-        request_mock.assert_requested("get", "/v1/sigma/scheduled_query_runs")
+        request_mock.assert_requested(
+            "get",
+            "/v1/sigma/scheduled_query_runs",
+        )
 
     def test_sigma_scheduledqueryrun_retrieve(self, request_mock):
         stripe.sigma.ScheduledQueryRun.retrieve("sqr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/sigma/scheduled_query_runs/sqr_xxxxxxxxxxxxx",
         )
 
     def test_source_retrieve(self, request_mock):
         stripe.Source.retrieve("src_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/sources/src_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/sources/src_xxxxxxxxxxxxx",
+        )
 
     def test_source_retrieve2(self, request_mock):
         stripe.Source.retrieve("src_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/sources/src_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/sources/src_xxxxxxxxxxxxx",
+        )
 
     def test_source_update(self, request_mock):
         stripe.Source.modify(
-            "src_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "src_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/sources/src_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/sources/src_xxxxxxxxxxxxx")
 
     def test_subscriptionitem_list(self, request_mock):
         stripe.SubscriptionItem.list(subscription="sub_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/subscription_items")
+        request_mock.assert_requested(
+            "get",
+            "/v1/subscription_items",
+        )
 
     def test_subscriptionitem_create(self, request_mock):
         stripe.SubscriptionItem.create(
             subscription="sub_xxxxxxxxxxxxx",
             price="price_xxxxxxxxxxxxx",
             quantity=2,
         )
-        request_mock.assert_requested("post", "/v1/subscription_items")
+        request_mock.assert_requested(
+            "post",
+            "/v1/subscription_items",
+        )
 
     def test_subscriptionitem_delete(self, request_mock):
         stripe.SubscriptionItem.delete("si_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/subscription_items/si_xxxxxxxxxxxxx",
         )
@@ -1855,29 +2364,35 @@
         request_mock.assert_requested(
             "post",
             "/v1/subscription_items/si_xxxxxxxxxxxxx",
         )
 
     def test_subscriptionschedule_list(self, request_mock):
         stripe.SubscriptionSchedule.list(limit=3)
-        request_mock.assert_requested("get", "/v1/subscription_schedules")
+        request_mock.assert_requested(
+            "get",
+            "/v1/subscription_schedules",
+        )
 
     def test_subscriptionschedule_create(self, request_mock):
         stripe.SubscriptionSchedule.create(
             customer="cus_xxxxxxxxxxxxx",
             start_date=1676070661,
             end_behavior="release",
             phases=[
                 {
                     "items": [{"price": "price_xxxxxxxxxxxxx", "quantity": 1}],
                     "iterations": 12,
                 },
             ],
         )
-        request_mock.assert_requested("post", "/v1/subscription_schedules")
+        request_mock.assert_requested(
+            "post",
+            "/v1/subscription_schedules",
+        )
 
     def test_subscriptionschedule_retrieve(self, request_mock):
         stripe.SubscriptionSchedule.retrieve("sub_sched_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/subscription_schedules/sub_sched_xxxxxxxxxxxxx",
         )
@@ -1904,87 +2419,121 @@
         request_mock.assert_requested(
             "post",
             "/v1/subscription_schedules/sub_sched_xxxxxxxxxxxxx/release",
         )
 
     def test_subscription_list(self, request_mock):
         stripe.Subscription.list(limit=3)
-        request_mock.assert_requested("get", "/v1/subscriptions")
+        request_mock.assert_requested(
+            "get",
+            "/v1/subscriptions",
+        )
 
     def test_subscription_create(self, request_mock):
         stripe.Subscription.create(
             customer="cus_xxxxxxxxxxxxx",
             items=[{"price": "price_xxxxxxxxxxxxx"}],
         )
-        request_mock.assert_requested("post", "/v1/subscriptions")
+        request_mock.assert_requested(
+            "post",
+            "/v1/subscriptions",
+        )
 
     def test_subscription_retrieve(self, request_mock):
         stripe.Subscription.retrieve("sub_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/subscriptions/sub_xxxxxxxxxxxxx"
+            "get",
+            "/v1/subscriptions/sub_xxxxxxxxxxxxx",
         )
 
     def test_subscription_update(self, request_mock):
         stripe.Subscription.modify(
             "sub_xxxxxxxxxxxxx",
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
-            "post", "/v1/subscriptions/sub_xxxxxxxxxxxxx"
+            "post",
+            "/v1/subscriptions/sub_xxxxxxxxxxxxx",
         )
 
     def test_subscription_search(self, request_mock):
         stripe.Subscription.search(
             query="status:'active' AND metadata['order_id']:'6735'",
         )
-        request_mock.assert_requested("get", "/v1/subscriptions/search")
+        request_mock.assert_requested(
+            "get",
+            "/v1/subscriptions/search",
+        )
 
     def test_taxcode_list(self, request_mock):
         stripe.TaxCode.list(limit=3)
-        request_mock.assert_requested("get", "/v1/tax_codes")
+        request_mock.assert_requested(
+            "get",
+            "/v1/tax_codes",
+        )
 
     def test_taxcode_retrieve(self, request_mock):
         stripe.TaxCode.retrieve("txcd_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "get", "/v1/tax_codes/txcd_xxxxxxxxxxxxx"
+            "get",
+            "/v1/tax_codes/txcd_xxxxxxxxxxxxx",
         )
 
     def test_taxrate_list(self, request_mock):
         stripe.TaxRate.list(limit=3)
-        request_mock.assert_requested("get", "/v1/tax_rates")
+        request_mock.assert_requested(
+            "get",
+            "/v1/tax_rates",
+        )
 
     def test_taxrate_create(self, request_mock):
         stripe.TaxRate.create(
             display_name="VAT",
             description="VAT Germany",
             jurisdiction="DE",
             percentage=16,
             inclusive=False,
         )
-        request_mock.assert_requested("post", "/v1/tax_rates")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tax_rates",
+        )
 
     def test_taxrate_retrieve(self, request_mock):
         stripe.TaxRate.retrieve("txr_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/tax_rates/txr_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/tax_rates/txr_xxxxxxxxxxxxx",
+        )
 
     def test_taxrate_update(self, request_mock):
-        stripe.TaxRate.modify("txr_xxxxxxxxxxxxx", active=False)
+        stripe.TaxRate.modify(
+            "txr_xxxxxxxxxxxxx",
+            active=False,
+        )
         request_mock.assert_requested(
-            "post", "/v1/tax_rates/txr_xxxxxxxxxxxxx"
+            "post",
+            "/v1/tax_rates/txr_xxxxxxxxxxxxx",
         )
 
     def test_terminal_configuration_list2(self, request_mock):
         stripe.terminal.Configuration.list(limit=3)
-        request_mock.assert_requested("get", "/v1/terminal/configurations")
+        request_mock.assert_requested(
+            "get",
+            "/v1/terminal/configurations",
+        )
 
     def test_terminal_configuration_create2(self, request_mock):
         stripe.terminal.Configuration.create(
             bbpos_wisepos_e={"splashscreen": "file_xxxxxxxxxxxxx"},
         )
-        request_mock.assert_requested("post", "/v1/terminal/configurations")
+        request_mock.assert_requested(
+            "post",
+            "/v1/terminal/configurations",
+        )
 
     def test_terminal_configuration_delete2(self, request_mock):
         stripe.terminal.Configuration.delete("tmc_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/terminal/configurations/tmc_xxxxxxxxxxxxx",
         )
@@ -2004,32 +2553,41 @@
         request_mock.assert_requested(
             "post",
             "/v1/terminal/configurations/tmc_xxxxxxxxxxxxx",
         )
 
     def test_terminal_connectiontoken_create(self, request_mock):
         stripe.terminal.ConnectionToken.create()
-        request_mock.assert_requested("post", "/v1/terminal/connection_tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/terminal/connection_tokens",
+        )
 
     def test_terminal_location_list(self, request_mock):
         stripe.terminal.Location.list(limit=3)
-        request_mock.assert_requested("get", "/v1/terminal/locations")
+        request_mock.assert_requested(
+            "get",
+            "/v1/terminal/locations",
+        )
 
     def test_terminal_location_create(self, request_mock):
         stripe.terminal.Location.create(
             display_name="My First Store",
             address={
                 "line1": "1234 Main Street",
                 "city": "San Francisco",
                 "postal_code": "94111",
                 "state": "CA",
                 "country": "US",
             },
         )
-        request_mock.assert_requested("post", "/v1/terminal/locations")
+        request_mock.assert_requested(
+            "post",
+            "/v1/terminal/locations",
+        )
 
     def test_terminal_location_delete(self, request_mock):
         stripe.terminal.Location.delete("tml_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/terminal/locations/tml_xxxxxxxxxxxxx",
         )
@@ -2049,23 +2607,29 @@
         request_mock.assert_requested(
             "post",
             "/v1/terminal/locations/tml_xxxxxxxxxxxxx",
         )
 
     def test_terminal_reader_list(self, request_mock):
         stripe.terminal.Reader.list(limit=3)
-        request_mock.assert_requested("get", "/v1/terminal/readers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/terminal/readers",
+        )
 
     def test_terminal_reader_create(self, request_mock):
         stripe.terminal.Reader.create(
             registration_code="puppies-plug-could",
             label="Blue Rabbit",
             location="tml_1234",
         )
-        request_mock.assert_requested("post", "/v1/terminal/readers")
+        request_mock.assert_requested(
+            "post",
+            "/v1/terminal/readers",
+        )
 
     def test_terminal_reader_delete(self, request_mock):
         stripe.terminal.Reader.delete("tmr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/terminal/readers/tmr_xxxxxxxxxxxxx",
         )
@@ -2074,15 +2638,18 @@
         stripe.terminal.Reader.retrieve("tmr_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/terminal/readers/tmr_xxxxxxxxxxxxx",
         )
 
     def test_terminal_reader_update(self, request_mock):
-        stripe.terminal.Reader.modify("tmr_xxxxxxxxxxxxx", label="Blue Rabbit")
+        stripe.terminal.Reader.modify(
+            "tmr_xxxxxxxxxxxxx",
+            label="Blue Rabbit",
+        )
         request_mock.assert_requested(
             "post",
             "/v1/terminal/readers/tmr_xxxxxxxxxxxxx",
         )
 
     def test_terminal_reader_cancel_action(self, request_mock):
         stripe.terminal.Reader.cancel_action("tmr_xxxxxxxxxxxxx")
@@ -2110,19 +2677,25 @@
         request_mock.assert_requested(
             "post",
             "/v1/terminal/readers/tmr_xxxxxxxxxxxxx/process_setup_intent",
         )
 
     def test_test_helpers_testclock_list2(self, request_mock):
         stripe.test_helpers.TestClock.list(limit=3)
-        request_mock.assert_requested("get", "/v1/test_helpers/test_clocks")
+        request_mock.assert_requested(
+            "get",
+            "/v1/test_helpers/test_clocks",
+        )
 
     def test_test_helpers_testclock_create2(self, request_mock):
         stripe.test_helpers.TestClock.create(frozen_time=1577836800)
-        request_mock.assert_requested("post", "/v1/test_helpers/test_clocks")
+        request_mock.assert_requested(
+            "post",
+            "/v1/test_helpers/test_clocks",
+        )
 
     def test_test_helpers_testclock_delete2(self, request_mock):
         stripe.test_helpers.TestClock.delete("clock_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/test_helpers/test_clocks/clock_xxxxxxxxxxxxx",
         )
@@ -2151,100 +2724,148 @@
                 "currency": "usd",
                 "account_holder_name": "Jenny Rosen",
                 "account_holder_type": "individual",
                 "routing_number": "110000000",
                 "account_number": "000123456789",
             },
         )
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_token_create3(self, request_mock):
         stripe.Token.create(pii={"id_number": "000000000"})
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_token_create4(self, request_mock):
         stripe.Token.create(
             account={
                 "individual": {"first_name": "Jane", "last_name": "Doe"},
                 "tos_shown_and_accepted": True,
             },
         )
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_token_create5(self, request_mock):
         stripe.Token.create(
             person={
                 "first_name": "Jane",
                 "last_name": "Doe",
                 "relationship": {"owner": True},
             },
         )
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_token_create6(self, request_mock):
         stripe.Token.create(cvc_update={"cvc": "123"})
-        request_mock.assert_requested("post", "/v1/tokens")
+        request_mock.assert_requested(
+            "post",
+            "/v1/tokens",
+        )
 
     def test_token_retrieve(self, request_mock):
         stripe.Token.retrieve("tok_xxxx")
-        request_mock.assert_requested("get", "/v1/tokens/tok_xxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/tokens/tok_xxxx",
+        )
 
     def test_topup_list(self, request_mock):
         stripe.Topup.list(limit=3)
-        request_mock.assert_requested("get", "/v1/topups")
+        request_mock.assert_requested(
+            "get",
+            "/v1/topups",
+        )
 
     def test_topup_create(self, request_mock):
         stripe.Topup.create(
             amount=2000,
             currency="usd",
             description="Top-up for Jenny Rosen",
             statement_descriptor="Top-up",
         )
-        request_mock.assert_requested("post", "/v1/topups")
+        request_mock.assert_requested(
+            "post",
+            "/v1/topups",
+        )
 
     def test_topup_retrieve(self, request_mock):
         stripe.Topup.retrieve("tu_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/topups/tu_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/topups/tu_xxxxxxxxxxxxx",
+        )
 
     def test_topup_update(self, request_mock):
-        stripe.Topup.modify("tu_xxxxxxxxxxxxx", metadata={"order_id": "6735"})
-        request_mock.assert_requested("post", "/v1/topups/tu_xxxxxxxxxxxxx")
+        stripe.Topup.modify(
+            "tu_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/topups/tu_xxxxxxxxxxxxx",
+        )
 
     def test_topup_cancel(self, request_mock):
         stripe.Topup.cancel("tu_xxxxxxxxxxxxx")
         request_mock.assert_requested(
-            "post", "/v1/topups/tu_xxxxxxxxxxxxx/cancel"
+            "post",
+            "/v1/topups/tu_xxxxxxxxxxxxx/cancel",
         )
 
     def test_transfer_list(self, request_mock):
         stripe.Transfer.list(limit=3)
-        request_mock.assert_requested("get", "/v1/transfers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/transfers",
+        )
 
     def test_transfer_create(self, request_mock):
         stripe.Transfer.create(
             amount=400,
             currency="usd",
             destination="acct_xxxxxxxxxxxxx",
             transfer_group="ORDER_95",
         )
-        request_mock.assert_requested("post", "/v1/transfers")
+        request_mock.assert_requested(
+            "post",
+            "/v1/transfers",
+        )
 
     def test_transfer_retrieve(self, request_mock):
         stripe.Transfer.retrieve("tr_xxxxxxxxxxxxx")
-        request_mock.assert_requested("get", "/v1/transfers/tr_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/transfers/tr_xxxxxxxxxxxxx",
+        )
 
     def test_transfer_update(self, request_mock):
         stripe.Transfer.modify(
-            "tr_xxxxxxxxxxxxx", metadata={"order_id": "6735"}
+            "tr_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/transfers/tr_xxxxxxxxxxxxx",
         )
-        request_mock.assert_requested("post", "/v1/transfers/tr_xxxxxxxxxxxxx")
 
     def test_transfer_transferreversal_retrieve(self, request_mock):
         stripe.Transfer.retrieve_reversal(
-            "tr_xxxxxxxxxxxxx", "trr_xxxxxxxxxxxxx"
+            "tr_xxxxxxxxxxxxx",
+            "trr_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
             "/v1/transfers/tr_xxxxxxxxxxxxx/reversals/trr_xxxxxxxxxxxxx",
         )
 
     def test_transfer_transferreversal_update(self, request_mock):
@@ -2259,58 +2880,74 @@
         )
 
     def test_treasury_creditreversal_list(self, request_mock):
         stripe.treasury.CreditReversal.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/credit_reversals")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/credit_reversals",
+        )
 
     def test_treasury_creditreversal_create(self, request_mock):
         stripe.treasury.CreditReversal.create(
             received_credit="rc_xxxxxxxxxxxxx"
         )
-        request_mock.assert_requested("post", "/v1/treasury/credit_reversals")
+        request_mock.assert_requested(
+            "post",
+            "/v1/treasury/credit_reversals",
+        )
 
     def test_treasury_creditreversal_retrieve(self, request_mock):
         stripe.treasury.CreditReversal.retrieve("credrev_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/credit_reversals/credrev_xxxxxxxxxxxxx",
         )
 
     def test_treasury_debitreversal_list(self, request_mock):
         stripe.treasury.DebitReversal.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/debit_reversals")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/debit_reversals",
+        )
 
     def test_treasury_debitreversal_create(self, request_mock):
         stripe.treasury.DebitReversal.create(received_debit="rd_xxxxxxxxxxxxx")
-        request_mock.assert_requested("post", "/v1/treasury/debit_reversals")
+        request_mock.assert_requested(
+            "post",
+            "/v1/treasury/debit_reversals",
+        )
 
     def test_treasury_debitreversal_retrieve(self, request_mock):
         stripe.treasury.DebitReversal.retrieve("debrev_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/debit_reversals/debrev_xxxxxxxxxxxxx",
         )
 
     def test_treasury_financialaccount_list(self, request_mock):
         stripe.treasury.FinancialAccount.list(limit=3)
-        request_mock.assert_requested("get", "/v1/treasury/financial_accounts")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/financial_accounts",
+        )
 
     def test_treasury_financialaccount_create(self, request_mock):
         stripe.treasury.FinancialAccount.create(
             supported_currencies=["usd"],
             features={},
         )
         request_mock.assert_requested(
-            "post", "/v1/treasury/financial_accounts"
+            "post",
+            "/v1/treasury/financial_accounts",
         )
 
     def test_treasury_financialaccount_retrieve(self, request_mock):
         stripe.treasury.FinancialAccount.retrieve("fa_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/financial_accounts/fa_xxxxxxxxxxxxx",
@@ -2334,25 +2971,31 @@
         )
 
     def test_treasury_inboundtransfer_list(self, request_mock):
         stripe.treasury.InboundTransfer.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/inbound_transfers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/inbound_transfers",
+        )
 
     def test_treasury_inboundtransfer_create(self, request_mock):
         stripe.treasury.InboundTransfer.create(
             financial_account="fa_xxxxxxxxxxxxx",
             amount=10000,
             currency="usd",
             origin_payment_method="pm_xxxxxxxxxxxxx",
             description="InboundTransfer from my bank account",
         )
-        request_mock.assert_requested("post", "/v1/treasury/inbound_transfers")
+        request_mock.assert_requested(
+            "post",
+            "/v1/treasury/inbound_transfers",
+        )
 
     def test_treasury_inboundtransfer_retrieve(self, request_mock):
         stripe.treasury.InboundTransfer.retrieve("ibt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/inbound_transfers/ibt_xxxxxxxxxxxxx",
         )
@@ -2365,26 +3008,32 @@
         )
 
     def test_treasury_outboundpayment_list(self, request_mock):
         stripe.treasury.OutboundPayment.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/outbound_payments")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/outbound_payments",
+        )
 
     def test_treasury_outboundpayment_create(self, request_mock):
         stripe.treasury.OutboundPayment.create(
             financial_account="fa_xxxxxxxxxxxxx",
             amount=10000,
             currency="usd",
             customer="cus_xxxxxxxxxxxxx",
             destination_payment_method="pm_xxxxxxxxxxxxx",
             description="OutboundPayment to a 3rd party",
         )
-        request_mock.assert_requested("post", "/v1/treasury/outbound_payments")
+        request_mock.assert_requested(
+            "post",
+            "/v1/treasury/outbound_payments",
+        )
 
     def test_treasury_outboundpayment_retrieve(self, request_mock):
         stripe.treasury.OutboundPayment.retrieve("bot_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/outbound_payments/bot_xxxxxxxxxxxxx",
         )
@@ -2397,26 +3046,30 @@
         )
 
     def test_treasury_outboundtransfer_list(self, request_mock):
         stripe.treasury.OutboundTransfer.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/outbound_transfers")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/outbound_transfers",
+        )
 
     def test_treasury_outboundtransfer_create(self, request_mock):
         stripe.treasury.OutboundTransfer.create(
             financial_account="fa_xxxxxxxxxxxxx",
             destination_payment_method="pm_xxxxxxxxxxxxx",
             amount=500,
             currency="usd",
             description="OutboundTransfer to my external bank account",
         )
         request_mock.assert_requested(
-            "post", "/v1/treasury/outbound_transfers"
+            "post",
+            "/v1/treasury/outbound_transfers",
         )
 
     def test_treasury_outboundtransfer_retrieve(self, request_mock):
         stripe.treasury.OutboundTransfer.retrieve("obt_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/outbound_transfers/obt_xxxxxxxxxxxxx",
@@ -2430,77 +3083,93 @@
         )
 
     def test_treasury_receivedcredit_list(self, request_mock):
         stripe.treasury.ReceivedCredit.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/received_credits")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/received_credits",
+        )
 
     def test_treasury_receivedcredit_retrieve(self, request_mock):
         stripe.treasury.ReceivedCredit.retrieve("rc_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/received_credits/rc_xxxxxxxxxxxxx",
         )
 
     def test_treasury_receiveddebit_list(self, request_mock):
         stripe.treasury.ReceivedDebit.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/received_debits")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/received_debits",
+        )
 
     def test_treasury_receiveddebit_retrieve(self, request_mock):
         stripe.treasury.ReceivedDebit.retrieve("rd_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/received_debits/rd_xxxxxxxxxxxxx",
         )
 
     def test_treasury_transactionentry_list(self, request_mock):
         stripe.treasury.TransactionEntry.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
         request_mock.assert_requested(
-            "get", "/v1/treasury/transaction_entries"
+            "get",
+            "/v1/treasury/transaction_entries",
         )
 
     def test_treasury_transactionentry_retrieve(self, request_mock):
         stripe.treasury.TransactionEntry.retrieve("trxne_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/transaction_entries/trxne_xxxxxxxxxxxxx",
         )
 
     def test_treasury_transaction_list(self, request_mock):
         stripe.treasury.Transaction.list(
             financial_account="fa_xxxxxxxxxxxxx",
             limit=3,
         )
-        request_mock.assert_requested("get", "/v1/treasury/transactions")
+        request_mock.assert_requested(
+            "get",
+            "/v1/treasury/transactions",
+        )
 
     def test_treasury_transaction_retrieve(self, request_mock):
         stripe.treasury.Transaction.retrieve("trxn_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/treasury/transactions/trxn_xxxxxxxxxxxxx",
         )
 
     def test_webhookendpoint_list(self, request_mock):
         stripe.WebhookEndpoint.list(limit=3)
-        request_mock.assert_requested("get", "/v1/webhook_endpoints")
+        request_mock.assert_requested(
+            "get",
+            "/v1/webhook_endpoints",
+        )
 
     def test_webhookendpoint_create(self, request_mock):
         stripe.WebhookEndpoint.create(
             url="https://example.com/my/webhook/endpoint",
             enabled_events=["charge.failed", "charge.succeeded"],
         )
-        request_mock.assert_requested("post", "/v1/webhook_endpoints")
+        request_mock.assert_requested(
+            "post",
+            "/v1/webhook_endpoints",
+        )
 
     def test_webhookendpoint_delete(self, request_mock):
         stripe.WebhookEndpoint.delete("we_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "delete",
             "/v1/webhook_endpoints/we_xxxxxxxxxxxxx",
         )
@@ -2531,24 +3200,38 @@
             "post",
             "/v1/tax/transactions/create_from_calculation",
         )
 
     def test_tax_calculation_list_line_items(self, request_mock):
         stripe.tax.Calculation.list_line_items("xxx")
         request_mock.assert_requested(
-            "get", "/v1/tax/calculations/xxx/line_items"
+            "get",
+            "/v1/tax/calculations/xxx/line_items",
         )
 
     def test_quote_preview_invoice_lines(self, request_mock):
-        stripe.Quote.preview_invoice_lines("qt_xyz", "in_xyz")
+        stripe.Quote.preview_invoice_lines(
+            "qt_xyz",
+            "in_xyz",
+        )
         request_mock.assert_requested(
             "get",
             "/v1/quotes/qt_xyz/preview_invoices/in_xyz/lines",
         )
 
     def test_paymentintent_create3(self, request_mock):
         stripe.PaymentIntent.create(
             amount=200,
             currency="usd",
             payment_method_data={"type": "p24", "p24": {"bank": "blik"}},
         )
-        request_mock.assert_requested("post", "/v1/payment_intents")
+        request_mock.assert_requested(
+            "post",
+            "/v1/payment_intents",
+        )
+
+    def test_quote_list_line_items(self, request_mock):
+        stripe.Quote.list_line_items("qt_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/quotes/qt_xxxxxxxxxxxxx/line_items",
+        )
```

### Comparing `stripe-5.5.0b2/tests/test_http_client.py` & `stripe-5.5.0b3/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_integration.py` & `stripe-5.5.0b3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_multipart_data_generator.py` & `stripe-5.5.0b3/tests/test_multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_oauth.py` & `stripe-5.5.0b3/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_stripe_object.py` & `stripe-5.5.0b3/tests/test_stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_stripe_response.py` & `stripe-5.5.0b3/tests/test_stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_util.py` & `stripe-5.5.0b3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tests/test_webhook.py` & `stripe-5.5.0b3/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b2/tox.ini` & `stripe-5.5.0b3/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -69,14 +69,11 @@
 skip_install = true
 setenv =
     COVERAGE_FILE = {toxworkdir}/.coverage
 passenv = GITHUB_*
 deps =
     coverage >= 4.5.3, < 5 # TODO: upgrade to coverage 5 when we drop support for Python 3.4
     coveralls
-    pytest
-    pytest-mock
 commands =
-    coverage run --source=stripe -m pytest tests/
     coverage combine
     coveralls --service=github
 depends = py{310,39,38,37,36,35,34,27,py3,py2}
```

