# Comparing `tmp/codat-accounting-0.5.1.tar.gz` & `tmp/codat-accounting-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-accounting-0.5.1.tar", last modified: Fri Mar 17 05:39:24 2023, max compression
+gzip compressed data, was "codat-accounting-0.9.6.tar", last modified: Wed Apr  5 09:30:27 2023, max compression
```

## Comparing `codat-accounting-0.5.1.tar` & `codat-accounting-0.9.6.tar`

### file list

```diff
@@ -1,177 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7700 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.678335 codat-accounting-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.682335 codat-accounting-0.5.1/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/account_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6291 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/bank_account_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9306 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/bank_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8457 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/bill_credit_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8041 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/bill_payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13533 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/bills.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2715 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/company_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8258 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/credit_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11172 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10431 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/direct_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10740 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/direct_incomes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4250 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/financials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12705 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/invoices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5929 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/items.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6366 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/journal_entries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6076 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/journals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.682335 codat-accounting-0.5.1/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)   140235 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23416 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17042 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_bank_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47920 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_bill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_bill_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48200 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_bill_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42732 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_bill_payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48257 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28180 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43051 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_direct_cost.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38519 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_direct_income.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50021 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_invoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24341 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26693 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_journal_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    69607 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37571 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_purchase_order.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19833 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_suppliers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22290 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/create_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8050 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/delete_companies_companyid_connections_connectionid_push_billpayments_billpaymentid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7827 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/delete_companies_companyid_connections_connectionid_push_bills_billid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      970 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/donwload_invoice_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/download_bill_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/download_customer_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/download_direct_cost_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/download_direct_income_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/download_supplier_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8902 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12054 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_aged_creditors_report.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5493 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_aged_debtors_report.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4489 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_all_bank_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8516 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_balance_sheet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5790 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bank_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21753 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bank_account_push_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20693 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3156 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bill_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bill_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20803 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bill_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18434 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_bill_payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8993 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_cash_flow_statement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_company_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21108 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_billpayments_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21282 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_chartofaccounts_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21050 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_directcosts_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21166 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_directincomes_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20702 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_items_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21224 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_journalentries_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20876 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_journals_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20876 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_payments_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20934 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_transfers_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8779 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_accounttransactions_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21456 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_bankaccounts_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21630 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_billcreditnotes_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21050 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_bills_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21398 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_creditnotes_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21282 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_customers_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21224 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_invoices_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21572 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_purchaseorders_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21282 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_create_update_suppliers_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20703 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11101 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_customer_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_customer_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14354 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18463 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_cost.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3193 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_cost_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21827 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16282 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_income.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_income_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19620 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_direct_incomes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21751 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_invoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3174 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_invoice_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3395 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_invoice_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_invoice_pdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9201 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6521 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_journal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10374 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_journal_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31868 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4265 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_payment_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10473 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_profit_and_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15671 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_purchase_order.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15398 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_sales_order.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7060 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_supplier_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9146 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_tax_rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9325 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_tracking_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8430 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/get_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/is_aged_creditors_report_available.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/is_aged_debtor_report_available.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11793 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_account_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8999 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bank_account_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8986 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bank_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7013 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bank_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24323 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bill_credit_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21708 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bill_payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24119 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_bills.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24180 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_credit_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3426 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_direct_cost_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3442 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_direct_income_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25196 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_invoices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12452 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_items.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13714 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_journal_entries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9686 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_journals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_payment_methods.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35124 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19076 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_purchase_orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18777 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_sales_orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_supplier_attachments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10264 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_suppliers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12172 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_tax_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7477 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_tracking_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11683 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/list_transfers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16557 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/post_bank_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/post_direct_cost_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/post_direct_income_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3937 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/post_sync_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47719 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/push_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/push_invoice_attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17572 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/push_journal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17058 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/put_bank_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19940 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/put_supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48207 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/update_bill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48509 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/update_bill_credit_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28475 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/update_customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50314 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/update_invoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37877 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/operations/update_purchase_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2883 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/payment_methods.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8295 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/purchase_orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/sales_orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10010 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11101 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/suppliers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2784 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/tax_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/tracking_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6061 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/transfers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24723 2023-03-17 05:39:16.000000 codat-accounting-0.5.1/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:24.698336 codat-accounting-0.5.1/src/codat_accounting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-03-17 05:39:24.000000 codat-accounting-0.5.1/src/codat_accounting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-17 05:39:24.000000 codat-accounting-0.5.1/src/codat_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 05:39:24.000000 codat-accounting-0.5.1/src/codat_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-17 05:39:24.000000 codat-accounting-0.5.1/src/codat_accounting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 05:39:24.000000 codat-accounting-0.5.1/src/codat_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.091824 codat-accounting-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-04-05 09:30:27.091824 codat-accounting-0.9.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7600 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:30:27.091824 codat-accounting-0.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.059825 codat-accounting-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.063825 codat-accounting-0.9.6/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3177 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/account_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6076 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6247 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/bank_account_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9200 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/bank_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8398 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/bill_credit_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7526 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/bill_payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13056 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/bills.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2731 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/company_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8194 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/credit_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11127 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10688 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/direct_costs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10999 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/direct_incomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4174 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/financials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13027 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/invoices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5877 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/items.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/journal_entries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6065 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/journals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.063825 codat-accounting-0.9.6/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.071824 codat-accounting-0.9.6/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12089 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_bank_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_bank_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_bill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_bill_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_bill_payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_direct_cost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_direct_income.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_invoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_journal_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1425 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_purchase_order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/create_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1143 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/delete_bill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/delete_billpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_bill_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_customer_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_direct_cost_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_direct_income_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1242 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_invoice_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_invoice_pdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1246 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/download_supplier_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_account_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_aged_creditors_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1504 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_aged_debtors_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_all_bank_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_balance_sheet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1120 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bank_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bill_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bill_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bill_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_bill_payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_cash_flow_statement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_company_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_bank_account_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_billpayments_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_chartofaccounts_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_directcosts_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      957 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_directincomes_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_items_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_journalentries_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_journals_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_payments_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_transfers_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_bankaccounts_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_billcreditnotes_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_bills_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_creditnotes_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_customers_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_invoices_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_purchaseorders_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_create_update_suppliers_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      935 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1274 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_customer_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_customer_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1123 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_cost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_cost_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_costs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_income.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1512 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_income_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_direct_incomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_invoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_invoice_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_invoice_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      906 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_journal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_journal_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      906 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_payment_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_profit_and_loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_purchase_order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      935 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_sales_order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_supplier_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      908 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_tax_rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_tracking_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/get_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/is_aged_creditors_report_available.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/is_aged_debtor_report_available.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_account_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bank_account_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1911 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bank_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bank_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1792 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bill_credit_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1770 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bill_payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1720 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_bills.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_credit_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_direct_cost_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_direct_income_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_invoices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1724 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_items.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_journal_entries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_journals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_payment_methods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_purchase_orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_sales_orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_supplier_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1748 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_suppliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1742 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_tax_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_tracking_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/list_transfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/post_sync_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8701 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/push_journal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7475 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/put_supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1755 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_bank_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1646 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_bill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_bill_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1693 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_credit_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1692 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_invoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1735 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/update_purchase_order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1422 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/upload_bill_attachments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1462 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/upload_direct_cost_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/upload_direct_income_attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/operations/upload_invoice_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.087824 codat-accounting-0.9.6/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9838 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7790 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accountref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accountstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10209 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accounttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accounttransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accounttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/accounttype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1899 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/addressesitems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/addresstype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5586 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/agedcreditor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5564 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/agedcreditorreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4596 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/agedcurrencyoutstandingitems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/ageddebtor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5535 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/ageddebtorreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5894 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/attachmentsdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/balancesheet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5019 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/balancesheet1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8531 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bankaccountref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bankaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bankaccounttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5050 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bankstatementaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5068 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/banktransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/banktransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1217 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/banktransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/banktransactiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14941 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12812 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billcreditnote.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5631 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billcreditnotelineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billcreditnotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      371 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billcreditnotestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billedtotype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billedtotype_enum1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4474 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billlineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18547 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1903 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billpaymentline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3170 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billpaymentlinelink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billpaymentlinelinktype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/bills.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      340 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/billstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2988 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/cashflowstatement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/cashflowstatement1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10077 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/companydataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2721 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/contactref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6709 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createaccountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6713 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createbankaccountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6457 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createbanktransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6858 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createbillcreditnoteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14948 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createbillpaymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6612 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createbillresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6396 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createcreditnoteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6168 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createcustomerresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createdirectcostresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6370 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createdirectincomeresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7380 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createinvoiceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5877 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createitemresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7250 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createjournalentryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28634 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createpaymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6168 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createpurchaseorderresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6059 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createsupplierresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6008 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/createtransferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12781 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/creditnote.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5816 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/creditnotelineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/creditnotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/creditnotestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7183 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/customerref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/customerstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4890 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/datatype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9582 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directcost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4331 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directcostlineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directcosts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9509 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directincome.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4212 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directincomelineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1190 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/directincomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/halref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16165 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1929 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoiceitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4621 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoicelineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoicestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/invoiceto.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5544 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      741 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/itemref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/items.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/items1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/itemstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7809 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1191 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journalentries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9868 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journalentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1767 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journalline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journalref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/journalstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/one.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32148 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5146 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentallocationpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1878 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentlinelink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      901 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentlinktype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4428 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentmethod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentmethodref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentmethods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentmethodstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/paymentmethodtype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/phonenumbersitems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/phonenumbertype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/profitandlossreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5119 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/profitandlossreport1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/projectref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/propertiestracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1627 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/propertiestracking1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      608 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/propertiestracking2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13387 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/purchaseorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4008 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/purchaseorderlineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/purchaseorderref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/purchaseorders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      325 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/purchaseorderstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushchangetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushfieldvalidation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoperationchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoperationref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoperationstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5274 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoperationsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoptionchoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoptionproperty.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushoptiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/pushvalidationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/reportbasis_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      310 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/reportinput_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1213 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/reportline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13551 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/salesorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/salesorderinvoicestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4179 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/salesorderlineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/salesorders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/salesorderstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/shipto.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      286 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/status_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/supplementaldata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6486 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      763 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/supplierref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/suppliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/supplierstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7064 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/taxrate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/taxratecomponent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/taxrateref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/taxrates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/taxratestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1611 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/tracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/trackingcategories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5530 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/trackingcategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/trackingcategoryref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4203 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/trackingcategorytree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7095 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/transferaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/transfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6440 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatebankaccountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6858 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatebillcreditnoteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6612 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatebillresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6396 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatecreditnoteresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6168 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatecustomerresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7380 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updateinvoiceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6168 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/updatepurchaseorderresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/validationitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/validdatatypelinks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/withholdingtaxitems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1421 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/models/shared/zero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/payment_methods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6007 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8227 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/purchase_orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5471 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/sales_orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10913 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11079 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/suppliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2805 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/tax_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3044 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/tracking_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6020 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/transfers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.091824 codat-accounting-0.9.6/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:30:15.000000 codat-accounting-0.9.6/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:27.091824 codat-accounting-0.9.6/src/codat_accounting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-04-05 09:30:26.000000 codat-accounting-0.9.6/src/codat_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15531 2023-04-05 09:30:27.000000 codat-accounting-0.9.6/src/codat_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:30:26.000000 codat-accounting-0.9.6/src/codat_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:30:26.000000 codat-accounting-0.9.6/src/codat_accounting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:30:26.000000 codat-accounting-0.9.6/src/codat_accounting.egg-info/top_level.txt
```

### Comparing `codat-accounting-0.5.1/PKG-INFO` & `codat-accounting-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-accounting
-Version: 0.5.1
+Version: 0.9.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,100 +28,100 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCreateUpdateAccountTransactionsModelRequest(
-    account_transaction_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+req = operations.GetAccountTransactionRequest(
+    account_transaction_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.account_transactions.get_create_update_account_transactions_model(req)
+res = s.account_transactions.get_account_transaction(req)
 
-if res.source_modified_date is not None:
+if res.account_transaction is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### account_transactions
 
-* `get_create_update_account_transactions_model` - Get account transaction
+* `get_account_transaction` - Get account transaction
 * `list_account_transactions` - List account transactions
 
 ### accounts
 
 * `create_account` - Create account
 * `get_account` - Get account
-* `get_accounts` - List accounts
 * `get_create_chart_of_accounts_model` - Get create account model
+* `list_accounts` - List accounts
 
 ### bank_account_transactions
 
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
 * `list_bank_transactions` - List all bank transactions
-* `post_bank_transactions` - Create bank transactions
 
 ### bank_accounts
 
 * `create_bank_account` - Create bank account
 * `get_all_bank_account` - Get bank account
 * `get_bank_account` - Get bank account
 * `get_create_update_bank_accounts_model` - Get create/update bank account model
 * `list_bank_accounts` - List bank accounts
-* `put_bank_account` - Update bank account
+* `update_bank_account` - Update bank account
 
 ### bill_credit_notes
 
 * `create_bill_credit_note` - Create bill credit note
 * `get_bill_credit_note` - Get bill credit note
 * `get_create_update_bill_credit_notes_model` - Get create/update bill credit note model
 * `list_bill_credit_notes` - List bill credit notes
 * `update_bill_credit_note` - Update bill credit note
 
 ### bill_payments
 
 * `create_bill_payment` - Create bill payments
-* `delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id` - Delete bill payment
+* `delete_bill_payment` - Delete bill payment
 * `get_bill_payments` - Get bill payment
 * `get_create_bill_payments_model` - Get create bill payment model
 * `list_bill_payments` - List bill payments
 
 ### bills
 
 * `create_bill` - Create bill
-* `create_bill_attachments` - Create bill attachments
-* `delete_companies_company_id_connections_connection_id_push_bills_bill_id` - Delete bill
+* `delete_bill` - Delete bill
 * `download_bill_attachment` - Download bill attachment
 * `get_bill` - Get bill
 * `get_bill_attachment` - Get bill attachment
 * `get_bill_attachments` - List bill attachments
 * `get_create_update_bills_model` - Get create/update bill model
 * `list_bills` - List bills
 * `update_bill` - Update bill
+* `upload_bill_attachments` - Upload bill attachments
 
 ### company_info
 
 * `get_company_info` - Get company info
 * `post_sync_info` - Refresh company info
 
 ### credit_notes
 
-* `create_credit_note` - Update creditNote
+* `create_credit_note` - Create credit note
 * `get_create_update_credit_notes_model` - Get create/update credit note model
 * `get_credit_note` - Get credit note
 * `list_credit_notes` - List credit notes
-* `push_credit_note` - Create credit note
+* `update_credit_note` - Update creditNote
 
 ### customers
 
 * `create_customer` - Create customer
 * `download_customer_attachment` - Download customer attachment
 * `get_create_update_customers_model` - Get create/update customer model
 * `get_customer` - Get customer
@@ -135,45 +135,45 @@
 * `create_direct_cost` - Create direct cost
 * `download_direct_cost_attachment` - Download direct cost attachment
 * `get_create_direct_costs_model` - Get create direct cost model
 * `get_direct_cost` - Get direct cost
 * `get_direct_cost_attachment` - Get direct cost attachment
 * `get_direct_costs` - List direct costs
 * `list_direct_cost_attachments` - List direct cost attachments
-* `post_direct_cost_attachment` - Create direct cost attachment
+* `upload_direct_cost_attachment` - Upload direct cost attachment
 
 ### direct_incomes
 
 * `create_direct_income` - Create direct income
 * `download_direct_income_attachment` - Download direct income attachment
 * `get_create_direct_incomes_model` - Get create direct income model
 * `get_direct_income` - Get direct income
 * `get_direct_income_attachment` - Get direct income attachment
 * `get_direct_incomes` - Get direct incomes
 * `list_direct_income_attachments` - List direct income attachments
-* `post_direct_income_attachment` - Create direct income attachment
+* `upload_direct_income_attachment` - Create direct income attachment
 
 ### financials
 
 * `get_balance_sheet` - Get balance sheet
 * `get_cash_flow_statement` - Get cash flow statement
 * `get_profit_and_loss` - Get profit and loss
 
 ### invoices
 
+* `download_invoice_pdf` - Get invoice as PDF
 * `create_invoice` - Create invoice
-* `donwload_invoice_attachment` - Download invoice attachment
+* `download_invoice_attachment` - Download invoice attachment
 * `get_create_update_invoices_model` - Get create/update invoice model
 * `get_invoice` - Get invoice
 * `get_invoice_attachment` - Get invoice attachment
 * `get_invoice_attachments` - Get invoice attachments
-* `get_invoice_pdf` - Get invoice as PDF
 * `list_invoices` - List invoices
-* `push_invoice_attachment` - Push invoice attachment
 * `update_invoice` - Update invoice
+* `upload_invoice_attachment` - Push invoice attachment
 
 ### items
 
 * `create_item` - Create item
 * `get_create_items_model` - Get create item model
 * `get_item` - Get item
 * `list_items` - List items
@@ -222,15 +222,15 @@
 ### sales_orders
 
 * `get_sales_order` - Get sales order
 * `list_sales_orders` - List sales orders
 
 ### suppliers
 
-* `create_suppliers` - Create suppliers
+* `create_supplier` - Create suppliers
 * `download_supplier_attachment` - Download supplier attachment
 * `get_create_update_suppliers_model` - Get create/update supplier model
 * `get_supplier` - Get supplier
 * `get_supplier_attachment` - Get supplier attachment
 * `list_supplier_attachments` - List supplier attachments
 * `list_suppliers` - List suppliers
 * `put_supplier` - Update supplier
```

### Comparing `codat-accounting-0.5.1/README.md` & `codat-accounting-0.9.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,100 +17,100 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCreateUpdateAccountTransactionsModelRequest(
-    account_transaction_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+req = operations.GetAccountTransactionRequest(
+    account_transaction_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.account_transactions.get_create_update_account_transactions_model(req)
+res = s.account_transactions.get_account_transaction(req)
 
-if res.source_modified_date is not None:
+if res.account_transaction is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### account_transactions
 
-* `get_create_update_account_transactions_model` - Get account transaction
+* `get_account_transaction` - Get account transaction
 * `list_account_transactions` - List account transactions
 
 ### accounts
 
 * `create_account` - Create account
 * `get_account` - Get account
-* `get_accounts` - List accounts
 * `get_create_chart_of_accounts_model` - Get create account model
+* `list_accounts` - List accounts
 
 ### bank_account_transactions
 
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
 * `list_bank_transactions` - List all bank transactions
-* `post_bank_transactions` - Create bank transactions
 
 ### bank_accounts
 
 * `create_bank_account` - Create bank account
 * `get_all_bank_account` - Get bank account
 * `get_bank_account` - Get bank account
 * `get_create_update_bank_accounts_model` - Get create/update bank account model
 * `list_bank_accounts` - List bank accounts
-* `put_bank_account` - Update bank account
+* `update_bank_account` - Update bank account
 
 ### bill_credit_notes
 
 * `create_bill_credit_note` - Create bill credit note
 * `get_bill_credit_note` - Get bill credit note
 * `get_create_update_bill_credit_notes_model` - Get create/update bill credit note model
 * `list_bill_credit_notes` - List bill credit notes
 * `update_bill_credit_note` - Update bill credit note
 
 ### bill_payments
 
 * `create_bill_payment` - Create bill payments
-* `delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id` - Delete bill payment
+* `delete_bill_payment` - Delete bill payment
 * `get_bill_payments` - Get bill payment
 * `get_create_bill_payments_model` - Get create bill payment model
 * `list_bill_payments` - List bill payments
 
 ### bills
 
 * `create_bill` - Create bill
-* `create_bill_attachments` - Create bill attachments
-* `delete_companies_company_id_connections_connection_id_push_bills_bill_id` - Delete bill
+* `delete_bill` - Delete bill
 * `download_bill_attachment` - Download bill attachment
 * `get_bill` - Get bill
 * `get_bill_attachment` - Get bill attachment
 * `get_bill_attachments` - List bill attachments
 * `get_create_update_bills_model` - Get create/update bill model
 * `list_bills` - List bills
 * `update_bill` - Update bill
+* `upload_bill_attachments` - Upload bill attachments
 
 ### company_info
 
 * `get_company_info` - Get company info
 * `post_sync_info` - Refresh company info
 
 ### credit_notes
 
-* `create_credit_note` - Update creditNote
+* `create_credit_note` - Create credit note
 * `get_create_update_credit_notes_model` - Get create/update credit note model
 * `get_credit_note` - Get credit note
 * `list_credit_notes` - List credit notes
-* `push_credit_note` - Create credit note
+* `update_credit_note` - Update creditNote
 
 ### customers
 
 * `create_customer` - Create customer
 * `download_customer_attachment` - Download customer attachment
 * `get_create_update_customers_model` - Get create/update customer model
 * `get_customer` - Get customer
@@ -124,45 +124,45 @@
 * `create_direct_cost` - Create direct cost
 * `download_direct_cost_attachment` - Download direct cost attachment
 * `get_create_direct_costs_model` - Get create direct cost model
 * `get_direct_cost` - Get direct cost
 * `get_direct_cost_attachment` - Get direct cost attachment
 * `get_direct_costs` - List direct costs
 * `list_direct_cost_attachments` - List direct cost attachments
-* `post_direct_cost_attachment` - Create direct cost attachment
+* `upload_direct_cost_attachment` - Upload direct cost attachment
 
 ### direct_incomes
 
 * `create_direct_income` - Create direct income
 * `download_direct_income_attachment` - Download direct income attachment
 * `get_create_direct_incomes_model` - Get create direct income model
 * `get_direct_income` - Get direct income
 * `get_direct_income_attachment` - Get direct income attachment
 * `get_direct_incomes` - Get direct incomes
 * `list_direct_income_attachments` - List direct income attachments
-* `post_direct_income_attachment` - Create direct income attachment
+* `upload_direct_income_attachment` - Create direct income attachment
 
 ### financials
 
 * `get_balance_sheet` - Get balance sheet
 * `get_cash_flow_statement` - Get cash flow statement
 * `get_profit_and_loss` - Get profit and loss
 
 ### invoices
 
+* `download_invoice_pdf` - Get invoice as PDF
 * `create_invoice` - Create invoice
-* `donwload_invoice_attachment` - Download invoice attachment
+* `download_invoice_attachment` - Download invoice attachment
 * `get_create_update_invoices_model` - Get create/update invoice model
 * `get_invoice` - Get invoice
 * `get_invoice_attachment` - Get invoice attachment
 * `get_invoice_attachments` - Get invoice attachments
-* `get_invoice_pdf` - Get invoice as PDF
 * `list_invoices` - List invoices
-* `push_invoice_attachment` - Push invoice attachment
 * `update_invoice` - Update invoice
+* `upload_invoice_attachment` - Push invoice attachment
 
 ### items
 
 * `create_item` - Create item
 * `get_create_items_model` - Get create item model
 * `get_item` - Get item
 * `list_items` - List items
@@ -211,15 +211,15 @@
 ### sales_orders
 
 * `get_sales_order` - Get sales order
 * `list_sales_orders` - List sales orders
 
 ### suppliers
 
-* `create_suppliers` - Create suppliers
+* `create_supplier` - Create suppliers
 * `download_supplier_attachment` - Download supplier attachment
 * `get_create_update_suppliers_model` - Get create/update supplier model
 * `get_supplier` - Get supplier
 * `get_supplier_attachment` - Get supplier attachment
 * `list_supplier_attachments` - List supplier attachments
 * `list_suppliers` - List suppliers
 * `put_supplier` - Update supplier
```

### Comparing `codat-accounting-0.5.1/src/codat/account_transactions.py` & `codat-accounting-0.9.6/src/codat/account_transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class AccountTransactions:
+    r"""Account transactions"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,43 +18,41 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_create_update_account_transactions_model(self, request: operations.GetCreateUpdateAccountTransactionsModelRequest) -> operations.GetCreateUpdateAccountTransactionsModelResponse:
+    def get_account_transaction(self, request: operations.GetAccountTransactionRequest) -> operations.GetAccountTransactionResponse:
         r"""Get account transaction
-        Get create/update account transactions model.
+        Gets the account transactions for a given company.Gets the specified account transaction for a given company and connection.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetCreateUpdateAccountTransactionsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/accountTransactions/{accountTransactionId}', request)
+        url = utils.generate_url(operations.GetAccountTransactionRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/accountTransactions/{accountTransactionId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCreateUpdateAccountTransactionsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAccountTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateAccountTransactionsModelSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AccountTransaction])
+                res.account_transaction = out
 
         return res
 
     def list_account_transactions(self, request: operations.ListAccountTransactionsRequest) -> operations.ListAccountTransactionsResponse:
         r"""List account transactions
         Gets the account transactions for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListAccountTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/accountTransactions', request)
         
         query_params = utils.get_query_params(operations.ListAccountTransactionsRequest, request)
         
         client = self._security_client
@@ -59,13 +60,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListAccountTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListAccountTransactionsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AccountTransactions])
+                res.account_transactions = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/accounts.py` & `codat-accounting-0.9.6/src/codat/accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Accounts:
+    r"""Accounts"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,112 +28,108 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create account model](https://docs.codat.io/accounting-api#/operations/get-create-chartOfAccounts-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts) for integrations that support creating an account.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/accounts', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "account", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateAccountRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateAccount200ApplicationJSON])
-                res.create_account_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateAccountResponse])
+                res.create_account_response = out
 
         return res
 
     def get_account(self, request: operations.GetAccountRequest) -> operations.GetAccountResponse:
         r"""Get account
         Gets a single account corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAccountRequest, base_url, '/companies/{companyId}/data/accounts/{accountId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Account])
+                res.account = out
 
         return res
 
-    def get_accounts(self, request: operations.GetAccountsRequest) -> operations.GetAccountsResponse:
-        r"""List accounts
-        Gets the latest accounts for a company
-        """
+    def get_create_chart_of_accounts_model(self, request: operations.GetCreateChartOfAccountsModelRequest) -> operations.GetCreateChartOfAccountsModelResponse:
+        r"""Get create account model
+        Get create account model. Returns the expected data for the request payload.
         
+        See the examples for integration-specific indicative models.
+        
+        > **Supported Integrations**
+        > 
+        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts) for integrations that support creating an account.
+        """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetAccountsRequest, base_url, '/companies/{companyId}/data/accounts', request)
+        url = utils.generate_url(operations.GetCreateChartOfAccountsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/chartOfAccounts', request)
         
-        query_params = utils.get_query_params(operations.GetAccountsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCreateChartOfAccountsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
+                res.push_option = out
 
         return res
 
-    def get_create_chart_of_accounts_model(self, request: operations.GetCreateChartOfAccountsModelRequest) -> operations.GetCreateChartOfAccountsModelResponse:
-        r"""Get create account model
-        Get create account model. Returns the expected data for the request payload.
-        
-        See the examples for integration-specific indicative models.
-        
-        > **Supported Integrations**
-        > 
-        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts) for integrations that support creating an account.
+    def list_accounts(self, request: operations.ListAccountsRequest) -> operations.ListAccountsResponse:
+        r"""List accounts
+        Gets the latest accounts for a company
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetCreateChartOfAccountsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/chartOfAccounts', request)
+        url = utils.generate_url(operations.ListAccountsRequest, base_url, '/companies/{companyId}/data/accounts', request)
         
+        query_params = utils.get_query_params(operations.ListAccountsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCreateChartOfAccountsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateChartOfAccountsModelPushOption])
-                res.push_option = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Accounts])
+                res.accounts = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/bank_account_transactions.py` & `codat-accounting-0.9.6/src/codat/bank_account_transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class BankAccountTransactions:
+    r"""Bank transactions for bank accounts"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,44 +18,73 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_bank_account_push_options(self, request: operations.GetBankAccountPushOptionsRequest) -> operations.GetBankAccountPushOptionsResponse:
+    def create_bank_transactions(self, request: operations.CreateBankTransactionsRequest) -> operations.CreateBankTransactionsResponse:
+        r"""Create bank transactions
+        Posts bank transactions to the accounting package for a given company.
+        
+        > **Supported Integrations**
+        > 
+        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankTransactions) for integrations that support POST methods.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.CreateBankTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{accountId}/bankTransactions', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "bank_transactions", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        query_params = utils.get_query_params(operations.CreateBankTransactionsRequest, request)
+        
+        client = self._security_client
+        
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.CreateBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBankTransactionsResponse])
+                res.create_bank_transactions_response = out
+
+        return res
+
+    def get_create_bank_account_model(self, request: operations.GetCreateBankAccountModelRequest) -> operations.GetCreateBankAccountModelResponse:
         r"""List push options for bank account bank transactions
         Gets the options of pushing bank account transactions.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetBankAccountPushOptionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bankAccounts/{accountId}/bankTransactions', request)
+        url = utils.generate_url(operations.GetCreateBankAccountModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bankAccounts/{accountId}/bankTransactions', request)
         
-        query_params = utils.get_query_params(operations.GetBankAccountPushOptionsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBankAccountPushOptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCreateBankAccountModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBankAccountPushOptionsPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def list_bank_account_transactions(self, request: operations.ListBankAccountTransactionsRequest) -> operations.ListBankAccountTransactionsResponse:
         r"""List bank transactions for bank account
         Gets bank transactions for a given bank account ID
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBankAccountTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bankAccounts/{accountId}/bankTransactions', request)
         
         query_params = utils.get_query_params(operations.ListBankAccountTransactionsRequest, request)
         
         client = self._security_client
@@ -60,24 +92,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBankAccountTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankAccountTransactionsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankTransactionsResponse])
+                res.bank_transactions_response = out
 
         return res
 
     def list_bank_transactions(self, request: operations.ListBankTransactionsRequest) -> operations.ListBankTransactionsResponse:
         r"""List all bank transactions
         Gets the latest bank transactions for given account ID and company. Doesn't require connection ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBankTransactionsRequest, base_url, '/companies/{companyId}/data/bankAccounts/{accountId}/transactions', request)
         
         query_params = utils.get_query_params(operations.ListBankTransactionsRequest, request)
         
         client = self._security_client
@@ -85,46 +116,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankTransactionsLinks])
-                res.links = out
-
-        return res
-
-    def post_bank_transactions(self, request: operations.PostBankTransactionsRequest) -> operations.PostBankTransactionsResponse:
-        r"""Create bank transactions
-        Posts bank transactions to the accounting package for a given company.
-        
-        > **Supported Integrations**
-        > 
-        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankTransactions) for integrations that support POST methods.
-        """
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.PostBankTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{accountId}/bankTransactions', request)
-        
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.PostBankTransactionsRequest, request)
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PostBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostBankTransactions200ApplicationJSON])
-                res.post_bank_transactions_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccountTransactions])
+                res.bank_account_transactions = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/bank_accounts.py` & `codat-accounting-0.9.6/src/codat/bank_accounts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class BankAccounts:
+    r"""Bank accounts"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,44 +28,42 @@
         
         Required data may vary by integration. To see what data to post, first call []().
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankAccounts) for integrations that support creating bank accounts.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateBankAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bank_account", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateBankAccountRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBankAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateBankAccount200ApplicationJSON])
-                res.create_bank_account_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBankAccountResponse])
+                res.create_bank_account_response = out
 
         return res
 
     def get_all_bank_account(self, request: operations.GetAllBankAccountRequest) -> operations.GetAllBankAccountResponse:
         r"""Get bank account
         Gets the bank account for given account ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAllBankAccountRequest, base_url, '/companies/{companyId}/data/bankAccounts/{accountId}', request)
         
         query_params = utils.get_query_params(operations.GetAllBankAccountRequest, request)
         
         client = self._security_client
@@ -70,78 +71,75 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllBankAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllBankAccount200ApplicationJSON])
-                res.get_all_bank_account_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankStatementAccount])
+                res.bank_statement_account = out
 
         return res
 
     def get_bank_account(self, request: operations.GetBankAccountRequest) -> operations.GetBankAccountResponse:
         r"""Get bank account
         Gets the bank account with a given ID
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBankAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bankAccounts/{accountId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBankAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBankAccountSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccount])
+                res.bank_account = out
 
         return res
 
     def get_create_update_bank_accounts_model(self, request: operations.GetCreateUpdateBankAccountsModelRequest) -> operations.GetCreateUpdateBankAccountsModelResponse:
         r"""Get create/update bank account model
         Get create/update bank account model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankAccounts) for integrations that support creating and updating bank accounts.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateBankAccountsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bankAccounts', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateBankAccountsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateBankAccountsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def list_bank_accounts(self, request: operations.ListBankAccountsRequest) -> operations.ListBankAccountsResponse:
         r"""List bank accounts
         Gets the list of bank accounts for a given connection
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBankAccountsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bankAccounts', request)
         
         query_params = utils.get_query_params(operations.ListBankAccountsRequest, request)
         
         client = self._security_client
@@ -149,48 +147,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBankAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankAccountsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccounts])
+                res.bank_accounts = out
 
         return res
 
-    def put_bank_account(self, request: operations.PutBankAccountRequest) -> operations.PutBankAccountResponse:
+    def update_bank_account(self, request: operations.UpdateBankAccountRequest) -> operations.UpdateBankAccountResponse:
         r"""Update bank account
         Posts an updated bank account to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call []().
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankAccounts) for integrations that support updating bank accounts.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PutBankAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{bankAccountId}', request)
+        url = utils.generate_url(operations.UpdateBankAccountRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{bankAccountId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bank_account", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.PutBankAccountRequest, request)
+        query_params = utils.get_query_params(operations.UpdateBankAccountRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutBankAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateBankAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutBankAccount200ApplicationJSON])
-                res.put_bank_account_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateBankAccountResponse])
+                res.update_bank_account_response = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/bill_credit_notes.py` & `codat-accounting-0.9.6/src/codat/bill_credit_notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class BillCreditNotes:
+    r"""Bill credit notes"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,96 +28,92 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create/update bill credit note model](https://docs.codat.io/accounting-api#/operations/get-create-update-billCreditNotes-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billCreditNotes) for integrations that support creating bill credit notes.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateBillCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/billCreditNotes', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bill_credit_note", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateBillCreditNoteRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBillCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateBillCreditNote200ApplicationJSON])
-                res.create_bill_credit_note_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBillCreditNoteResponse])
+                res.create_bill_credit_note_response = out
 
         return res
 
     def get_bill_credit_note(self, request: operations.GetBillCreditNoteRequest) -> operations.GetBillCreditNoteResponse:
         r"""Get bill credit note
         Gets a single billCreditNote corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBillCreditNoteRequest, base_url, '/companies/{companyId}/data/billCreditNotes/{billCreditNoteId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBillCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBillCreditNoteSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BillCreditNote])
+                res.bill_credit_note = out
 
         return res
 
     def get_create_update_bill_credit_notes_model(self, request: operations.GetCreateUpdateBillCreditNotesModelRequest) -> operations.GetCreateUpdateBillCreditNotesModelResponse:
         r"""Get create/update bill credit note model
         Get create/update bill credit note model.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billCreditNotes) for integrations that support creating and updating bill credit notes.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateBillCreditNotesModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/billCreditNotes', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateBillCreditNotesModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateBillCreditNotesModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def list_bill_credit_notes(self, request: operations.ListBillCreditNotesRequest) -> operations.ListBillCreditNotesResponse:
         r"""List bill credit notes
         Gets a list of all bill credit notes for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBillCreditNotesRequest, base_url, '/companies/{companyId}/data/billCreditNotes', request)
         
         query_params = utils.get_query_params(operations.ListBillCreditNotesRequest, request)
         
         client = self._security_client
@@ -122,48 +121,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBillCreditNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBillCreditNotesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BillCreditNotes])
+                res.bill_credit_notes = out
 
         return res
 
     def update_bill_credit_note(self, request: operations.UpdateBillCreditNoteRequest) -> operations.UpdateBillCreditNoteResponse:
         r"""Update bill credit note
         Posts an updated billCreditNote to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update bill credit note model](https://docs.codat.io/accounting-api#/operations/get-create-update-billCreditNotes-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billCreditNotes) for integrations that support updating bill credit notes.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateBillCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/billCreditNotes/{billCreditNoteId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bill_credit_note", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.UpdateBillCreditNoteRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateBillCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateBillCreditNote200ApplicationJSON])
-                res.update_bill_credit_note_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateBillCreditNoteResponse])
+                res.update_bill_credit_note_response = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/bill_payments.py` & `codat-accounting-0.9.6/src/codat/bill_payments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class BillPayments:
+    r"""Bill payments"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,124 +28,119 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create bill payment model](https://docs.codat.io/accounting-api#/operations/get-create-billPayments-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billPayments) for integrations that support creating bill payments.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateBillPaymentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/billPayments', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bill_payment", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateBillPaymentRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBillPaymentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateBillPayment200ApplicationJSON])
-                res.create_bill_payment_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBillPaymentResponse])
+                res.create_bill_payment_response = out
 
         return res
 
-    def delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id(self, request: operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDRequest) -> operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDResponse:
+    def delete_bill_payment(self, request: operations.DeleteBillPaymentRequest) -> operations.DeleteBillPaymentResponse:
         r"""Delete bill payment
         Deletes a bill payment from the accounting package for a given company.
         
         > **Supported Integrations**
         > 
         > This functionality is currently only supported for our Oracle NetSuite integration. Check out our [public roadmap](https://portal.productboard.com/codat/7-public-product-roadmap/tabs/46-accounting-api) to see what we're building next, and to submit ideas for new features.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/billPayments/{billPaymentId}', request)
+        url = utils.generate_url(operations.DeleteBillPaymentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/billPayments/{billPaymentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('DELETE', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteBillPaymentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSON])
-                res.delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperationSummary])
+                res.push_operation_summary = out
 
         return res
 
     def get_bill_payments(self, request: operations.GetBillPaymentsRequest) -> operations.GetBillPaymentsResponse:
         r"""Get bill payment
         Get a bill payment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBillPaymentsRequest, base_url, '/companies/{companyId}/data/billPayments/{billPaymentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBillPaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBillPaymentsSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BillPayment])
+                res.bill_payment = out
 
         return res
 
     def get_create_bill_payments_model(self, request: operations.GetCreateBillPaymentsModelRequest) -> operations.GetCreateBillPaymentsModelResponse:
         r"""Get create bill payment model
         Get create bill payment model.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billPayments) for integrations that support creating and deleting bill payments.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateBillPaymentsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/billPayments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateBillPaymentsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateBillPaymentsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def list_bill_payments(self, request: operations.ListBillPaymentsRequest) -> operations.ListBillPaymentsResponse:
         r"""List bill payments
         Gets the latest billPayments for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBillPaymentsRequest, base_url, '/companies/{companyId}/data/billPayments', request)
         
         query_params = utils.get_query_params(operations.ListBillPaymentsRequest, request)
         
         client = self._security_client
@@ -150,13 +148,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBillPaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBillPaymentsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BillPayments])
+                res.bill_payments = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/bills.py` & `codat-accounting-0.9.6/src/codat/bills.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Bills:
+    r"""Bills"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,220 +28,187 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create/update bill model](https://docs.codat.io/accounting-api#/operations/get-create-update-bills-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bills) for integrations that support creating a bill.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateBillRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bill", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateBillRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBillResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateBill200ApplicationJSON])
-                res.create_bill_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBillResponse])
+                res.create_bill_response = out
 
         return res
 
-    def create_bill_attachments(self, request: operations.CreateBillAttachmentsRequest) -> operations.CreateBillAttachmentsResponse:
-        r"""Create bill attachments
-        Post bill attachments
-        """
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.CreateBillAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills/{billId}/attachments', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.CreateBillAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            pass
-
-        return res
-
-    def delete_companies_company_id_connections_connection_id_push_bills_bill_id(self, request: operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDRequest) -> operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDResponse:
+    def delete_bill(self, request: operations.DeleteBillRequest) -> operations.DeleteBillResponse:
         r"""Delete bill
         Deletes a bill from the accounting package for a given company.
         
         > **Supported Integrations**
         > 
         > This functionality is currently only supported for our Oracle NetSuite integration. Check out our [public roadmap](https://portal.productboard.com/codat/7-public-product-roadmap/tabs/46-accounting-api) to see what we're building next, and to submit ideas for new features.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills/{billId}', request)
+        url = utils.generate_url(operations.DeleteBillRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills/{billId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('DELETE', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteBillResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSON])
-                res.delete_companies_company_id_connections_connection_id_push_bills_bill_id_200_application_json_object = out
-            if utils.match_content_type(content_type, 'application/xml'):
-                res.body = http_res.content
-            if utils.match_content_type(content_type, 'multipart/form-data'):
-                res.body = http_res.content
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOperationSummary])
+                res.push_operation_summary = out
 
         return res
 
     def download_bill_attachment(self, request: operations.DownloadBillAttachmentRequest) -> operations.DownloadBillAttachmentResponse:
         r"""Download bill attachment
         Download bill attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadBillAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bills/{billId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadBillAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_bill(self, request: operations.GetBillRequest) -> operations.GetBillResponse:
         r"""Get bill
         Get bill
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBillRequest, base_url, '/companies/{companyId}/data/bills/{billId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBillResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBillSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Bill])
+                res.bill = out
 
         return res
 
     def get_bill_attachment(self, request: operations.GetBillAttachmentRequest) -> operations.GetBillAttachmentResponse:
         r"""Get bill attachment
         Get bill attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBillAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bills/{billId}/attachments/{attachmentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBillAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBillAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def get_bill_attachments(self, request: operations.GetBillAttachmentsRequest) -> operations.GetBillAttachmentsResponse:
         r"""List bill attachments
         Get bill attachments
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBillAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bills/{billId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBillAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBillAttachmentsAttachments])
-                res.attachments = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
     def get_create_update_bills_model(self, request: operations.GetCreateUpdateBillsModelRequest) -> operations.GetCreateUpdateBillsModelResponse:
         r"""Get create/update bill model
         Get create/update bill model.
         
          > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bills) for integrations that support creating and updating a bill.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateBillsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bills', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateBillsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateBillsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def list_bills(self, request: operations.ListBillsRequest) -> operations.ListBillsResponse:
         r"""List bills
         Gets the latest bills for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListBillsRequest, base_url, '/companies/{companyId}/data/bills', request)
         
         query_params = utils.get_query_params(operations.ListBillsRequest, request)
         
         client = self._security_client
@@ -246,48 +216,70 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBillsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBillsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Bills])
+                res.bills = out
 
         return res
 
     def update_bill(self, request: operations.UpdateBillRequest) -> operations.UpdateBillResponse:
         r"""Update bill
         Posts an updated bill to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update bill model](https://docs.codat.io/accounting-api#/operations/get-create-update-bills-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bills) for integrations that support updating a bill.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateBillRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills/{billId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bill", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.UpdateBillRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateBillResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateBill200ApplicationJSON])
-                res.update_bill_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateBillResponse])
+                res.update_bill_response = out
+
+        return res
+
+    def upload_bill_attachments(self, request: operations.UploadBillAttachmentsRequest) -> operations.UploadBillAttachmentsResponse:
+        r"""Upload bill attachments
+        Upload bill attachments
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.UploadBillAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bills/{billId}/attachments', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.UploadBillAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/company_info.py` & `codat-accounting-0.9.6/src/codat/company_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class CompanyInfo:
+    r"""Company info"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,52 +22,50 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_company_info(self, request: operations.GetCompanyInfoRequest) -> operations.GetCompanyInfoResponse:
         r"""Get company info
         Gets the latest basic info for a company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCompanyInfoRequest, base_url, '/companies/{companyId}/data/info', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCompanyInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCompanyInfoCompanyInfo])
-                res.company_info = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyDataset])
+                res.company_dataset = out
 
         return res
 
     def post_sync_info(self, request: operations.PostSyncInfoRequest) -> operations.PostSyncInfoResponse:
         r"""Refresh company info
         Initiates the process of synchronising basic info for a company
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PostSyncInfoRequest, base_url, '/companies/{companyId}/data/info', request)
         
         
         client = self._security_client
         
         http_res = client.request('POST', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostSyncInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostSyncInfo200ApplicationJSON])
-                res.post_sync_info_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Dataset])
+                res.dataset = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/credit_notes.py` & `codat-accounting-0.9.6/src/codat/credit_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class CreditNotes:
+    r"""Credit notes"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -16,107 +19,104 @@
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def create_credit_note(self, request: operations.CreateCreditNoteRequest) -> operations.CreateCreditNoteResponse:
-        r"""Update creditNote
-        Posts an updated credit note to the accounting package for a given company.
+        r"""Create credit note
+        Push credit note
+        
         
         Required data may vary by integration. To see what data to post, first call [Get create/update credit note model](https://docs.codat.io/accounting-api#/operations/get-create-update-creditNotes-model).
         
         > **Supported Integrations**
         > 
-        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=creditNotes) for integrations that support updating a credit note.
+        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=creditNotes) for integrations that support creating a credit note.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.CreateCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/creditNotes/{creditNoteId}', request)
+        url = utils.generate_url(operations.CreateCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/creditNotes', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "credit_note", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateCreditNoteRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateCreditNote200ApplicationJSON])
-                res.create_credit_note_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateCreditNoteResponse])
+                res.create_credit_note_response = out
 
         return res
 
     def get_create_update_credit_notes_model(self, request: operations.GetCreateUpdateCreditNotesModelRequest) -> operations.GetCreateUpdateCreditNotesModelResponse:
         r"""Get create/update credit note model
         Get create/update credit note model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=creditNotes) for integrations that support creating and updating a credit note.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateCreditNotesModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/creditNotes', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateCreditNotesModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateCreditNotesModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_credit_note(self, request: operations.GetCreditNoteRequest) -> operations.GetCreditNoteResponse:
         r"""Get credit note
         Gets a single creditNote corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreditNoteRequest, base_url, '/companies/{companyId}/data/creditNotes/{creditNoteId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreditNoteSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreditNote])
+                res.credit_note = out
 
         return res
 
     def list_credit_notes(self, request: operations.ListCreditNotesRequest) -> operations.ListCreditNotesResponse:
         r"""List credit notes
         Gets a list of all credit notes for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListCreditNotesRequest, base_url, '/companies/{companyId}/data/creditNotes', request)
         
         query_params = utils.get_query_params(operations.ListCreditNotesRequest, request)
         
         client = self._security_client
@@ -124,49 +124,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListCreditNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCreditNotesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreditNotes])
+                res.credit_notes = out
 
         return res
 
-    def push_credit_note(self, request: operations.PushCreditNoteRequest) -> operations.PushCreditNoteResponse:
-        r"""Create credit note
-        Push credit note
-        
+    def update_credit_note(self, request: operations.UpdateCreditNoteRequest) -> operations.UpdateCreditNoteResponse:
+        r"""Update creditNote
+        Posts an updated credit note to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update credit note model](https://docs.codat.io/accounting-api#/operations/get-create-update-creditNotes-model).
         
         > **Supported Integrations**
         > 
-        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=creditNotes) for integrations that support creating a credit note.
+        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=creditNotes) for integrations that support updating a credit note.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PushCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/creditNotes', request)
+        url = utils.generate_url(operations.UpdateCreditNoteRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/creditNotes/{creditNoteId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "credit_note", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.PushCreditNoteRequest, request)
+        query_params = utils.get_query_params(operations.UpdateCreditNoteRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PushCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UpdateCreditNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PushCreditNote200ApplicationJSON])
-                res.push_credit_note_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateCreditNoteResponse])
+                res.update_credit_note_response = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/customers.py` & `codat-accounting-0.9.6/src/codat/customers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Customers:
+    r"""Customers"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,168 +28,162 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create/update customer model](https://docs.codat.io/accounting-api#/operations/get-create-update-customers-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support creating customers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateCustomerRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/customers', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "customer", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateCustomerRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateCustomerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateCustomer200ApplicationJSON])
-                res.create_customer_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateCustomerResponse])
+                res.create_customer_response = out
 
         return res
 
     def download_customer_attachment(self, request: operations.DownloadCustomerAttachmentRequest) -> operations.DownloadCustomerAttachmentResponse:
         r"""Download customer attachment
         Download customer attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadCustomerAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/customers/{customerId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadCustomerAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_create_update_customers_model(self, request: operations.GetCreateUpdateCustomersModelRequest) -> operations.GetCreateUpdateCustomersModelResponse:
         r"""Get create/update customer model
         Get create/update customer model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support creating and updating customers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateCustomersModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/customers', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateCustomersModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateCustomersModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_customer(self, request: operations.GetCustomerRequest) -> operations.GetCustomerResponse:
         r"""Get customer
         Gets a single customer corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCustomerRequest, base_url, '/companies/{companyId}/data/customers/{customerId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCustomerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomerSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
+                res.customer = out
 
         return res
 
     def get_customer_attachment(self, request: operations.GetCustomerAttachmentRequest) -> operations.GetCustomerAttachmentResponse:
         r"""Get customer attachment
         Get  customer attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCustomerAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/customers/{customerId}/attachments/{attachmentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCustomerAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomerAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def get_customer_attachments(self, request: operations.GetCustomerAttachmentsRequest) -> operations.GetCustomerAttachmentsResponse:
         r"""List customer attachments
         Get customer attachments
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCustomerAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/customers/{customerId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCustomerAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomerAttachmentsAttachments])
-                res.attachments = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
     def get_customers(self, request: operations.GetCustomersRequest) -> operations.GetCustomersResponse:
         r"""List customers
         Gets the latest customers for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCustomersRequest, base_url, '/companies/{companyId}/data/customers', request)
         
         query_params = utils.get_query_params(operations.GetCustomersRequest, request)
         
         client = self._security_client
@@ -194,48 +191,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customers])
+                res.customers = out
 
         return res
 
     def update_customer(self, request: operations.UpdateCustomerRequest) -> operations.UpdateCustomerResponse:
         r"""Update customer
         Posts an updated customer for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update customer model](https://docs.codat.io/accounting-api#/operations/get-create-update-customers-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers) for integrations that support updating customers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateCustomerRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/customers/{customerId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "customer", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.UpdateCustomerRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateCustomerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateCustomer200ApplicationJSON])
-                res.update_customer_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateCustomerResponse])
+                res.update_customer_response = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/direct_costs.py` & `codat-accounting-0.9.6/src/codat/direct_costs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class DirectCosts:
+    r"""Direct costs"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,144 +28,139 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create direct cost model](https://docs.codat.io/accounting-api#/operations/get-create-directCosts-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=directCosts) for integrations that support creating direct costs.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateDirectCostRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directCosts', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "direct_cost", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateDirectCostRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateDirectCostResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDirectCost200ApplicationJSON])
-                res.create_direct_cost_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateDirectCostResponse])
+                res.create_direct_cost_response = out
 
         return res
 
     def download_direct_cost_attachment(self, request: operations.DownloadDirectCostAttachmentRequest) -> operations.DownloadDirectCostAttachmentResponse:
         r"""Download direct cost attachment
         Downloads an attachment for the specified direct cost for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadDirectCostAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directCosts/{directCostId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadDirectCostAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_create_direct_costs_model(self, request: operations.GetCreateDirectCostsModelRequest) -> operations.GetCreateDirectCostsModelResponse:
         r"""Get create direct cost model
         Get create direct cost model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=directCosts) for integrations that support creating direct costs.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateDirectCostsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/directCosts', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateDirectCostsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateDirectCostsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_direct_cost(self, request: operations.GetDirectCostRequest) -> operations.GetDirectCostResponse:
         r"""Get direct cost
         Gets the specified direct cost for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectCostRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directCosts/{directCostId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectCostResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectCostSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DirectCost])
+                res.direct_cost = out
 
         return res
 
     def get_direct_cost_attachment(self, request: operations.GetDirectCostAttachmentRequest) -> operations.GetDirectCostAttachmentResponse:
         r"""Get direct cost attachment
         Gets the specified direct cost attachment for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectCostAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directCosts/{directCostId}/attachments/{attachmentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectCostAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectCostAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def get_direct_costs(self, request: operations.GetDirectCostsRequest) -> operations.GetDirectCostsResponse:
         r"""List direct costs
         Gets the direct costs for the company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectCostsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directCosts', request)
         
         query_params = utils.get_query_params(operations.GetDirectCostsRequest, request)
         
         client = self._security_client
@@ -170,59 +168,59 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectCostsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectCostsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DirectCosts])
+                res.direct_costs = out
 
         return res
 
     def list_direct_cost_attachments(self, request: operations.ListDirectCostAttachmentsRequest) -> operations.ListDirectCostAttachmentsResponse:
         r"""List direct cost attachments
         Gets all attachments for the specified direct cost for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListDirectCostAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directCosts/{directCostId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListDirectCostAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListDirectCostAttachmentsAttachments])
-                res.attachments = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
-    def post_direct_cost_attachment(self, request: operations.PostDirectCostAttachmentRequest) -> operations.PostDirectCostAttachmentResponse:
-        r"""Create direct cost attachment
+    def upload_direct_cost_attachment(self, request: operations.UploadDirectCostAttachmentRequest) -> operations.UploadDirectCostAttachmentResponse:
+        r"""Upload direct cost attachment
         Posts a new direct cost attachment for a given company.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PostDirectCostAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directCosts/{directCostId}/attachment', request)
+        url = utils.generate_url(operations.UploadDirectCostAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directCosts/{directCostId}/attachment', request)
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url)
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostDirectCostAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UploadDirectCostAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
-            pass
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/direct_incomes.py` & `codat-accounting-0.9.6/src/codat/direct_incomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class DirectIncomes:
+    r"""Direct incomes"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,120 +28,116 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create direct income model](https://docs.codat.io/accounting-api#/operations/get-create-directIncomes-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=directIncomes) for integrations that support creating direct incomes.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateDirectIncomeRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directIncomes', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "direct_income", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateDirectIncomeRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateDirectIncomeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDirectIncome200ApplicationJSON])
-                res.create_direct_income_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateDirectIncomeResponse])
+                res.create_direct_income_response = out
 
         return res
 
     def download_direct_income_attachment(self, request: operations.DownloadDirectIncomeAttachmentRequest) -> operations.DownloadDirectIncomeAttachmentResponse:
         r"""Download direct income attachment
         Downloads an attachment for the specified direct income for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadDirectIncomeAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directIncomes/{directIncomeId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadDirectIncomeAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_create_direct_incomes_model(self, request: operations.GetCreateDirectIncomesModelRequest) -> operations.GetCreateDirectIncomesModelResponse:
         r"""Get create direct income model
         Get create direct income model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=directIncomes) for integrations that support creating direct incomes.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateDirectIncomesModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/directIncomes', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateDirectIncomesModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateDirectIncomesModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_direct_income(self, request: operations.GetDirectIncomeRequest) -> operations.GetDirectIncomeResponse:
         r"""Get direct income
         Gets the specified direct income for a given company and connection.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectIncomeRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directIncomes/{directIncomeId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectIncomeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectIncomeSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DirectIncome])
+                res.direct_income = out
 
         return res
 
     def get_direct_income_attachment(self, request: operations.GetDirectIncomeAttachmentRequest) -> operations.GetDirectIncomeAttachmentResponse:
         r"""Get direct income attachment
         Gets the specified direct income attachment for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectIncomeAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directIncomes/{directIncomeId}/attachments/{attachmentId}', request)
         
         query_params = utils.get_query_params(operations.GetDirectIncomeAttachmentRequest, request)
         
         client = self._security_client
@@ -146,24 +145,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectIncomeAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectIncomeAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def get_direct_incomes(self, request: operations.GetDirectIncomesRequest) -> operations.GetDirectIncomesResponse:
         r"""Get direct incomes
         Gets the direct incomes for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDirectIncomesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directIncomes', request)
         
         query_params = utils.get_query_params(operations.GetDirectIncomesRequest, request)
         
         client = self._security_client
@@ -171,59 +169,59 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDirectIncomesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDirectIncomesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.DirectIncomes])
+                res.direct_incomes = out
 
         return res
 
     def list_direct_income_attachments(self, request: operations.ListDirectIncomeAttachmentsRequest) -> operations.ListDirectIncomeAttachmentsResponse:
         r"""List direct income attachments
         Gets all attachments for the specified direct income for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListDirectIncomeAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/directIncomes/{directIncomeId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListDirectIncomeAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListDirectIncomeAttachmentsAttachments])
-                res.attachments = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
-    def post_direct_income_attachment(self, request: operations.PostDirectIncomeAttachmentRequest) -> operations.PostDirectIncomeAttachmentResponse:
+    def upload_direct_income_attachment(self, request: operations.UploadDirectIncomeAttachmentRequest) -> operations.UploadDirectIncomeAttachmentResponse:
         r"""Create direct income attachment
         Posts a new direct income attachment for a given company.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PostDirectIncomeAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directIncomes/{directIncomeId}/attachment', request)
+        url = utils.generate_url(operations.UploadDirectIncomeAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/directIncomes/{directIncomeId}/attachment', request)
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url)
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostDirectIncomeAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.UploadDirectIncomeAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
-            pass
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/financials.py` & `codat-accounting-0.9.6/src/codat/financials.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Financials:
+    r"""Financials"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,15 +22,14 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_balance_sheet(self, request: operations.GetBalanceSheetRequest) -> operations.GetBalanceSheetResponse:
         r"""Get balance sheet
         Gets the latest balance sheet for a company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetBalanceSheetRequest, base_url, '/companies/{companyId}/data/financials/balanceSheet', request)
         
         query_params = utils.get_query_params(operations.GetBalanceSheetRequest, request)
         
         client = self._security_client
@@ -35,24 +37,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBalanceSheetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBalanceSheet200ApplicationJSON])
-                res.get_balance_sheet_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BalanceSheet1])
+                res.balance_sheet = out
 
         return res
 
     def get_cash_flow_statement(self, request: operations.GetCashFlowStatementRequest) -> operations.GetCashFlowStatementResponse:
         r"""Get cash flow statement
         Gets the latest cash flow statement for a company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCashFlowStatementRequest, base_url, '/companies/{companyId}/data/financials/cashFlowStatement', request)
         
         query_params = utils.get_query_params(operations.GetCashFlowStatementRequest, request)
         
         client = self._security_client
@@ -60,24 +61,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCashFlowStatementResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCashFlowStatement200ApplicationJSON])
-                res.get_cash_flow_statement_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CashFlowStatement1])
+                res.cash_flow_statement = out
 
         return res
 
     def get_profit_and_loss(self, request: operations.GetProfitAndLossRequest) -> operations.GetProfitAndLossResponse:
         r"""Get profit and loss
         Gets the latest profit and loss for a company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetProfitAndLossRequest, base_url, '/companies/{companyId}/data/financials/profitAndLoss', request)
         
         query_params = utils.get_query_params(operations.GetProfitAndLossRequest, request)
         
         client = self._security_client
@@ -85,13 +85,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetProfitAndLossResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetProfitAndLoss200ApplicationJSON])
-                res.get_profit_and_loss_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ProfitAndLossReport1])
+                res.profit_and_loss_report = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/invoices.py` & `codat-accounting-0.9.6/src/codat/invoices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Invoices:
+    r"""Invoices"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,200 +18,194 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    def download_invoice_pdf(self, request: operations.DownloadInvoicePdfRequest) -> operations.DownloadInvoicePdfResponse:
+        r"""Get invoice as PDF
+        Get invoice as PDF
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DownloadInvoicePdfRequest, base_url, '/companies/{companyId}/data/invoices/{invoiceId}/pdf', request)
+        
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DownloadInvoicePdfResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
+
+        return res
+
     def create_invoice(self, request: operations.CreateInvoiceRequest) -> operations.CreateInvoiceResponse:
         r"""Create invoice
         Posts a new invoice to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update invoice model](https://docs.codat.io/accounting-api#/operations/get-create-update-invoices-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=invoices) for integrations that support creating invoices.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateInvoiceRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/invoices', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "invoice", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateInvoiceRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateInvoiceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateInvoice200ApplicationJSON])
-                res.create_invoice_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateInvoiceResponse])
+                res.create_invoice_response = out
 
         return res
 
-    def donwload_invoice_attachment(self, request: operations.DonwloadInvoiceAttachmentRequest) -> operations.DonwloadInvoiceAttachmentResponse:
+    def download_invoice_attachment(self, request: operations.DownloadInvoiceAttachmentRequest) -> operations.DownloadInvoiceAttachmentResponse:
         r"""Download invoice attachment
         Download invoice attachments
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.DonwloadInvoiceAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/invoices/{invoiceId}/attachments/{attachmentId}/download', request)
+        url = utils.generate_url(operations.DownloadInvoiceAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/invoices/{invoiceId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DonwloadInvoiceAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DownloadInvoiceAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_create_update_invoices_model(self, request: operations.GetCreateUpdateInvoicesModelRequest) -> operations.GetCreateUpdateInvoicesModelResponse:
         r"""Get create/update invoice model
         Get create/update invoice model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=invoices) for integrations that support creating and updating invoices.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateInvoicesModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/invoices', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateInvoicesModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateInvoicesModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_invoice(self, request: operations.GetInvoiceRequest) -> operations.GetInvoiceResponse:
         r"""Get invoice
         Get invoice
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetInvoiceRequest, base_url, '/companies/{companyId}/data/invoices/{invoiceId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInvoiceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetInvoiceSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Invoice])
+                res.invoice = out
 
         return res
 
     def get_invoice_attachment(self, request: operations.GetInvoiceAttachmentRequest) -> operations.GetInvoiceAttachmentResponse:
         r"""Get invoice attachment
-        Get invoice attachments
+        Get invoice attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetInvoiceAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/invoices/{invoiceId}/attachments/{attachmentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInvoiceAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetInvoiceAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def get_invoice_attachments(self, request: operations.GetInvoiceAttachmentsRequest) -> operations.GetInvoiceAttachmentsResponse:
         r"""Get invoice attachments
         Get invoice attachments
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetInvoiceAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/invoices/{invoiceId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInvoiceAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetInvoiceAttachmentsAttachments])
-                res.attachments = out
-
-        return res
-
-    def get_invoice_pdf(self, request: operations.GetInvoicePdfRequest) -> operations.GetInvoicePdfResponse:
-        r"""Get invoice as PDF
-        Get invoice as PDF
-        """
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetInvoicePdfRequest, base_url, '/companies/{companyId}/data/invoices/{invoiceId}/pdf', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetInvoicePdfResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            pass
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
     def list_invoices(self, request: operations.ListInvoicesRequest) -> operations.ListInvoicesResponse:
         r"""List invoices
         Gets the latest invoices for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListInvoicesRequest, base_url, '/companies/{companyId}/data/invoices', request)
         
         query_params = utils.get_query_params(operations.ListInvoicesRequest, request)
         
         client = self._security_client
@@ -216,70 +213,70 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListInvoicesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListInvoicesLinks])
-                res.links = out
-
-        return res
-
-    def push_invoice_attachment(self, request: operations.PushInvoiceAttachmentRequest) -> operations.PushInvoiceAttachmentResponse:
-        r"""Push invoice attachment
-        Push invoice attachment
-        """
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.PushInvoiceAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/invoices/{invoiceId}/attachment', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PushInvoiceAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            pass
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Invoices])
+                res.invoices = out
 
         return res
 
     def update_invoice(self, request: operations.UpdateInvoiceRequest) -> operations.UpdateInvoiceResponse:
         r"""Update invoice
         Posts an updated invoice to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create/update invoice model](https://docs.codat.io/accounting-api#/operations/get-create-update-invoices-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=invoices) for integrations that support updating invoices.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateInvoiceRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/invoices/{invoiceId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "invoice", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.UpdateInvoiceRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateInvoiceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateInvoice200ApplicationJSON])
-                res.update_invoice_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateInvoiceResponse])
+                res.update_invoice_response = out
+
+        return res
+
+    def upload_invoice_attachment(self, request: operations.UploadInvoiceAttachmentRequest) -> operations.UploadInvoiceAttachmentResponse:
+        r"""Push invoice attachment
+        Push invoice attachment
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.UploadInvoiceAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/invoices/{invoiceId}/attachment', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.UploadInvoiceAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/items.py` & `codat-accounting-0.9.6/src/codat/items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Items:
+    r"""Items"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,98 +28,94 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create item model](https://docs.codat.io/accounting-api#/operations/get-create-items-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=items) for integrations that support creating items.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateItemRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/items', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "item", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateItemRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateItemResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateItem200ApplicationJSON])
-                res.create_item_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateItemResponse])
+                res.create_item_response = out
 
         return res
 
     def get_create_items_model(self, request: operations.GetCreateItemsModelRequest) -> operations.GetCreateItemsModelResponse:
         r"""Get create item model
         Get create item model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=items) for integrations that support creating items.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateItemsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/items', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateItemsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateItemsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_item(self, request: operations.GetItemRequest) -> operations.GetItemResponse:
         r"""Get item
         Gets the specified item for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetItemRequest, base_url, '/companies/{companyId}/data/items/{itemId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetItemResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetItemSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Item])
+                res.item = out
 
         return res
 
     def list_items(self, request: operations.ListItemsRequest) -> operations.ListItemsResponse:
         r"""List items
         Gets the items for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListItemsRequest, base_url, '/companies/{companyId}/data/items', request)
         
         query_params = utils.get_query_params(operations.ListItemsRequest, request)
         
         client = self._security_client
@@ -124,13 +123,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListItemsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListItemsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Items1])
+                res.items = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/journal_entries.py` & `codat-accounting-0.9.6/src/codat/journal_entries.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class JournalEntries:
+    r"""Journal entries"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,98 +28,94 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create journal entry model](https://docs.codat.io/accounting-api#/operations/get-create-journalEntries-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journalEntries) for integrations that support creating journal entries.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateJournalEntryRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/journalEntries', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "journal_entry", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreateJournalEntryRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateJournalEntryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateJournalEntry200ApplicationJSON])
-                res.create_journal_entry_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateJournalEntryResponse])
+                res.create_journal_entry_response = out
 
         return res
 
     def get_create_journal_entries_model(self, request: operations.GetCreateJournalEntriesModelRequest) -> operations.GetCreateJournalEntriesModelResponse:
         r"""Get create journal entry model
         Get create journal entry model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journalEntries) for integrations that support creating journal entries.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateJournalEntriesModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/journalEntries', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateJournalEntriesModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateJournalEntriesModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_journal_entry(self, request: operations.GetJournalEntryRequest) -> operations.GetJournalEntryResponse:
         r"""Get journal entry
         Gets a single JournalEntry corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetJournalEntryRequest, base_url, '/companies/{companyId}/data/journalEntries/{journalEntryId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetJournalEntryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetJournalEntrySourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.JournalEntry])
+                res.journal_entry = out
 
         return res
 
     def list_journal_entries(self, request: operations.ListJournalEntriesRequest) -> operations.ListJournalEntriesResponse:
         r"""List journal entries
         Gets the latest journal entries for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListJournalEntriesRequest, base_url, '/companies/{companyId}/data/journalEntries', request)
         
         query_params = utils.get_query_params(operations.ListJournalEntriesRequest, request)
         
         client = self._security_client
@@ -124,13 +123,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListJournalEntriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListJournalEntriesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.JournalEntries])
+                res.journal_entries = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/journals.py` & `codat-accounting-0.9.6/src/codat/journals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Journals:
+    r"""Journals"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,63 +28,60 @@
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journals) for integrations that support creating journals.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateJournalsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/journals', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateJournalsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateJournalsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_journal(self, request: operations.GetJournalRequest) -> operations.GetJournalResponse:
         r"""Get journal
         Gets a single journal corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetJournalRequest, base_url, '/companies/{companyId}/data/journals/{journalId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetJournalResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetJournalSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Journal])
+                res.journal = out
 
         return res
 
     def list_journals(self, request: operations.ListJournalsRequest) -> operations.ListJournalsResponse:
         r"""List journals
         Gets the latest journals for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListJournalsRequest, base_url, '/companies/{companyId}/data/journals', request)
         
         query_params = utils.get_query_params(operations.ListJournalsRequest, request)
         
         client = self._security_client
@@ -89,36 +89,35 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListJournalsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListJournalsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Journals])
+                res.journals = out
 
         return res
 
     def push_journal(self, request: operations.PushJournalRequest) -> operations.PushJournalResponse:
         r"""Create journal
         Posts a new journal to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call [Get create journal model](https://docs.codat.io/accounting-api#/operations/get-create-journals-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journals) for integrations that support creating journals.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PushJournalRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/journals', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "journal", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.PushJournalRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/create_bill_attachments.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_bill.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import bill as shared_bill
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateBillAttachmentsRequest:
+class GetBillRequest:
+    
     bill_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a bill"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class CreateBillAttachmentsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetBillResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    bill: Optional[shared_bill.Bill] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/delete_companies_companyid_connections_connectionid_push_billpayments_billpaymentid.py` & `codat-accounting-0.9.6/src/codat/models/shared/customer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,101 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import addressesitems as shared_addressesitems
+from ..shared import contact as shared_contact
+from ..shared import customerstatus_enum as shared_customerstatus_enum
+from ..shared import metadata as shared_metadata
+from ..shared import supplementaldata as shared_supplementaldata
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDRequest:
-    bill_payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billPaymentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChangesPushOperationRecordRef:
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class Customer:
+    r"""> View the coverage for customers in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=customers\\" target=\\"_blank\\">Data coverage explorer</a>.
     
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChangesTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    CREATED = "Created"
-    MODIFIED = "Modified"
-    DELETED = "Deleted"
-    ATTACHMENT_UPLOADED = "AttachmentUploaded"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChanges:
-    attachment_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attachmentId'), 'exclude': lambda f: f is None }})
-    record_ref: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChangesPushOperationRecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRef'), 'exclude': lambda f: f is None }})
-    type: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChangesTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-    
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONStatusEnum(str, Enum):
-    PENDING = "Pending"
-    FAILED = "Failed"
-    SUCCESS = "Success"
-    TIMED_OUT = "TimedOut"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidationValidationItem:
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
+    ## Overview
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidation:
-    r"""DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidation
-    A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here.
+    A customer is a person or organisation that buys goods or services. From the Customers endpoints, you can retrieve a [list of all the customers of a company](https://api.codat.io/swagger/index.html#/Customers/get_companies__companyId__data_customers).
+    
+    Customers' data links to accounts receivable [invoices](https://docs.codat.io/accounting-api#/schemas/Invoice).
     """
     
-    errors: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidationValidationItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
-    warnings: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidationValidationItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
+    status: shared_customerstatus_enum.CustomerStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""Status of customer."""  
+    addresses: Optional[list[shared_addressesitems.Addressesitems]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addresses'), 'exclude': lambda f: f is None }})
+    r"""An array of Addresses."""  
+    contact_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactName'), 'exclude': lambda f: f is None }})
+    r"""Name of the main contact for the identified customer."""  
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+    r"""An array of Contacts."""  
+    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is None }})
+    r"""Name of the customer as recorded in the accounting system, typically the company name."""  
+    default_currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCurrency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
+    
+    ## Unknown currencies
+    
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
+    
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
+    email_address: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailAddress'), 'exclude': lambda f: f is None }})
+    r"""Email address the customer can be contacted by."""  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the customer, unique to the company in the accounting platform."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSON:
-    company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
-    data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
-    push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
-    requested_on_utc: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    status: DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})
-    changes: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONChanges]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})
-    completed_on_utc: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})
-    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})
-    validation: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSONValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
     
-
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentIDResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id_200_application_json_object: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillPaymentsBillPaymentID200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    r"""Phone number the customer can be contacted by."""  
+    registration_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('registrationNumber'), 'exclude': lambda f: f is None }})
+    r"""Company number. In the UK, this is typically the Companies House company registration number."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    supplemental_data: Optional[shared_supplementaldata.SupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""  
+    tax_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxNumber'), 'exclude': lambda f: f is None }})
+    r"""Company tax number."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/delete_companies_companyid_connections_connectionid_push_bills_billid.py` & `codat-accounting-0.9.6/src/codat/models/operations/push_journal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,123 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
+from ..shared import datatype_enum as shared_datatype_enum
+from ..shared import journal as shared_journal
+from ..shared import pushoperationchange as shared_pushoperationchange
+from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
+from ..shared import validation as shared_validation
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDRequest:
-    bill_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
+class PushJournalRequest:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChangesPushOperationRecordRef:
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChangesTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    CREATED = "Created"
-    MODIFIED = "Modified"
-    DELETED = "Deleted"
-    ATTACHMENT_UPLOADED = "AttachmentUploaded"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChanges:
-    attachment_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attachmentId'), 'exclude': lambda f: f is None }})
-    record_ref: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChangesPushOperationRecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRef'), 'exclude': lambda f: f is None }})
-    type: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChangesTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-    
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONStatusEnum(str, Enum):
-    PENDING = "Pending"
-    FAILED = "Failed"
-    SUCCESS = "Success"
-    TIMED_OUT = "TimedOut"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidationValidationItem:
-    item_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemId'), 'exclude': lambda f: f is None }})
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-    validator_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validatorName'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    journal: Optional[shared_journal.Journal] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeoutInMinutes', 'style': 'form', 'explode': True }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidation:
-    r"""DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidation
-    A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here.
-    """
-    
-    errors: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidationValidationItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})
-    warnings: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidationValidationItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
+class PushJournal200ApplicationJSON:
+    r"""Success"""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSON:
     company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
+    r"""Unique identifier for your SMB in Codat."""  
     data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
+    r"""Unique identifier for a company's data connection."""  
     push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
-    requested_on_utc: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    status: DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})
-    changes: Optional[list[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONChanges]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})
-    completed_on_utc: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})
-    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})
-    validation: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSONValidation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A unique identifier generated by Codat to represent this single push operation. This identifier can be used to track the status of the push, and should be persisted."""  
+    requested_on_utc: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: shared_pushoperationstatus_enum.PushOperationStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The status of the push operation."""  
+    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})  
+    changes: Optional[list[shared_pushoperationchange.PushOperationChange]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})  
+    completed_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    data: Optional[shared_journal.Journal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    r"""> **Language tip:** For line items, or individual transactions, of a company's financial documents, refer to the [Journal entries](https://docs.codat.io/accounting-api#/schemas/JournalEntry) data type
+    
+    > View the coverage for journals in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journals\" target=\"_blank\">Data coverage explorer</a>.
+    
+    ## Overview
+    
+    In accounting software, journals are used to record all the financial transactions of a company. Each transaction in a journal is represented by a separate [journal entry](https://docs.codat.io/accounting-api#/schemas/JournalEntry). These entries are used to create the general ledger, which is then used to create the financial statements of a business.
+    
+    When a company records all their transactions in a single journal, it can become large and difficult to maintain and track. This is why large companies often use multiple journals (also known as subjournals) to categorize and manage journal entries.
+    
+    Such journals can be divided into two categories:
+    
+    - Special journals: journals used to record specific types of transactions; for example, a purchases journal, a sales journal, or a cash management journal.
+    - General journals: journals used to record transactions that fall outside the scope of the special journals.
+    
+    Multiple journals or subjournals are used in the following Codat integrations:
+    
+    - [Sage Intacct](https://docs.codat.io/integrations/accounting/sage-intacct/accounting-sage-intacct)  (mandatory)
+    - [Exact Online](https://docs.codat.io/integrations/accounting/exact-online/accounting-exact-online)  (mandatory)
+    - [Oracle NetSuite](https://docs.codat.io/integrations/accounting/netsuite/accounting-netsuite) (optional)
+    
+    > When pushing journal entries to an accounting platform that doesn’t support multiple journals (multi-book accounting), the entries will be linked to the platform-generic journal. The Journals data type will only include one object.
+    """  
+    data_type: Optional[shared_datatype_enum.DataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})  
+    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_validation.Validation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here."""  
     
 
 @dataclasses.dataclass
-class DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillIDResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    body: Optional[bytes] = dataclasses.field(default=None)
-    delete_companies_company_id_connections_connection_id_push_bills_bill_id_200_application_json_object: Optional[DeleteCompaniesCompanyIDConnectionsConnectionIDPushBillsBillID200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class PushJournalResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    push_journal_200_application_json_object: Optional[PushJournal200ApplicationJSON] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/donwload_invoice_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/download_supplier_attachment.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DonwloadInvoiceAttachmentRequest:
+class DownloadSupplierAttachmentRequest:
+    
     attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    invoice_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'invoiceId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for an attachment"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    supplier_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'supplierId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a supplier"""  
     
 
 @dataclasses.dataclass
-class DonwloadInvoiceAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class DownloadSupplierAttachmentResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    data: Optional[bytes] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/download_bill_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_bill_attachment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import attachment as shared_attachment
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DownloadBillAttachmentRequest:
+class GetBillAttachmentRequest:
+    
     attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for an attachment"""  
     bill_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a bill"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class DownloadBillAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetBillAttachmentResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    attachment: Optional[shared_attachment.Attachment] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/download_customer_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/download_customer_attachment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DownloadCustomerAttachmentRequest:
+    
     attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customerId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for an attachment"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customerId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class DownloadCustomerAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    data: Optional[bytes] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/download_direct_cost_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/download_direct_income_attachment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DownloadDirectCostAttachmentRequest:
+class DownloadDirectIncomeAttachmentRequest:
+    
     attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    direct_cost_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directCostId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for an attachment"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    direct_income_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directIncomeId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a direct income"""  
     
 
 @dataclasses.dataclass
-class DownloadDirectCostAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class DownloadDirectIncomeAttachmentResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    data: Optional[bytes] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/download_direct_income_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/download_bill_attachment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DownloadDirectIncomeAttachmentRequest:
+class DownloadBillAttachmentRequest:
+    
     attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    direct_income_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directIncomeId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for an attachment"""  
+    bill_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a bill"""  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class DownloadDirectIncomeAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class DownloadBillAttachmentResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    data: Optional[bytes] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/download_supplier_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/create_journal_entry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import createjournalentryresponse as shared_createjournalentryresponse
+from ..shared import journalentry as shared_journalentry
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DownloadSupplierAttachmentRequest:
-    attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    supplier_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'supplierId', 'style': 'simple', 'explode': False }})
+class CreateJournalEntryRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    journal_entry: Optional[shared_journalentry.JournalEntry] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeoutInMinutes', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
-class DownloadSupplierAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class CreateJournalEntryResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    create_journal_entry_response: Optional[shared_createjournalentryresponse.CreateJournalEntryResponse] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_account.py` & `codat-accounting-0.9.6/src/codat/models/shared/bankaccount.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,133 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import metadata as shared_metadata
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
+class BankAccountBankAccountTypeEnum(str, Enum):
+    r"""The type of transactions and balances on the account.
+    For Credit accounts, positive balances are liabilities, and positive transactions **reduce** liabilities.  
+    For Debit accounts, positive balances are assets, and positive transactions **increase** assets.
+    """
+    UNKNOWN = 'Unknown'
+    CREDIT = 'Credit'
+    DEBIT = 'Debit'
 
-@dataclasses.dataclass
-class GetAccountRequest:
-    account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+class BankAccount:
+    r"""> **Accessing Bank Accounts through Banking API**
+    > 
+    > This datatype was originally used for accessing bank account data both in accounting integrations and open banking aggregators. 
+    > 
+    > To view bank account data through the Banking API, please refer to the new datatype [here](https://docs.codat.io/banking-api#/schemas/Account)
     
-class GetAccountSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-    PENDING = "Pending"
-
-class GetAccountSourceModifiedDateTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ASSET = "Asset"
-    EXPENSE = "Expense"
-    INCOME = "Income"
-    LIABILITY = "Liability"
-    EQUITY = "Equity"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountSourceModifiedDateValidDataTypeLinks:
-    r"""GetAccountSourceModifiedDateValidDataTypeLinks
-    When querying Codat's data model, some data types return `validDatatypeLinks` metadata in the JSON response. This indicates where that object can be used as a reference—a _valid link_—when creating or updating other data.
-    
-    For example, `validDatatypeLinks` might indicate the following references:
-    
-    - Which tax rates are valid to use on the line item of a bill.
-    - Which items can be used when creating an invoice. 
-    
-    You can use `validDatatypeLinks` to present your SMB customers with only valid choices when selecting objects from a list, for example.
-    
-    ## `validDatatypeLinks` example
-    
-    The following example uses the `Accounting.Accounts` data type. It shows that, on the linked integration, this account is valid as the account on a payment or bill payment; and as the account referenced on the line item of a direct income or direct cost. Because there is no valid link to Invoices or Bills, using this account on those data types will result in an error.
-    
-    ```json validDatatypeLinks for an account
-    {
-                \"id\": \"bd9e85e0-0478-433d-ae9f-0b3c4f04bfe4\",
-                \"nominalCode\": \"090\",
-                \"name\": \"Business Bank Account\",
-                #...
-                \"validDatatypeLinks\": [
-                    {
-                        \"property\": \"Id\",
-                        \"links\": [
-                            \"Payment.AccountRef.Id\",
-                            \"BillPayment.AccountRef.Id\",
-                            \"DirectIncome.LineItems.AccountRef.Id\",
-                            \"DirectCost.LineItems.AccountRef.Id\"
-                        ]
-                    }
-                ]
-            }
-    ```
+    > View the coverage for bank accounts in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankAccounts\" target=\"_blank\">Data coverage explorer</a>.
     
+    ## Overview
     
+    A list of bank accounts associated with a company and a specific data connection.
     
-    ## Support for `validDatatypeLinks`
+    Bank accounts data includes:
+    * The name and ID of the account in the accounting platform.
+    * The currency and balance of the account.
+    * The sort code and account number.
+    """
     
-    Codat currently supports `validDatatypeLinks` for some data types on our Xero, QuickBooks Online, QuickBooks Desktop, Exact (NL), and Sage Business Cloud integrations. 
+    account_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountName'), 'exclude': lambda f: f is None }})
+    r"""Name of the bank account in the accounting platform."""  
+    account_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountNumber'), 'exclude': lambda f: f is None }})
+    r"""Account number for the bank account.
+    
+    Xero integrations
+    Only a UK account number shows for bank accounts with GBP currency and a combined total of sort code and account number that equals 14 digits, For non-GBP accounts, the full bank account number is populated.
+    
+    FreeAgent integrations
+    For Credit accounts, only the last four digits are required. For other types, the field is optional.
+    """  
+    account_type: Optional[BankAccountBankAccountTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
+    r"""The type of transactions and balances on the account.
+    For Credit accounts, positive balances are liabilities, and positive transactions **reduce** liabilities.  
+    For Debit accounts, positive balances are assets, and positive transactions **increase** assets.
+    """  
+    available_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('availableBalance'), 'exclude': lambda f: f is None }})
+    r"""Total available balance of the bank account as reported by the underlying data source. This may take into account overdrafts or pending transactions for example."""  
+    balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+    r"""Balance of the bank account."""  
+    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
     
-    If you'd like us to extend support to more data types or integrations, suggest or vote for this on our <a href=\"https://portal.productboard.com/codat/5-product-roadmap\">Product Roadmap</a>.
-    """
+    ## Unknown currencies
     
-    links: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('links'), 'exclude': lambda f: f is None }})
-    property: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('property'), 'exclude': lambda f: f is None }})
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountSourceModifiedDate:
-    r"""GetAccountSourceModifiedDate
-    > **Language tip:** Accounts are also referred to as **chart of accounts**, **nominal accounts**, and **general ledger**.
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
+    i_ban: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iBan'), 'exclude': lambda f: f is None }})
+    r"""International bank account number of the account. Often used when making or receiving international payments."""  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the account, unique for the company in the accounting platform."""  
+    institution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('institution'), 'exclude': lambda f: f is None }})
+    r"""The institution of the bank account."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    Explore the <a className=\"external\" href=\"https://api.codat.io/swagger/index.html#/Accounts\" target=\"_blank\">Accounts</a> endpoints in Swagger.
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    View the coverage for accounts in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts\" target=\"_blank\">Data coverage explorer</a>.
     
-    ## Overview
     
-    Accounts are the categories a business uses to record accounting transactions. From the Accounts endpoints, you can retrieve [a list of all accounts for a specified company](https://api.codat.io/swagger/index.html#/Accounts/Accounts_List). 
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    The categories for an account include:
-      * Asset
-      * Expense
-      * Income
-      * Liability
-      * Equity.
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    > **Accounts with no category**
-    > 
-    > If an account is pulled from the chart of accounts and its nominal code does not lie within the category layout for the company's accounts, then the **type** is `Unknown`. The **fullyQualifiedCategory** and **fullyQualifiedName** fields return `null`.
+    > Time zones
     > 
-    > This approach gives a true representation of the company's accounts whilst preventing distorting financials such as a company's profit and loss and balance sheet reports.
-    """
-    
-    is_bank_account: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBankAccount') }})
-    status: GetAccountSourceModifiedDateStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    type: GetAccountSourceModifiedDateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    current_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentBalance'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    fully_qualified_category: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullyQualifiedCategory'), 'exclude': lambda f: f is None }})
-    fully_qualified_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullyQualifiedName'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetAccountSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
     nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    valid_datatype_links: Optional[list[GetAccountSourceModifiedDateValidDataTypeLinks]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validDatatypeLinks'), 'exclude': lambda f: f is None }})
+    r"""Code used to identify each nominal account for a business."""  
+    overdraft_limit: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overdraftLimit'), 'exclude': lambda f: f is None }})
+    r"""Pre-arranged overdraft limit of the account.
+    
+    The value is always positive. For example, an overdraftLimit of `1000` means that the balance of the account can go down to `-1000`.
+    """  
+    sort_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortCode'), 'exclude': lambda f: f is None }})
+    r"""Sort code for the bank account.
+    
+    Xero integrations
+    The sort code is only displayed when the currency = GBP and the sort code and account number sum to 14 digits. For non-GBP accounts, this field is not populated.
+    """  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclasses.dataclass
-class GetAccountResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetAccountSourceModifiedDate] = dataclasses.field(default=None)
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_accounts.py` & `codat-accounting-0.9.6/src/codat/models/shared/salesorder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,190 +1,195 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import addressesitems as shared_addressesitems
+from ..shared import customerref as shared_customerref
+from ..shared import metadata as shared_metadata
+from ..shared import salesorderinvoicestatus_enum as shared_salesorderinvoicestatus_enum
+from ..shared import salesorderlineitem as shared_salesorderlineitem
+from ..shared import salesorderstatus_enum as shared_salesorderstatus_enum
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetAccountsRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountsLinksLinksCurrent:
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})
+class SalesOrderShipToContact:
+    r"""Details of the named contact at the delivery address."""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinksLinksNext:
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    r"""Email address of the contact at the delivery address."""  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name of the contact at the delivery address."""  
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    r"""Phone number of the contact at the delivery address."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountsLinksLinksPrevious:
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+class SalesOrderShipTo:
+    r"""Delivery details for any goods that have been ordered."""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinksLinksSelf:
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})
+    address: Optional[shared_addressesitems.Addressesitems] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})  
+    contact: Optional[SalesOrderShipToContact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
+    r"""Details of the named contact at the delivery address."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountsLinksLinks:
-    current: GetAccountsLinksLinksCurrent = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-    self_: GetAccountsLinksLinksSelf = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-    next: Optional[GetAccountsLinksLinksNext] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[GetAccountsLinksLinksPrevious] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+class SalesOrder:
+    r"""> View the coverage for sales orders in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=salesOrders\\" target=\\"_blank\\">Data coverage explorer</a>.
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinksSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+    ## Overview
     
-class GetAccountsLinksSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-    PENDING = "Pending"
-
-class GetAccountsLinksSourceModifiedDateTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ASSET = "Asset"
-    EXPENSE = "Expense"
-    INCOME = "Income"
-    LIABILITY = "Liability"
-    EQUITY = "Equity"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinksSourceModifiedDateValidDataTypeLinks:
-    r"""GetAccountsLinksSourceModifiedDateValidDataTypeLinks
-    When querying Codat's data model, some data types return `validDatatypeLinks` metadata in the JSON response. This indicates where that object can be used as a reference—a _valid link_—when creating or updating other data.
+    A sales order represents a customer's intention to purchase goods or services from a seller and usually includes information such as the expected delivery date and shipping details. This information can be used to provide visibility on a business's expected receivables and to track sales through the full procurement process.
     
-    For example, `validDatatypeLinks` might indicate the following references:
+    A sales order is typically converted to an [invoice](https://docs.codat.io/accounting-api#/schemas/Invoice) after approval.
+    """
     
-    - Which tax rates are valid to use on the line item of a bill.
-    - Which items can be used when creating an invoice. 
+    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
     
-    You can use `validDatatypeLinks` to present your SMB customers with only valid choices when selecting objects from a list, for example.
+    ## Unknown currencies
     
-    ## `validDatatypeLinks` example
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
     
-    The following example uses the `Accounting.Accounts` data type. It shows that, on the linked integration, this account is valid as the account on a payment or bill payment; and as the account referenced on the line item of a direct income or direct cost. Because there is no valid link to Invoices or Bills, using this account on those data types will result in an error.
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
+    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
+    r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
     
-    ```json validDatatypeLinks for an account
-    {
-                \"id\": \"bd9e85e0-0478-433d-ae9f-0b3c4f04bfe4\",
-                \"nominalCode\": \"090\",
-                \"name\": \"Business Bank Account\",
-                #...
-                \"validDatatypeLinks\": [
-                    {
-                        \"property\": \"Id\",
-                        \"links\": [
-                            \"Payment.AccountRef.Id\",
-                            \"BillPayment.AccountRef.Id\",
-                            \"DirectIncome.LineItems.AccountRef.Id\",
-                            \"DirectCost.LineItems.AccountRef.Id\"
-                        ]
-                    }
-                ]
-            }
-    ```
+    Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
+    Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
     
+    For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
     
-    ## Support for `validDatatypeLinks`
+    ## Examples with base currency of GBP
     
-    Codat currently supports `validDatatypeLinks` for some data types on our Xero, QuickBooks Online, QuickBooks Desktop, Exact (NL), and Sage Business Cloud integrations. 
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **USD**          | $20            | 0.781         | £15.62                     |
+    | **EUR**          | €20            | 0.885         | £17.70                     |
+    | **RUB**          | ₽20            | 0.011         | £0.22                      |
     
-    If you'd like us to extend support to more data types or integrations, suggest or vote for this on our <a href=\"https://portal.productboard.com/codat/5-product-roadmap\">Product Roadmap</a>.
-    """
+    ## Examples with base currency of USD
     
-    links: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('links'), 'exclude': lambda f: f is None }})
-    property: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('property'), 'exclude': lambda f: f is None }})
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **GBP**          | £20            | 1.277         | $25.54                     |
+    | **EUR**          | €20            | 1.134         | $22.68                     |
+    | **RUB**          | ₽20            | 0.015         | $0.30                      |
+    """  
+    customer_purchase_order_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerPurchaseOrderNumber'), 'exclude': lambda f: f is None }})
+    r"""A customer-supplied identifier for the purchase order in the customer's system."""  
+    customer_ref: Optional[shared_customerref.CustomerRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerRef'), 'exclude': lambda f: f is None }})  
+    expected_delivery_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedDeliveryDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinksSourceModifiedDate:
-    r"""GetAccountsLinksSourceModifiedDate
-    > **Language tip:** Accounts are also referred to as **chart of accounts**, **nominal accounts**, and **general ledger**.
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    Explore the <a className=\"external\" href=\"https://api.codat.io/swagger/index.html#/Accounts\" target=\"_blank\">Accounts</a> endpoints in Swagger.
     
-    View the coverage for accounts in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts\" target=\"_blank\">Data coverage explorer</a>.
     
-    ## Overview
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    Accounts are the categories a business uses to record accounting transactions. From the Accounts endpoints, you can retrieve [a list of all accounts for a specified company](https://api.codat.io/swagger/index.html#/Accounts/Accounts_List). 
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the sales order, unique for the company in the accounting platform."""  
+    invoicing_status: Optional[shared_salesorderinvoicestatus_enum.SalesOrderInvoiceStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoicingStatus'), 'exclude': lambda f: f is None }})
+    r"""If the sales order is converted to an invoice, or will be in future, the invoicingStatus field indicates the current stage of the invoicing process."""  
+    issue_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    The categories for an account include:
-      * Asset
-      * Expense
-      * Income
-      * Liability
-      * Equity.
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    > **Accounts with no category**
+    > Time zones
     > 
-    > If an account is pulled from the chart of accounts and its nominal code does not lie within the category layout for the company's accounts, then the **type** is `Unknown`. The **fullyQualifiedCategory** and **fullyQualifiedName** fields return `null`.
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    line_items: Optional[list[shared_salesorderlineitem.SalesOrderLineItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lineItems'), 'exclude': lambda f: f is None }})
+    r"""An array of line items."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
     > 
-    > This approach gives a true representation of the company's accounts whilst preventing distorting financials such as a company's profit and loss and balance sheet reports.
-    """
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    note: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
+    r"""Any additional information associated with the sales order."""  
+    sales_order_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesOrderNumber'), 'exclude': lambda f: f is None }})
+    r"""Friendly reference for the sales order, commonly generated by the accounting platform."""  
+    ship_to: Optional[SalesOrderShipTo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipTo'), 'exclude': lambda f: f is None }})
+    r"""Delivery details for any goods that have been ordered."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    is_bank_account: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBankAccount') }})
-    status: GetAccountsLinksSourceModifiedDateStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    type: GetAccountsLinksSourceModifiedDateTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    current_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentBalance'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    fully_qualified_category: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullyQualifiedCategory'), 'exclude': lambda f: f is None }})
-    fully_qualified_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fullyQualifiedName'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetAccountsLinksSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    valid_datatype_links: Optional[list[GetAccountsLinksSourceModifiedDateValidDataTypeLinks]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validDatatypeLinks'), 'exclude': lambda f: f is None }})
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountsLinks:
-    r"""GetAccountsLinks
-    Codat's Paging Model
-    """
     
-    links: GetAccountsLinksLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[GetAccountsLinksSourceModifiedDate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
     
-
-@dataclasses.dataclass
-class GetAccountsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    links: Optional[GetAccountsLinks] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: Optional[shared_salesorderstatus_enum.SalesOrderStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    r"""Current state of the sales order."""  
+    sub_total: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subTotal'), 'exclude': lambda f: f is None }})
+    r"""Total amount of the sales order, including discounts but excluding tax."""  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Total amount of the sales order, including discounts and tax."""  
+    total_discount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalDiscount'), 'exclude': lambda f: f is None }})
+    r"""Total value of any discounts applied to the sales order."""  
+    total_tax_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxAmount'), 'exclude': lambda f: f is None }})
+    r"""Total amount of tax included in the sales order."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_aged_debtors_report.py` & `codat-accounting-0.9.6/src/codat/models/shared/billcreditnotelineitem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,68 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import accountref as shared_accountref
+from ..shared import billedtotype_enum as shared_billedtotype_enum
+from ..shared import customerref as shared_customerref
+from ..shared import itemref as shared_itemref
+from ..shared import projectref as shared_projectref
+from ..shared import taxrateref as shared_taxrateref
+from ..shared import trackingcategoryref as shared_trackingcategoryref
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date, datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetAgedDebtorsReportRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    number_of_periods: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'numberOfPeriods', 'style': 'form', 'explode': True }})
-    period_length_days: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'periodLengthDays', 'style': 'form', 'explode': True }})
-    report_date: Optional[date] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'reportDate', 'style': 'form', 'explode': True }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstandingAgedOutstandingAmountAmountsOutstandingByDataType:
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class BillCreditNoteLineItemTracking:
+    r"""Categories, and a project and customer, against which the item is tracked."""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstandingAgedOutstandingAmount:
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    details: Optional[list[GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstandingAgedOutstandingAmountAmountsOutstandingByDataType]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
-    from_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fromDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    to_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('toDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    category_refs: list[shared_trackingcategoryref.TrackingCategoryRef] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryRefs') }})  
+    is_billed_to: shared_billedtotype_enum.BilledToTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBilledTo') }})  
+    is_rebilled_to: shared_billedtotype_enum.BilledToTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isRebilledTo') }})  
+    customer_ref: Optional[shared_customerref.CustomerRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerRef'), 'exclude': lambda f: f is None }})  
+    project_ref: Optional[shared_projectref.ProjectRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('projectRef'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstanding:
-    aged_outstanding_amounts: Optional[list[GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstandingAgedOutstandingAmount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('agedOutstandingAmounts'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+class BillCreditNoteLineItem:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAgedDebtorsReportAgedDebtorsReportAgedDebtor:
-    aged_currency_outstanding: Optional[list[GetAgedDebtorsReportAgedDebtorsReportAgedDebtorAgedCurrencyOutstanding]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('agedCurrencyOutstanding'), 'exclude': lambda f: f is None }})
-    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerId'), 'exclude': lambda f: f is None }})
-    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAgedDebtorsReportAgedDebtorsReport:
-    data: Optional[list[GetAgedDebtorsReportAgedDebtorsReportAgedDebtor]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    generated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    report_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetAgedDebtorsReportResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    aged_debtors_report: Optional[GetAgedDebtorsReportAgedDebtorsReport] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
+    r"""Number of units of the goods or service for which credit has been received."""  
+    unit_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitAmount') }})
+    r"""Unit price of the goods or service."""  
+    account_ref: Optional[shared_accountref.AccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account."""  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Friendly name of each line item. For example, the goods or service for which credit has been received."""  
+    discount_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountAmount'), 'exclude': lambda f: f is None }})
+    r"""Value of any discounts applied."""  
+    discount_percentage: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountPercentage'), 'exclude': lambda f: f is None }})
+    r"""Percentage rate of any discount applied to the line item."""  
+    item_ref: Optional[shared_itemref.ItemRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemRef'), 'exclude': lambda f: f is None }})  
+    sub_total: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subTotal'), 'exclude': lambda f: f is None }})
+    r"""Amount of credit associated with the line item, including discounts but excluding tax."""  
+    tax_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount'), 'exclude': lambda f: f is None }})
+    r"""Amount of tax associated with the line item."""  
+    tax_rate_ref: Optional[shared_taxrateref.TaxRateRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference a tax rate, for example invoice and bill line items, use a taxRateRef that includes the ID and name of the linked tax rate.
+    
+    Found on:
+    
+    - Bill line items
+    - Bill Credit Note line items
+    - Credit Note line items
+    - Direct incomes line items
+    - Invoice line items
+    - Items
+    """  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Total amount of the line item, including discounts and tax."""  
+    tracking: Optional[BillCreditNoteLineItemTracking] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking'), 'exclude': lambda f: f is None }})
+    r"""Categories, and a project and customer, against which the item is tracked."""  
+    tracking_category_refs: Optional[list[shared_trackingcategoryref.TrackingCategoryRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategoryRefs'), 'exclude': lambda f: f is None }})
+    r"""Reference to the tracking categories to which the line item is linked."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_all_bank_account.py` & `codat-accounting-0.9.6/src/codat/models/shared/billlineitem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,57 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import accountref as shared_accountref
+from ..shared import itemref as shared_itemref
+from ..shared import propertiestracking as shared_propertiestracking
+from ..shared import taxrateref as shared_taxrateref
+from ..shared import trackingcategoryref as shared_trackingcategoryref
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetAllBankAccountRequest:
-    account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllBankAccount200ApplicationJSON:
-    account_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountName'), 'exclude': lambda f: f is None }})
-    account_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountNumber'), 'exclude': lambda f: f is None }})
-    available_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('availableBalance'), 'exclude': lambda f: f is None }})
-    balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    from_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fromDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    iban: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iban'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    institution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('institution'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    overdraft_limit: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overdraftLimit'), 'exclude': lambda f: f is None }})
-    sort_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortCode'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    to_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('toDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class BillLineItem:
     
-
-@dataclasses.dataclass
-class GetAllBankAccountResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_all_bank_account_200_application_json_object: Optional[GetAllBankAccount200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
+    r"""Number of units of goods or services received."""  
+    unit_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitAmount') }})
+    r"""Price of each unit of goods or services."""  
+    account_ref: Optional[shared_accountref.AccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account."""  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Friendly name of the goods or services received."""  
+    discount_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountAmount'), 'exclude': lambda f: f is None }})
+    r"""Numerical value of any discounts applied.
+    
+    Do not use to apply discounts in Oracle NetSuite—see Oracle NetSuite integration reference.
+    """  
+    discount_percentage: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountPercentage'), 'exclude': lambda f: f is None }})  
+    is_direct_cost: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDirectCost'), 'exclude': lambda f: f is None }})  
+    item_ref: Optional[shared_itemref.ItemRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemRef'), 'exclude': lambda f: f is None }})  
+    sub_total: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subTotal'), 'exclude': lambda f: f is None }})
+    r"""Amount of the line, inclusive of discounts but exclusive of tax."""  
+    tax_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount'), 'exclude': lambda f: f is None }})
+    r"""Amount of tax for the line."""  
+    tax_rate_ref: Optional[shared_taxrateref.TaxRateRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference a tax rate, for example invoice and bill line items, use a taxRateRef that includes the ID and name of the linked tax rate.
+    
+    Found on:
+    
+    - Bill line items
+    - Bill Credit Note line items
+    - Credit Note line items
+    - Direct incomes line items
+    - Invoice line items
+    - Items
+    """  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Total amount of the line, including tax."""  
+    tracking: Optional[shared_propertiestracking.Propertiestracking] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking'), 'exclude': lambda f: f is None }})
+    r"""Categories, and a project and customer, against which the item is tracked."""  
+    tracking_category_refs: Optional[list[shared_trackingcategoryref.TrackingCategoryRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategoryRefs'), 'exclude': lambda f: f is None }})
+    r"""Collection of categories against which this item is tracked."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_bank_account.py` & `codat-accounting-0.9.6/src/codat/models/shared/creditnotelineitem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,69 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import accountref as shared_accountref
+from ..shared import billedtotype_enum1 as shared_billedtotype_enum1
+from ..shared import customerref as shared_customerref
+from ..shared import itemref as shared_itemref
+from ..shared import projectref as shared_projectref
+from ..shared import taxrateref as shared_taxrateref
+from ..shared import trackingcategoryref as shared_trackingcategoryref
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetBankAccountRequest:
-    account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    
-class GetBankAccountSourceModifiedDateAccountTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    CREDIT = "Credit"
-    DEBIT = "Debit"
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBankAccountSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+class CreditNoteLineItemTracking:
+    r"""Categories, and a project and customer, against which the item is tracked."""
+    
+    category_refs: list[shared_trackingcategoryref.TrackingCategoryRef] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categoryRefs') }})  
+    is_billed_to: shared_billedtotype_enum1.BilledToTypeEnum1 = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBilledTo') }})  
+    is_rebilled_to: shared_billedtotype_enum1.BilledToTypeEnum1 = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isRebilledTo') }})  
+    customer_ref: Optional[shared_customerref.CustomerRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerRef'), 'exclude': lambda f: f is None }})  
+    project_ref: Optional[shared_projectref.ProjectRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('projectRef'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBankAccountSourceModifiedDate:
-    r"""GetBankAccountSourceModifiedDate
-    > **Accessing Bank Accounts through Banking API**
-    > 
-    > This datatype was originally used for accessing bank account data both in accounting integrations and open banking aggregators. 
-    > 
-    > To view bank account data through the Banking API, please refer to the new datatype [here](https://docs.codat.io/banking-api#/schemas/Account)
-    
-    > View the coverage for bank accounts in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankAccounts\" target=\"_blank\">Data coverage explorer</a>.
+class CreditNoteLineItem:
     
-    ## Overview
-    
-    A list of bank accounts associated with a company and a specific [data connection](https://api.codat.io/swagger/index.html#/Connection/get_companies__companyId__connections__connectionId_).
-    
-    Bank accounts data includes:
-    * The name and ID of the account in the accounting platform.
-    * The currency and balance of the account.
-    * The sort code and account number.
-    """
-    
-    account_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountName'), 'exclude': lambda f: f is None }})
-    account_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountNumber'), 'exclude': lambda f: f is None }})
-    account_type: Optional[GetBankAccountSourceModifiedDateAccountTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
-    available_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('availableBalance'), 'exclude': lambda f: f is None }})
-    balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    i_ban: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iBan'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    institution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('institution'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetBankAccountSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})
-    overdraft_limit: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overdraftLimit'), 'exclude': lambda f: f is None }})
-    sort_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortCode'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetBankAccountResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetBankAccountSourceModifiedDate] = dataclasses.field(default=None)
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
+    r"""Number of units of the goods or service for which credit has been issued."""  
+    unit_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitAmount') }})
+    r"""Unit price of the goods or service."""  
+    account_ref: Optional[shared_accountref.AccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account."""  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Friendly name of each line item. For example, the goods or service for which credit has been issued."""  
+    discount_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountAmount'), 'exclude': lambda f: f is None }})
+    r"""Value of any discounts applied."""  
+    discount_percentage: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discountPercentage'), 'exclude': lambda f: f is None }})
+    r"""Percentage rate of any discount applied to the line item."""  
+    is_direct_income: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDirectIncome'), 'exclude': lambda f: f is None }})  
+    item_ref: Optional[shared_itemref.ItemRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemRef'), 'exclude': lambda f: f is None }})  
+    sub_total: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subTotal'), 'exclude': lambda f: f is None }})
+    r"""Amount of credit associated with the line item, including discounts but excluding tax."""  
+    tax_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount'), 'exclude': lambda f: f is None }})
+    r"""Amount of tax associated with the line item."""  
+    tax_rate_ref: Optional[shared_taxrateref.TaxRateRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxRateRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference a tax rate, for example invoice and bill line items, use a taxRateRef that includes the ID and name of the linked tax rate.
+    
+    Found on:
+    
+    - Bill line items
+    - Bill Credit Note line items
+    - Credit Note line items
+    - Direct incomes line items
+    - Invoice line items
+    - Items
+    """  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Total amount of the line item, including discounts and tax."""  
+    tracking: Optional[CreditNoteLineItemTracking] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking'), 'exclude': lambda f: f is None }})
+    r"""Categories, and a project and customer, against which the item is tracked."""  
+    tracking_category_refs: Optional[list[shared_trackingcategoryref.TrackingCategoryRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategoryRefs'), 'exclude': lambda f: f is None }})
+    r"""Reference to the tracking categories to which the line item is linked."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_bill_attachment.py` & `codat-accounting-0.9.6/src/codat/models/shared/addressesitems.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,29 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import addresstype_enum as shared_addresstype_enum
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetBillAttachmentRequest:
-    attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    bill_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBillAttachmentAttachment:
-    content_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentType'), 'exclude': lambda f: f is None }})
-    date_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dateCreated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    include_when_sent: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('includeWhenSent'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class Addressesitems:
     
-
-@dataclasses.dataclass
-class GetBillAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    attachment: Optional[GetBillAttachmentAttachment] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    type: shared_addresstype_enum.AddressTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""The type of the address"""  
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    r"""City of the customer address."""  
+    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    r"""Country of the customer address."""  
+    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
+    r"""Line 1 of the customer address."""  
+    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
+    r"""Line 2 of the customer address."""  
+    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
+    r"""Postal code or zip code."""  
+    region: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
+    r"""Region of the customer address."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_bill_payments.py` & `codat-accounting-0.9.6/src/codat/models/shared/billpayment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,42 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import accountref as shared_accountref
+from ..shared import billpaymentline as shared_billpaymentline
+from ..shared import metadata as shared_metadata
+from ..shared import paymentmethodref as shared_paymentmethodref
+from ..shared import supplementaldata as shared_supplementaldata
+from ..shared import supplierref as shared_supplierref
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
-from typing import Any, Optional
-
-
-@dataclasses.dataclass
-class GetBillPaymentsRequest:
-    bill_payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billPaymentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateAccountRef:
-    r"""GetBillPaymentsSourceModifiedDateAccountRef
-    Account the payment is linked to in the accounting platform.
-    """
-    
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
-class GetBillPaymentsSourceModifiedDateLinesLinksTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    UNLINKED = "Unlinked"
-    BILL = "Bill"
-    OTHER = "Other"
-    CREDIT_NOTE = "CreditNote"
-    BILL_PAYMENT = "BillPayment"
-    PAYMENT_ON_ACCOUNT = "PaymentOnAccount"
-    REFUND = "Refund"
-    MANUAL_JOURNAL = "ManualJournal"
-    DISCOUNT = "Discount"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateLinesLinks:
-    type: GetBillPaymentsSourceModifiedDateLinesLinksTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateLines:
-    amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    allocated_on_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allocatedOnDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    links: Optional[list[GetBillPaymentsSourceModifiedDateLinesLinks]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('links'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDatePaymentMethodRef:
-    r"""GetBillPaymentsSourceModifiedDatePaymentMethodRef
-    The Payment Method to which the payment is linked in the accounting platform.
-    """
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
+from typing import Optional
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateSupplementalData:
-    r"""GetBillPaymentsSourceModifiedDateSupplementalData
-    Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more.
-    """
-    
-    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDateSupplierRef:
-    r"""GetBillPaymentsSourceModifiedDateSupplierRef
-    Supplier against which the payment is recorded in the accounting platform.
-    """
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    supplier_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierName'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBillPaymentsSourceModifiedDate:
-    r"""GetBillPaymentsSourceModifiedDate
-    > **Bill payments or payments?**  
+class BillPayment:
+    r"""> **Bill payments or payments?**
     > 
     > In Codat, bill payments represent accounts payable only. For accounts receivable, see [payments](https://docs.codat.io/accounting-api#/schemas/Payment), which includes [invoices](https://docs.codat.io/accounting-api#/schemas/Invoice) and [credit notes](https://docs.codat.io/accounting-api#/schemas/CreditNote).
     
     > View the coverage for bill payments in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=billPayments\" target=\"_blank\">Data coverage explorer</a>.
     
     ## Overview
     
     Bill payments include all accounts payable transaction data. This includes [bills](https://docs.codat.io/accounting-api#/schemas/Bill) and [credit notes against bills](https://docs.codat.io/accounting-api#/schemas/BillCreditNote).
     
-    A bill payment in Codat usually represents an allocation of money within any customer accounts payable account. This includes but is not strictly limited to:
+    A bill payment in Codat usually represents an allocation of money within any customer accounts payable account. This includes, but is not strictly limited to:
     
-    - A payment made against a bill—for example, a credit card payment, cheque payment, or cash payment.
-    - An allocation of a supplier's credit note, to a bill or perhaps a refund.
+    - A payment made against a bill — for example, a credit card payment, cheque payment, or cash payment.
+    - An allocation of a supplier's credit note to a bill or perhaps a refund.
     - A bill payment made directly to an accounts payable account. This could be an overpayment or a prepayment, or a refund of a payment made directly to an accounts payable account.
     
-    Depending on the bill payments which are allowed by the underlying accounting package, some of these types may be combined. Please see the [Example data](#example-data) section for samples of what these cases look like.
+    Depending on the bill payments which are allowed by the underlying accounting package, some of these types may be combined. Please see the example data section for samples of what these cases look like.
     
     In Codat, a bill payment contains details of:
     
     - When the bill payment was recorded in the accounting system.
     - How much it is for and in the currency.
     - Who the payment has been paid to, the _supplier_.
     - The types of bill payments, the _line items_.  
@@ -127,80 +45,80 @@
     
     Bill payments is a child data type of [account transactions](https://docs.codat.io/accounting-api#/schemas/AccountTransaction).
     
     ---
     
     ## Bill payment types
     
-    ## Payment of a bill
+    ### Payment of a bill
     
     A payment paying a single bill should have the following properties:
     
     - A `totalAmount` indicating the amount of the bill that was paid. This is always positive.
     - A `lines` array containing one element with the following properties:
       - An `amount` equal to the `totalAmount` above.
       - A `links` array containing one element with the following properties:
         - A `type` indicating the type of link, in this case a `Bill`.
         - An `id` containing the ID of the bill that was paid.
         - An amount of `-totalAmount` (negative `totalAmount`), indicating that the entirety of the paid amount is allocated to the bill.
     
-    ## Payment of multiple bills
+    ### Payment of multiple bills
     
     It is possible for one payment to pay multiple bills. This can be represented using two possible formats, depending on how the supplier keeps their books:
     
     1. The payment has multiple entries in its **lines** array, one for each bill that is paid. Each line will follow the above example for paying a bill, and the rules detailed in the data model.
     2. The payment has a line with multiple links to each bill. This occurs when the proportion of the original payment allocated to each bill is not available.
     
     Each line is the same as those described above, with the **amount** indicating how much of the payment is allocated to the bill. The **amount** on the lines sum to the **totalAmount** on the payment.
     
-    > 🚧 Pushing batch payments to Xero
+    > Pushing batch payments to Xero
     > 
     > When pushing a single bill payment to Xero to pay multiple bills, only the first format is supported—multiple entries in the payment **lines** array.
     
-    ## Payments and refunds on account
+    ### Payments and refunds on account
     
     A payment on account, that is a payment that doesn’t pay a specific bill, has one entry in its lines array.
     
     The line has the following properties:
     
     - A **totalAmount** indicating the amount paid by a supplier or refunded to them by a company. A payment to the supplier is always negative. A refund is always positive.
     - A **links** array containing one element with the following properties:
       - A **type** indicating the type of link. For a payment this is `PaymentOnAccount`. For a refund this is `Refund`.
       - The **id** containing the ID of the supplier.
       - An amount for the link is `0` **totalAmount** or the amount of the payment or refund.
     
     It is possible to have a payment that is part on account and part allocated to a bill. Each line should follow the examples above.
     
-    ## Using a credit note to pay a bill
+    ### Using a credit note to pay a bill
     
     The payment of a bill using a credit note has one entry in its `lines` array. This **line** has the following properties:
     
     - An **amount** indicating the amount of money moved, which in this case is `0`, as the credit note and bill allocation must balance each other.
     - A **links** array containing two elements:
       - The first link has:
         - A **type** indicating the type of link, in this case a `Bill`.
         - An **id** containing the ID of the bill that was paid.
       - The second link has:
         - A **type** indicating the type of link, in this case a `CreditNote`.
         - An **id** containing the ID of the credit note used by this payment.
     
     The **amount** field on the **line** equals the **totalAmount** on the payment.
     
-    ## Refunding a credit note
+    ### Refunding a credit note
     
     A bill payment refunding a credit note has one entry in its **lines** array. This line has the following properties:
     
     - An **amount** indicating the amount of the credit note that was refunded. This is always negative, indicating that it is a refund.
     - A **links** array containing one element with the following properties:
       - A **type** indicating the type of `link`, in this case a `CreditNote`.
       - An **id** containing the ID of the credit note that was refunded.
     
     The **totalAmount** field on the payment equals the line's **amount** field. These are both negative, as this is money leaving accounts payable.
     
-    ## Refunding a payment
+    ### Refunding a payment
     
     If a payment is refunded, for example, when a company overpaid a bill and the overpayment is returned, there are two payment records: 
     
     - One for the incoming overpayment.
     - Another for the outgoing refund.
     
     The payment issuing the refund is identified by the fact that the **totalAmount** is negative. This payment has one entry in its lines array that have the following properties:
@@ -220,15 +138,15 @@
     The line linked to the bill payment has the following properties:
     
     - An **amount** indicating the amount that was refunded. This is positive as its money that was added to accounts payable, but is balanced out by the negative amount of the refund.
     - A **links** array containing one element with the following properties:
       - A **type** indicating the type of the link, in this case a `Refund`.
       - An **id** containing the ID of the payment that refunded this line.
     
-    > 📘 Linked payments
+    > Linked payments
     > 
     > Not all accounting packages support linked payments in this way. In these platforms you may see a payment on account and a refund on account.
     
     ## Foreign currencies
     
     There are two types of currency rate that are detailed in the bill payments data type: 
     
@@ -242,34 +160,125 @@
     - Base currency of the item that the link represents.
     - Foreign currency of the payment.
     
     These two rates allow the calculation of currency loss or gain for any of the transactions affected by the payment lines. The second rate is used when a bill payment is applied to an item in a currency that does not match either:
     
     - The base currency for the accounts payable account. 
     - The currency of the item.
-    
     """
     
-    date_: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    account_ref: Optional[GetBillPaymentsSourceModifiedDateAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    date_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    account_ref: Optional[shared_accountref.AccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account."""  
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
+    
+    ## Unknown currencies
+    
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
+    
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
+    r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
+    
+    Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
+    
+    Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
+    
+    For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
+    
+    ## Examples with base currency of GBP
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **USD**          | $20            | 0.781         | £15.62                     |
+    | **EUR**          | €20            | 0.885         | £17.70                     |
+    | **RUB**          | ₽20            | 0.011         | £0.22                      |
+    
+    ## Examples with base currency of USD
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **GBP**          | £20            | 1.277         | $25.54                     |
+    | **EUR**          | €20            | 1.134         | $22.68                     |
+    | **RUB**          | ₽20            | 0.015         | $0.30                      |
+    """  
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    lines: Optional[list[GetBillPaymentsSourceModifiedDateLines]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetBillPaymentsSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the bill payment, unique for the company in the accounting platform."""  
+    lines: Optional[list[shared_billpaymentline.BillPaymentLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
+    r"""An array of bill payment lines."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
     note: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
-    payment_method_ref: Optional[GetBillPaymentsSourceModifiedDatePaymentMethodRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('paymentMethodRef'), 'exclude': lambda f: f is None }})
+    r"""Additional information associated with the payment."""  
+    payment_method_ref: Optional[shared_paymentmethodref.PaymentMethodRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('paymentMethodRef'), 'exclude': lambda f: f is None }})  
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    supplemental_data: Optional[GetBillPaymentsSourceModifiedDateSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
-    supplier_ref: Optional[GetBillPaymentsSourceModifiedDateSupplierRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierRef'), 'exclude': lambda f: f is None }})
-    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Additional information associated with the payment."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclasses.dataclass
-class GetBillPaymentsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetBillPaymentsSourceModifiedDate] = dataclasses.field(default=None)
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    supplemental_data: Optional[shared_supplementaldata.SupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""  
+    supplier_ref: Optional[shared_supplierref.SupplierRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierRef'), 'exclude': lambda f: f is None }})
+    r"""Reference to the supplier the record relates to."""  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Amount of the payment in the payment currency. This value never changes and represents the amount of money that is paid into the supplier's account."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_cash_flow_statement.py` & `codat-accounting-0.9.6/src/codat/models/operations/put_supplier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,109 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
+from ..shared import datatype_enum as shared_datatype_enum
+from ..shared import pushoperationchange as shared_pushoperationchange
+from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
+from ..shared import supplier as shared_supplier
+from ..shared import validation as shared_validation
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetCashFlowStatementRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    period_length: int = dataclasses.field(metadata={'query_param': { 'field_name': 'periodLength', 'style': 'form', 'explode': True }})
-    periods_to_compare: int = dataclasses.field(metadata={'query_param': { 'field_name': 'periodsToCompare', 'style': 'form', 'explode': True }})
-    start_month: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'startMonth', 'style': 'form', 'explode': True }})
-    
-class GetCashFlowStatement200ApplicationJSONReportBasisEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACCRUAL = "Accrual"
-    CASH = "Cash"
-
-class GetCashFlowStatement200ApplicationJSONReportInputEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    INDIRECT = "Indirect"
-    DIRECT = "Direct"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLineReportLineReportLine:
-    value: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class PutSupplierRequest:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLineReportLine:
-    value: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    items: Optional[list[GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLineReportLineReportLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    supplier_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'supplierId', 'style': 'simple', 'explode': False }})
+    r"""Unique identifier for a supplier"""  
+    force_update: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'forceUpdate', 'style': 'form', 'explode': True }})  
+    supplier: Optional[shared_supplier.Supplier] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeoutInMinutes', 'style': 'form', 'explode': True }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLine:
-    value: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    items: Optional[list[GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLineReportLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class PutSupplier200ApplicationJSON:
+    r"""Success"""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLine:
-    r"""GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLine
-    ReportLines for cash payments to suppliers for the purchase of goods or services.
-    """
-    
-    value: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    items: Optional[list[GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLineReportLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('items'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
+    r"""Unique identifier for your SMB in Codat."""  
+    data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
+    r"""Unique identifier for a company's data connection."""  
+    push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
+    r"""A unique identifier generated by Codat to represent this single push operation. This identifier can be used to track the status of the push, and should be persisted."""  
+    requested_on_utc: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSONCashFlowStatement:
-    r"""GetCashFlowStatement200ApplicationJSONCashFlowStatement
-    > View the coverage for cash flow statement in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=cashFlowStatement\" target=\"_blank\">Data coverage explorer</a>.
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    > ** Operating activities only**  
+    > Time zones
     > 
-    > Currently, the cash flow statement shows cash that flows into and out of the company from operating activities *only*. Operating activities generate cash from the sale of goods or services.
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: shared_pushoperationstatus_enum.PushOperationStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The status of the push operation."""  
+    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})  
+    changes: Optional[list[shared_pushoperationchange.PushOperationChange]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})  
+    completed_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
     
-    ## Overview
     
-    A cash flow statement is a financial report that records all cash that is received or spent by a company during a given period. It gives you a clearer picture of the company’s performance, and their ability to pay creditors and finance growth.
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    > **Cash flow statement or balance sheet?**
+    > Time zones
     > 
-    > Look at the cash flow statement to understand a company's ability to pay its bills. Although the balance sheet may show healthy earnings at a specific point in time, the cash flow statement allows you to see whether the company is meeting its financial commitments, such as paying creditors or its employees.
-    """
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    data: Optional[shared_supplier.Supplier] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    r"""> View the coverage for suppliers in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers\\" target=\\"_blank\\">Data coverage explorer</a>.
     
-    cash_payments: Optional[GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLine] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cashPayments'), 'exclude': lambda f: f is None }})
-    cash_receipts: Optional[GetCashFlowStatement200ApplicationJSONCashFlowStatementReportLine] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cashReceipts'), 'exclude': lambda f: f is None }})
-    from_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fromDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    to_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('toDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    ## Overview
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCashFlowStatement200ApplicationJSON:
-    currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-    report_basis: GetCashFlowStatement200ApplicationJSONReportBasisEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportBasis') }})
-    report_input: GetCashFlowStatement200ApplicationJSONReportInputEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportInput') }})
-    reports: list[GetCashFlowStatement200ApplicationJSONCashFlowStatement] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reports') }})
-    earliest_available_month: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('earliestAvailableMonth'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    most_recent_available_month: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mostRecentAvailableMonth'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    From the **Suppliers** endpoints, you can retrieve a list of [all the suppliers for a company](https://docs.codat.io/accounting-api#/operations/list-suppliers). Suppliers' data links to accounts payable [bills](https://docs.codat.io/accounting-api#/schemas/Bill).
+    """  
+    data_type: Optional[shared_datatype_enum.DataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})  
+    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_validation.Validation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here."""  
     
 
 @dataclasses.dataclass
-class GetCashFlowStatementResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_cash_flow_statement_200_application_json_object: Optional[GetCashFlowStatement200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class PutSupplierResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    put_supplier_200_application_json_object: Optional[PutSupplier200ApplicationJSON] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_create_update_accounttransactions_model.py` & `codat-accounting-0.9.6/src/codat/models/shared/createbanktransactionsresponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,97 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import banktransactions as shared_banktransactions
+from ..shared import datatype_enum as shared_datatype_enum
+from ..shared import pushoperationchange as shared_pushoperationchange
+from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
+from ..shared import validation as shared_validation
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelRequest:
-    account_transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountTransactionId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDateBankAccountRef:
-    r"""GetCreateUpdateAccountTransactionsModelSourceModifiedDateBankAccountRef
-    Reference to the bank account the account transaction is recorded against.
-    """
+class CreateBankTransactionsResponse:
+    r"""Success"""
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
+    r"""Unique identifier for your SMB in Codat."""  
+    data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
+    r"""Unique identifier for a company's data connection."""  
+    push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
+    r"""A unique identifier generated by Codat to represent this single push operation. This identifier can be used to track the status of the push, and should be persisted."""  
+    requested_on_utc: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDateLinesRecordRef:
-    r"""GetCreateUpdateAccountTransactionsModelSourceModifiedDateLinesRecordRef
-    Links an account transaction line to the underlying record that created it.
-    """
-    
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDateLines:
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    record_ref: Optional[GetCreateUpdateAccountTransactionsModelSourceModifiedDateLinesRecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRef'), 'exclude': lambda f: f is None }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: shared_pushoperationstatus_enum.PushOperationStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The status of the push operation."""  
+    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})  
+    changes: Optional[list[shared_pushoperationchange.PushOperationChange]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})  
+    completed_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    UNRECONCILED = "Unreconciled"
-    RECONCILED = "Reconciled"
-    VOID = "Void"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelSourceModifiedDate:
-    r"""GetCreateUpdateAccountTransactionsModelSourceModifiedDate
-    > **Language tip:** In Codat, account transactions represent all transactions posted to a bank account within an accounting platform. For bank transactions posted within a banking platform, refer to [Banking transactions](https://docs.codat.io/banking-api#/operations/list-all-banking-transactions).
     
-    > View the coverage for account transactions in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=accountTransactions\" target=\"_blank\">Data coverage explorer</a>.
     
-    ## Overview
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    data: Optional[shared_banktransactions.BankTransactions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    r"""> **Accessing Bank Accounts through Banking API**
+    > 
+    > This datatype was originally used for accessing bank account data both in accounting integrations and open banking aggregators. 
+    >
+    > To view bank account data through the Banking API, please refer to the new datatype [here](https://docs.codat.io/banking-api#/operations/list-all-banking-transactions)
     
-    In Codat’s data model, account transactions represent bank activity within an accounting platform. All transactions that go through a bank account are recorded as account transactions.
+    > View the coverage for bank transactions in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankTransactions\" target=\"_blank\">Data coverage explorer</a>.
     
-    Account transactions are created as a result of different business activities, for example:
+    ## Overview
     
-    * Payments: for example, receiving money for payment against an invoice.
-    * Bill payments: for example, spending money for a payment against a bill.
-    * Direct costs: for example, withdrawing money from a bank account, either for cash purposes or to make a payment.
-    * Direct incomes: for example, selling an item directly to a contact and receiving payment at point of sale.
-    * Transfers: for example, transferring money between two bank accounts.
-    
-    Account transactions is the parent data type of [payments](https://docs.codat.io/accounting-api#/schemas/Payment), [bill payments](https://docs.codat.io/accounting-api#/schemas/BillPayment), [direct costs](https://docs.codat.io/accounting-api#/schemas/DirectCost), [direct incomes](https://docs.codat.io/accounting-api#/schemas/DirectIncome), and [transfers](https://docs.codat.io/accounting-api#/schemas/Transfer).
-    """
-    
-    bank_account_ref: Optional[GetCreateUpdateAccountTransactionsModelSourceModifiedDateBankAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bankAccountRef'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
-    date_: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    lines: Optional[list[GetCreateUpdateAccountTransactionsModelSourceModifiedDateLines]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetCreateUpdateAccountTransactionsModelSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    note: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status: Optional[GetCreateUpdateAccountTransactionsModelSourceModifiedDateStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
-    transaction_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactionId'), 'exclude': lambda f: f is None }})
+    Transactional banking data for a specific company and account.
     
-
-@dataclasses.dataclass
-class GetCreateUpdateAccountTransactionsModelResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetCreateUpdateAccountTransactionsModelSourceModifiedDate] = dataclasses.field(default=None)
+    Bank transactions include the:
+    * Amount of the transaction.
+    * Current account balance.
+    * Transaction type, for example, credit, debit, or transfer.
+    """  
+    data_type: Optional[shared_datatype_enum.DataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})  
+    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_validation.Validation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_customer_attachment.py` & `codat-accounting-0.9.6/src/codat/models/shared/pushoptionproperty.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,24 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import pushoptionchoice as shared_pushoptionchoice
+from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
+from ..shared import pushvalidationinfo as shared_pushvalidationinfo
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetCustomerAttachmentRequest:
-    attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customerId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCustomerAttachmentAttachment:
-    content_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentType'), 'exclude': lambda f: f is None }})
-    date_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dateCreated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    include_when_sent: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('includeWhenSent'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class PushOptionProperty:
     
-
-@dataclasses.dataclass
-class GetCustomerAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    attachment: Optional[GetCustomerAttachmentAttachment] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})  
+    display_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayName') }})  
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})  
+    type: shared_pushoptiontype_enum.PushOptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    options: Optional[list[shared_pushoptionchoice.PushOptionChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})  
+    properties: Optional[dict[str, PushOptionProperty]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_pushvalidationinfo.PushValidationInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_direct_cost_attachment.py` & `codat-accounting-0.9.6/src/codat/models/shared/pushoption.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,26 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import pushoptionchoice as shared_pushoptionchoice
+from ..shared import pushoptionproperty as shared_pushoptionproperty
+from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
+from ..shared import pushvalidationinfo as shared_pushvalidationinfo
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetDirectCostAttachmentRequest:
-    attachment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'attachmentId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    direct_cost_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directCostId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDirectCostAttachmentAttachment:
-    content_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentType'), 'exclude': lambda f: f is None }})
-    date_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dateCreated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    include_when_sent: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('includeWhenSent'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class PushOption:
+    r"""OK"""
     
-
-@dataclasses.dataclass
-class GetDirectCostAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    attachment: Optional[GetDirectCostAttachmentAttachment] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    display_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayName') }})  
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})  
+    type: shared_pushoptiontype_enum.PushOptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    options: Optional[list[shared_pushoptionchoice.PushOptionChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})  
+    properties: Optional[dict[str, shared_pushoptionproperty.PushOptionProperty]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_pushvalidationinfo.PushValidationInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_invoice_pdf.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_create_update_purchaseorders_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import pushoption as shared_pushoption
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetInvoicePdfRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    invoice_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'invoiceId', 'style': 'simple', 'explode': False }})
+class GetCreateUpdatePurchaseOrdersModelRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetInvoicePdfResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetCreateUpdatePurchaseOrdersModelResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    push_option: Optional[shared_pushoption.PushOption] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_journal.py` & `codat-accounting-0.9.6/src/codat/models/shared/createtransferresponse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,84 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import datatype_enum as shared_datatype_enum
+from ..shared import pushoperationchange as shared_pushoperationchange
+from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
+from ..shared import transfer as shared_transfer
+from ..shared import validation as shared_validation
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetJournalRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    journal_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'journalId', 'style': 'simple', 'explode': False }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalSourceModifiedDateMetadataMetadata:
-    r"""GetJournalSourceModifiedDateMetadataMetadata
-    Additional information about the entity
-    """
-    
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalSourceModifiedDateMetadata:
-    metadata: Optional[GetJournalSourceModifiedDateMetadataMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    
-class GetJournalSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetJournalSourceModifiedDate:
-    r"""GetJournalSourceModifiedDate
-    > **Language tip:** For line items, or individual transactions, of a company's financial documents, refer to the [Journal entries](https://docs.codat.io/accounting-api#/schemas/JournalEntry) data type
+class CreateTransferResponse:
+    r"""Success"""
     
-    > View the coverage for journals in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journals\" target=\"_blank\">Data coverage explorer</a>.
-    
-    ## Overview
-    
-    In accounting software, journals are used to record all the financial transactions of a company. Each transaction in a journal is represented by a separate [journal entry](https://docs.codat.io/accounting-api#/schemas/JournalEntry). These entries are used to create the general ledger, which is then used to create the financial statements of a business.
-    
-    When a company records all their transactions in a single journal, it can become large and difficult to maintain and track. This is why large companies often use multiple journals (also known as subjournals) to categorize and manage journal entries.
-    
-    Such journals can be divided into two categories:
-    
-    - Special journals: journals used to record specific types of transactions; for example, a purchases journal, a sales journal, or a cash management journal.
-    - General journals: journals used to record transactions that fall outside the scope of the special journals.
-    
-    Multiple journals or subjournals are used in the following Codat integrations:
-    
-    - [Sage Intacct](https://docs.codat.io/integrations/accounting/sage-intacct/accounting-sage-intacct)  (mandatory)
-    - [Exact Online](https://docs.codat.io/integrations/accounting/exact-online/accounting-exact-online)  (mandatory)
-    - [Oracle NetSuite](https://docs.codat.io/integrations/accounting/netsuite/accounting-netsuite) (optional)
-    
-    > When pushing journal entries to an accounting platform that doesn’t support multiple journals (multi-book accounting), the entries will be linked to the platform-generic journal. The Journals data type will only include one object.
-    
-    """
-    
-    created_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    has_children: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasChildren'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    journal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('journalCode'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetJournalSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    parent_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentId'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status: Optional[GetJournalSourceModifiedDateStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetJournalResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetJournalSourceModifiedDate] = dataclasses.field(default=None)
+    company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
+    r"""Unique identifier for your SMB in Codat."""  
+    data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
+    r"""Unique identifier for a company's data connection."""  
+    push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
+    r"""A unique identifier generated by Codat to represent this single push operation. This identifier can be used to track the status of the push, and should be persisted."""  
+    requested_on_utc: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: shared_pushoperationstatus_enum.PushOperationStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The status of the push operation."""  
+    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})  
+    changes: Optional[list[shared_pushoperationchange.PushOperationChange]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})  
+    completed_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    data: Optional[shared_transfer.Transfer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    r"""> View the coverage for transfers in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=transfers\\" target=\\"_blank\\">Data coverage explorer</a>.
+    
+    A transfer records the movement of money between two bank accounts, or between a bank account and a nominal account. It is a child data type of [account transactions](https://docs.codat.io/accounting-api#/schemas/AccountTransaction).
+    """  
+    data_type: Optional[shared_datatype_enum.DataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})  
+    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_validation.Validation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_journal_entry.py` & `codat-accounting-0.9.6/src/codat/models/shared/companydataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,158 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import addresstype_enum as shared_addresstype_enum
+from ..shared import phonenumbertype_enum as shared_phonenumbertype_enum
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
-from typing import Any, Optional
-
+from enum import Enum
+from typing import Optional
 
-@dataclasses.dataclass
-class GetJournalEntryRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    journal_entry_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'journalEntryId', 'style': 'simple', 'explode': False }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateJournalLinesAccountRef:
-    r"""GetJournalEntrySourceModifiedDateJournalLinesAccountRef
-    Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account.
-    """
+class CompanyDatasetAddresses:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    type: shared_addresstype_enum.AddressTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""The type of the address"""  
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    r"""City of the customer address."""  
+    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    r"""Country of the customer address."""  
+    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
+    r"""Line 1 of the customer address."""  
+    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
+    r"""Line 2 of the customer address."""  
+    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
+    r"""Postal code or zip code."""  
+    region: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
+    r"""Region of the customer address."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateJournalLinesTracking:
-    r"""GetJournalEntrySourceModifiedDateJournalLinesTracking
-    List of record refs associated with the tracking information for the line (eg to a Tracking Category, or customer etc.)
-    """
+class CompanyDatasetPhone:
     
-    record_refs: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRefs'), 'exclude': lambda f: f is None }})
+    number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('number') }})
+    r"""A phone number."""  
+    type: shared_phonenumbertype_enum.PhoneNumberTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""The type of phone number"""  
     
+class CompanyDatasetWeblinkTypeEnum(str, Enum):
+    r"""The type of the weblink."""
+    WEBSITE = 'Website'
+    SOCIAL = 'Social'
+    UNKNOWN = 'Unknown'
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateJournalLines:
-    net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
-    account_ref: Optional[GetJournalEntrySourceModifiedDateJournalLinesAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    tracking: Optional[GetJournalEntrySourceModifiedDateJournalLinesTracking] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking'), 'exclude': lambda f: f is None }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateJournalRef:
-    r"""GetJournalEntrySourceModifiedDateJournalRef
-    Links journal entries to the relevant journal in accounting integrations that use multi-book accounting (multiple journals).
-    """
+class CompanyDatasetWeblink:
+    r"""Weblink associated with the company."""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    type: Optional[CompanyDatasetWeblinkTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    r"""The type of the weblink."""  
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
+    r"""The full URL for the weblink."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+class CompanyDataset:
+    r"""> View the coverage for company info in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=cashFlowStatement\\" target=\\"_blank\\">Data coverage explorer</a>.
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateRecordRef:
-    r"""GetJournalEntrySourceModifiedDateRecordRef
-    Links to the underlying record or data type.
-    
-    Found on:
-    
-    - Journal entries
-    - Account transactions
-    - Invoices
-    - Transfers
+    Company info provides standard details about a linked company such as their address, phone number, and company registration.
+    
+    > **Company information or companies?**
+    > 
+    > Company information is standard information that is held in the accounting platform about a company. `Companies` is an endpoint that lists businesses in the Codat system that have linked and shared their data sources.
     """
     
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    accounting_platform_ref: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountingPlatformRef'), 'exclude': lambda f: f is None }})
+    r"""Identifier or reference for the company in the accounting platform."""  
+    addresses: Optional[list[CompanyDatasetAddresses]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addresses'), 'exclude': lambda f: f is None }})
+    r"""An array of Addresses."""  
+    base_currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('baseCurrency'), 'exclude': lambda f: f is None }})
+    r"""Currency set in the accounting platform of the linked company. Used by the currency rate."""  
+    company_legal_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyLegalName'), 'exclude': lambda f: f is None }})
+    r"""Registered legal name of the linked company."""  
+    company_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyName'), 'exclude': lambda f: f is None }})
+    r"""Name of the linked company."""  
+    created_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalEntrySourceModifiedDateSupplementalData:
-    r"""GetJournalEntrySourceModifiedDateSupplementalData
-    Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more.
-    """
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetJournalEntrySourceModifiedDate:
-    r"""GetJournalEntrySourceModifiedDate
-    > **Language tip:** For the top-level record of a company's financial transactions, refer to the [Journals](https://docs.codat.io/accounting-api#/schemas/Journal) data type
     
-    > View the coverage for journal entries in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journalEntries\" target=\"_blank\">Data coverage explorer</a>.
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    ## Overview
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    A journal entry report shows the entries made in a company's general ledger, or [accounts](https://api.codat.io/swagger/index.html#/Accounts/get_companies__companyId__data_accounts), when transactions are approved. The journal line items for each journal entry should balance.
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    financial_year_start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('financialYearStartDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    A journal entry line item is a single transaction line on the journal entry. For example: 
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    - When a journal entry is recording a receipt of cash, the credit to accounts receivable and the debit to cash are separate line items. 
-    - When a company needs to recognise revenue from an annual contract on a monthly basis, on receipt of cash for month one, they make a debit to deferred income and a credit to revenue.
     
-    In Codat a journal entry contains details of:
     
-    - The date on which the entry was created and posted.
-    - Itemised lines, including amounts and currency.
-    - A reference to the associated accounts.
-    - A reference to the underlying record. For example, the invoice, bill, or other data type that triggered the posting of the journal entry to the general ledger. 
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    > **Pushing journal entries **  
-    > Codat only supports journal entries in the base currency of the company that are pushed into accounts denominated in the same base currency.
-    """
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-    created_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    journal_lines: Optional[list[GetJournalEntrySourceModifiedDateJournalLines]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('journalLines'), 'exclude': lambda f: f is None }})
-    journal_ref: Optional[GetJournalEntrySourceModifiedDateJournalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('journalRef'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetJournalEntrySourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    posted_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postedOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    record_ref: Optional[GetJournalEntrySourceModifiedDateRecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRef'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    supplemental_data: Optional[GetJournalEntrySourceModifiedDateSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
-    updated_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    ledger_lock_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledgerLockDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclasses.dataclass
-class GetJournalEntryResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetJournalEntrySourceModifiedDate] = dataclasses.field(default=None)
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    phone_numbers: Optional[list[CompanyDatasetPhone]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phoneNumbers'), 'exclude': lambda f: f is None }})
+    r"""An array of phone numbers."""  
+    registration_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('registrationNumber'), 'exclude': lambda f: f is None }})
+    r"""Registration number given to the linked company by the companies authority in the country of origin. In the UK this is Companies House."""  
+    source_urls: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceUrls'), 'exclude': lambda f: f is None }})
+    r"""URL addresses for the accounting source.
+    
+    For example, for Xero integrations two URLs are returned. These have many potential use cases, such as [deep linking](https://developer.xero.com/documentation/api-guides/deep-link-xero).
+    """  
+    tax_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxNumber'), 'exclude': lambda f: f is None }})
+    r"""Company tax number."""  
+    web_links: Optional[list[CompanyDatasetWeblink]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webLinks'), 'exclude': lambda f: f is None }})
+    r"""An array of weblinks."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_payment.py` & `codat-accounting-0.9.6/src/codat/models/shared/payment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,108 +1,26 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import accountref as shared_accountref
+from ..shared import customerref as shared_customerref
+from ..shared import metadata as shared_metadata
+from ..shared import paymentline as shared_paymentline
+from ..shared import paymentmethodref as shared_paymentmethodref
+from ..shared import supplementaldata as shared_supplementaldata
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
-from typing import Any, Optional
-
-
-@dataclasses.dataclass
-class GetPaymentRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'paymentId', 'style': 'simple', 'explode': False }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateAccountRef:
-    r"""GetPaymentSourceModifiedDateAccountRef
-    Account the payment is recorded against in the accounting platform.
-    """
-    
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateCustomerRef:
-    r"""GetPaymentSourceModifiedDateCustomerRef
-    Customer the payment is recorded against in the accounting platform.
-    """
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    company_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyName'), 'exclude': lambda f: f is None }})
-    
-class GetPaymentSourceModifiedDateLinesLinksTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    UNLINKED = "Unlinked"
-    INVOICE = "Invoice"
-    CREDIT_NOTE = "CreditNote"
-    OTHER = "Other"
-    REFUND = "Refund"
-    PAYMENT = "Payment"
-    PAYMENT_ON_ACCOUNT = "PaymentOnAccount"
-    MANUAL_JOURNAL = "ManualJournal"
-    DISCOUNT = "Discount"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateLinesLinks:
-    type: GetPaymentSourceModifiedDateLinesLinksTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    
+from typing import Optional
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateLines:
-    amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    allocated_on_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allocatedOnDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    links: Optional[list[GetPaymentSourceModifiedDateLinesLinks]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('links'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDatePaymentMethodRef:
-    r"""GetPaymentSourceModifiedDatePaymentMethodRef
-    The Payment Method to which the payment is linked in the accounting platform.
-    """
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentSourceModifiedDateSupplementalData:
-    r"""GetPaymentSourceModifiedDateSupplementalData
-    Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more.
-    """
-    
-    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPaymentSourceModifiedDate:
-    r"""GetPaymentSourceModifiedDate
-    > **Payments or bill payments?**  
+class Payment:
+    r"""> **Payments or bill payments?**
     > 
     >  In Codat, payments represent accounts receivable only. For accounts payable, see [bill payments](https://docs.codat.io/accounting-api#/schemas/BillPayment). These include [bills](https://docs.codat.io/accounting-api#/schemas/Bill) and credit notes against bills.
     
     > View the coverage for payments in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=payments\" target=\"_blank\">Data coverage explorer</a>.
     
     ## Overview
     
@@ -110,15 +28,15 @@
     
     A payment in Codat usually represents an allocation of money within any customer accounts receivable account. This includes, but is not strictly limited to: 
     
     - A payment made against an invoice, like a credit card, cheque, or cash payment.
     - An allocation of a customer's credit note, either to an invoice or maybe a refund.
     - A payment made directly to that accounts receivable account. This might be an overpayment or a prepayment. It might also be the refund of a payment made directly to an accounts receivable account.
     
-    Depending on the payments allowed by the underlying accounting package, some payment types may be combined. Please see the [Example data](#section-example-data) below for more details.
+    Depending on the payments allowed by the underlying accounting package, some payment types may be combined. Please see the example for more details.
     
     In Codat, a payment contains details of:
     
     - When the payment was recorded in the accounting system.
     - How much it is for and in what currency that amount is in.
     - Who the payment was _paid by_ – the _customer_.
     - The payment method used.
@@ -213,15 +131,15 @@
     The **line** linked to the payment has the following properties:
     
     - An **amount** that indicates the amount that was refunded. This is positive as its money that was added to accounts receivable. It's balanced out by the negative amount of the refund.
     - A **links** array containing one element with the following properties:
       - A **type** that indicates the type of **link**, in this case a `Refund`.
       - An **id** that contains the ID of the payment that refunded this line.
     
-    > 📘 Support for linked payments
+    > **Support for linked payments**
     > 
     > Not all accounting packages support linking payments in this way. In some platforms, you may see a payment on account and a refund on account.
     
     ## Foreign currencies
     
     There are two types of currency rate that are included in the payments data type: 
     
@@ -236,15 +154,15 @@
     - Foreign currency of the payment.
     
     These two rates allow the calculation of currency loss or gain for any of the transactions affected by the payment lines. The second rate is used when a payment is applied to an item in a currency that doesn't match either:
     
     - The base currency for the accounts receivable account. 
     - The currency of the item.
     
-    ```json Currency rate example
+    ```json title=\"Currency rate example\"
     {
         \"id\": \"123\",
         \"note\": \"\"
         \"totalAmount\": 99.99,
         \"currency\": \"GBP\",
         \"lines\": [
             {
@@ -262,21 +180,21 @@
     }
     ```
     
     
     
     ## Example data
     
-    > 📘 Object properties
+    > **Object properties**
     > 
     > For the sake of brevity, the examples here may omit properties from objects. For the full object definition, see [Payments](https://api.codat.io/swagger/index.html#/Payments).
     
     ## Simple examples
     
-    ```json Payment for invoice
+    ```json title=\"Payment for invoice\"
     {
         \"totalAmount\": 1000,
         \"lines\": [
             {
                 \"amount\" : 1000,
                 \"links\" : [
                     {
@@ -288,15 +206,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Allocation of credit note
+    ```json title=\"Allocation of credit note\"
     {
         \"totalAmount\": 0,
         \"lines\": [
             {
                 \"amount\" : 0,
                 \"links\" : [
                     {
@@ -313,15 +231,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Payment of invoice and payment on account
+    ```json title=\"Payment of invoice and payment on account\"
     {
         \"totalAmount\": 2000,
         \"lines\": [
             {
                 \"amount\" : 1000,
                 \"links\" : [
                     {
@@ -343,15 +261,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Refund of credit note
+    ```json title=\"Refund of credit note\"
     {
         \"totalAmount\": -1000,
         \"lines\": [
             {
                 \"amount\" : -1000,
                 \"links\" : [
                     {
@@ -363,15 +281,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Refund on accounts receivable account
+    ```json title=\"Refund on accounts receivable account\"
     {
         \"totalAmount\": -1000,
         \"lines\": [
             {
                 \"amount\" : -1000,
                 \"links\" : [
                     {
@@ -383,15 +301,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Linked refund on accounts receivable account
+    ```json title=\"Linked refund on accounts receivable account\"
     {
         \"id\" : \"payment-001\",
         \"totalAmount\": 1000,
         \"lines\": [
             {
                 \"amount\" : 1000,
                 \"links\" : [
@@ -420,15 +338,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Using a credit note and cash to pay an invoice
+    ```json title=\"Using a credit note and cash to pay an invoice\"
     {
         \"totalAmount\": 250,
         \"lines\": [
             {
                 \"amount\": 0,
                 \"links\": [
                     {
@@ -457,15 +375,15 @@
     }
     ```
     
     
     
     ## Complex examples
     
-    ```json Use two credit notes and 1000 in to \"bank\" (cash, cheque etc.) to pay invoice
+    ```json title=\"Use two credit notes and 1000 in to \"bank\" (cash, cheque etc.) to pay invoice\"
     {
         \"totalAmount\": 1000,
         \"lines\": [
             {
                 \"amount\" : 0,
                 \"links\" : [
                     {
@@ -507,15 +425,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Pay an invoice with two credit notes and cash, with 1000 left \"on account\"
+    ```json title=\"Pay an invoice with two credit notes and cash, with 1000 left 'on account'\"
     {
         \"totalAmount\": 2000,
         \"lines\": [
             {
                 \"amount\" : 0,
                 \"links\" : [
                     {
@@ -567,15 +485,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Two credit notes pay two invoices with no allocation amount specified
+    ```json title=\"Two credit notes pay two invoices with no allocation amount specified\"
     {
         \"totalAmount\": 0,
         \"lines\": [
             {
                 \"amount\" : 0,
                 \"links\" : [
                     {
@@ -602,15 +520,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Two credit notes and cash pay three invoices with no allocation amount specified, and refund cash
+    ```json title=\"Two credit notes and cash pay three invoices with no allocation amount specified, and refund cash\"
     {
         \"totalAmount\": 2000,
         \"lines\": [
             {
                 \"amount\" : 1000,
                 \"links\" : [
                     {
@@ -670,15 +588,15 @@
     }
     ```
     
     
     
     In this example, a payment on account is used to pay the same invoice in January and again in February.
     
-    ```json January
+    ```json title=\"January\"
     {
         \"id\": \"001\",
         \"totalAmount\": 5000,
         \"date\" : \"1901-01-01\",
         \"lines\": [
             {
                 \"amount\" : 1000,
@@ -702,15 +620,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json February
+    ```json title=\"February\"
     {
         \"id\": \"001\",
         \"totalAmount\": 5000,
         \"date\" : \"1901-02-01\",
         \"lines\": [
             {
                 \"amount\" : 1000,
@@ -744,15 +662,15 @@
             }
         ]
     }
     ```
     
     
     
-    ```json Two credit notes and some cash pay two invoices with no allocations specified
+    ```json title=\"Two credit notes and some cash pay two invoices with no allocations specified\"
     {
         \"totalAmount\": 500,
         \"lines\": [
             {
                 \"amount\": 500,
                 \"links\": [{
                         \"type\": \"Invoice\",
@@ -774,31 +692,122 @@
                 ]
             }
         ]
     }
     ```
     """
     
-    date_: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    account_ref: Optional[GetPaymentSourceModifiedDateAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    date_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    account_ref: Optional[shared_accountref.AccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
+    r"""Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account."""  
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
+    
+    ## Unknown currencies
+    
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
+    
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
     currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
-    customer_ref: Optional[GetPaymentSourceModifiedDateCustomerRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerRef'), 'exclude': lambda f: f is None }})
+    r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
+    
+    Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
+    
+    Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
+    
+    For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
+    
+    ## Examples with base currency of GBP
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **USD**          | $20            | 0.781         | £15.62                     |
+    | **EUR**          | €20            | 0.885         | £17.70                     |
+    | **RUB**          | ₽20            | 0.011         | £0.22                      |
+    
+    ## Examples with base currency of USD
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **GBP**          | £20            | 1.277         | $25.54                     |
+    | **EUR**          | €20            | 1.134         | $22.68                     |
+    | **RUB**          | ₽20            | 0.015         | $0.30                      |
+    """  
+    customer_ref: Optional[shared_customerref.CustomerRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerRef'), 'exclude': lambda f: f is None }})  
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    lines: Optional[list[GetPaymentSourceModifiedDateLines]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetPaymentSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the payment, unique to the company in the accounting platform."""  
+    lines: Optional[list[shared_paymentline.PaymentLine]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lines'), 'exclude': lambda f: f is None }})
+    r"""An array of payment lines."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
     note: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
-    payment_method_ref: Optional[GetPaymentSourceModifiedDatePaymentMethodRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('paymentMethodRef'), 'exclude': lambda f: f is None }})
+    r"""Any additional information associated with the payment."""  
+    payment_method_ref: Optional[shared_paymentmethodref.PaymentMethodRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('paymentMethodRef'), 'exclude': lambda f: f is None }})  
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    supplemental_data: Optional[GetPaymentSourceModifiedDateSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
-    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Friendly reference for the payment."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclasses.dataclass
-class GetPaymentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetPaymentSourceModifiedDate] = dataclasses.field(default=None)
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    supplemental_data: Optional[shared_supplementaldata.SupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""Amount of the payment in the payment currency. This value should never change and represents the amount of money paid into the customer's account."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_payment_method.py` & `codat-accounting-0.9.6/src/codat/models/shared/bankstatementaccount.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,72 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import one as shared_one
+from ..shared import zero as shared_zero
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetPaymentMethodRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    payment_method_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'paymentMethodId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPaymentMethodSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+class BankStatementAccount:
+    r"""Success"""
     
-class GetPaymentMethodSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-
-class GetPaymentMethodSourceModifiedDateTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    CASH = "Cash"
-    CHECK = "Check"
-    CREDIT_CARD = "CreditCard"
-    DEBIT_CARD = "DebitCard"
-    BANK_TRANSFER = "BankTransfer"
-    OTHER = "Other"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetPaymentMethodSourceModifiedDate:
-    r"""GetPaymentMethodSourceModifiedDate
-    > View the coverage for payment methods in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=paymentMethods\" target=\"_blank\">Data coverage explorer</a>.
-    
-    ## Overview
-    
-    A Payment Method represents the payment method(s) used to pay a Bill. Payment Methods are referenced on [Bill Payments](https://docs.codat.io/accounting-api#/schemas/BillPayment) and [Payments](https://docs.codat.io/accounting-api#/schemas/Payment).
-    
-    From the Payment Methods endpoints you can retrieve:
-    
-    - A list of all the Payment Methods used by a company: `GET/companies/{companyId}/data/paymentMethods`.
-    - The details of an individual Payment Method:  
-      `GET /companies/{companyId}/data/paymentMethods/{paymentMethodId}`.
-    """
-    
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetPaymentMethodSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status: Optional[GetPaymentMethodSourceModifiedDateStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    type: Optional[GetPaymentMethodSourceModifiedDateTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    account_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountName'), 'exclude': lambda f: f is None }})  
+    account_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountNumber'), 'exclude': lambda f: f is None }})  
+    available_balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('availableBalance'), 'exclude': lambda f: f is None }})  
+    balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})  
+    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})  
+    from_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fromDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclasses.dataclass
-class GetPaymentMethodResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetPaymentMethodSourceModifiedDate] = dataclasses.field(default=None)
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    iban: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iban'), 'exclude': lambda f: f is None }})  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    institution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('institution'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[shared_zero.Zero] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})  
+    nominal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nominalCode'), 'exclude': lambda f: f is None }})  
+    overdraft_limit: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('overdraftLimit'), 'exclude': lambda f: f is None }})  
+    sort_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortCode'), 'exclude': lambda f: f is None }})  
+    source_modified_date: Optional[shared_one.One] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})  
+    to_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('toDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_supplier.py` & `codat-accounting-0.9.6/src/codat/models/shared/createbankaccountresponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,101 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import account as shared_account
+from ..shared import datatype_enum as shared_datatype_enum
+from ..shared import pushoperationchange as shared_pushoperationchange
+from ..shared import pushoperationstatus_enum as shared_pushoperationstatus_enum
+from ..shared import validation as shared_validation
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
-from typing import Any, Optional
-
-
-@dataclasses.dataclass
-class GetSupplierRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    supplier_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'supplierId', 'style': 'simple', 'explode': False }})
-    
-class GetSupplierSourceModifiedDateAddressesTypeEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    BILLING = "Billing"
-    DELIVERY = "Delivery"
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSupplierSourceModifiedDateAddresses:
-    type: GetSupplierSourceModifiedDateAddressesTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
-    region: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
+class CreateBankAccountResponse:
+    r"""Success"""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSupplierSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId') }})
+    r"""Unique identifier for your SMB in Codat."""  
+    data_connection_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionKey') }})
+    r"""Unique identifier for a company's data connection."""  
+    push_operation_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushOperationKey') }})
+    r"""A unique identifier generated by Codat to represent this single push operation. This identifier can be used to track the status of the push, and should be persisted."""  
+    requested_on_utc: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requestedOnUtc') }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-class GetSupplierSourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSupplierSourceModifiedDateSupplementalData:
-    r"""GetSupplierSourceModifiedDateSupplementalData
-    Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more.
-    """
     
-    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSupplierSourceModifiedDate:
-    r"""GetSupplierSourceModifiedDate
-    > View the coverage for suppliers in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers\" target=\"_blank\">Data coverage explorer</a>.
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    status: shared_pushoperationstatus_enum.PushOperationStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""The status of the push operation."""  
+    status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})  
+    changes: Optional[list[shared_pushoperationchange.PushOperationChange]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('changes'), 'exclude': lambda f: f is None }})  
+    completed_on_utc: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('completedOnUtc'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    ## Overview
     
-    From the **Suppliers** endpoints, you can retrieve a list of [all the suppliers for a company](https://api.codat.io/swagger/index.html#/Suppliers/get_companies__companyId__data_suppliers). Suppliers' data links to accounts payable [bills](https://docs.codat.io/accounting-api#/schemas/Bill).
-    """
     
-    status: GetSupplierSourceModifiedDateStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    addresses: Optional[list[GetSupplierSourceModifiedDateAddresses]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addresses'), 'exclude': lambda f: f is None }})
-    contact_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactName'), 'exclude': lambda f: f is None }})
-    default_currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCurrency'), 'exclude': lambda f: f is None }})
-    email_address: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailAddress'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetSupplierSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    registration_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('registrationNumber'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    supplemental_data: Optional[GetSupplierSourceModifiedDateSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
-    supplier_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierName'), 'exclude': lambda f: f is None }})
-    tax_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxNumber'), 'exclude': lambda f: f is None }})
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    data: Optional[shared_account.Account] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    r"""> **Language tip:** Accounts are also referred to as **chart of accounts**, **nominal accounts**, and **general ledger**.
     
-
-@dataclasses.dataclass
-class GetSupplierResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetSupplierSourceModifiedDate] = dataclasses.field(default=None)
+    View the coverage for accounts in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=chartOfAccounts\" target=\"_blank\">Data coverage explorer</a>.
+    
+    ## Overview
+    
+    Accounts are the categories a business uses to record accounting transactions. From the Accounts endpoints, you can retrieve a list of all accounts for a specified company. 
+    
+    The categories for an account include:
+      * Asset
+      * Expense
+      * Income
+      * Liability
+      * Equity.
+    
+    > **Accounts with no category**
+    > 
+    > If an account is pulled from the chart of accounts and its nominal code does not lie within the category layout for the company's accounts, then the **type** is `Unknown`. The **fullyQualifiedCategory** and **fullyQualifiedName** fields return `null`.
+    > 
+    > This approach gives a true representation of the company's accounts whilst preventing distorting financials such as a company's profit and loss and balance sheet reports.
+    """  
+    data_type: Optional[shared_datatype_enum.DataTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
+    r"""Available Data types"""  
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    timeout_in_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInMinutes'), 'exclude': lambda f: f is None }})  
+    timeout_in_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeoutInSeconds'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_validation.Validation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
+    r"""A human-readable object describing validation decisions Codat has made when pushing data into the platform. If a push has failed because of validation errors, they will be detailed here."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/get_tax_rate.py` & `codat-accounting-0.9.6/src/codat/models/shared/transfer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,108 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import metadata as shared_metadata
+from ..shared import supplementaldata as shared_supplementaldata
+from ..shared import trackingcategoryref as shared_trackingcategoryref
+from ..shared import transferaccount as shared_transferaccount
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetTaxRateRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    tax_rate_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'taxRateId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTaxRate200ApplicationJSONComponents:
-    is_compound: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isCompound') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
+class TransferContactRef:
+    r"""The customer or supplier for the transfer, if available."""
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetTaxRate200ApplicationJSONMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})  
     
-class GetTaxRate200ApplicationJSONStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTaxRate200ApplicationJSONValidDataTypeLinks:
-    r"""GetTaxRate200ApplicationJSONValidDataTypeLinks
-    When querying Codat's data model, some data types return `validDatatypeLinks` metadata in the JSON response. This indicates where that object can be used as a reference—a _valid link_—when creating or updating other data.
-    
-    For example, `validDatatypeLinks` might indicate the following references:
-    
-    - Which tax rates are valid to use on the line item of a bill.
-    - Which items can be used when creating an invoice. 
-    
-    You can use `validDatatypeLinks` to present your SMB customers with only valid choices when selecting objects from a list, for example.
+class Transfer:
+    r"""> View the coverage for transfers in the <a className=\\"external\\" href=\\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=transfers\\" target=\\"_blank\\">Data coverage explorer</a>.
     
-    ## `validDatatypeLinks` example
+    A transfer records the movement of money between two bank accounts, or between a bank account and a nominal account. It is a child data type of [account transactions](https://docs.codat.io/accounting-api#/schemas/AccountTransaction).
+    """
     
-    The following example uses the `Accounting.Accounts` data type. It shows that, on the linked integration, this account is valid as the account on a payment or bill payment; and as the account referenced on the line item of a direct income or direct cost. Because there is no valid link to Invoices or Bills, using this account on those data types will result in an error.
+    contact_ref: Optional[TransferContactRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactRef'), 'exclude': lambda f: f is None }})
+    r"""The customer or supplier for the transfer, if available."""  
+    date_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    ```json validDatatypeLinks for an account
-    {
-                \"id\": \"bd9e85e0-0478-433d-ae9f-0b3c4f04bfe4\",
-                \"nominalCode\": \"090\",
-                \"name\": \"Business Bank Account\",
-                #...
-                \"validDatatypeLinks\": [
-                    {
-                        \"property\": \"Id\",
-                        \"links\": [
-                            \"Payment.AccountRef.Id\",
-                            \"BillPayment.AccountRef.Id\",
-                            \"DirectIncome.LineItems.AccountRef.Id\",
-                            \"DirectCost.LineItems.AccountRef.Id\"
-                        ]
-                    }
-                ]
-            }
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
     ```
     
     
     
-    ## Support for `validDatatypeLinks`
-    
-    Codat currently supports `validDatatypeLinks` for some data types on our Xero, QuickBooks Online, QuickBooks Desktop, Exact (NL), and Sage Business Cloud integrations. 
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    If you'd like us to extend support to more data types or integrations, suggest or vote for this on our <a href=\"https://portal.productboard.com/codat/5-product-roadmap\">Product Roadmap</a>.
-    """
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    deposited_record_refs: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('depositedRecordRefs'), 'exclude': lambda f: f is None }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Description of the transfer."""  
+    from_: Optional[shared_transferaccount.TransferAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from'), 'exclude': lambda f: f is None }})  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for the transfer."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    links: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('links'), 'exclude': lambda f: f is None }})
-    property: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('property'), 'exclude': lambda f: f is None }})
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetTaxRate200ApplicationJSON:
-    r"""GetTaxRate200ApplicationJSON
-    > View the coverage for tax rates in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=taxRates\" target=\"_blank\">Data coverage explorer</a>.
     
-    ## Overview
     
-    Accounting systems typically store a set of taxes and associated rates within the accounting package. This means that users don't have to look up or remember the rates for each type of tax. For example: Applying the tax \"UK sales VAT\" to line items of an invoice adds the correct rate of 20%. 
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    ### Tax components
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-    In some cases, a tax is made up of multiple sub taxes, often called _components_ of the tax.  For example: You may have an item that is charged a tax rate called \"City import tax (8%)\" that has two components: 
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    - A city tax of 5%. 
-    - An import tax of 3%.
     
-    > **Effective tax rates**  
-    > Where there are multiple components of a tax, each component may be calculated on the original amount and added together. Alternatively, one tax may be calculated on the sub-total of the original amount plus another tax, which is referred to as _compounding_. When there is compounding, the effective tax rate is the rate that, if applied to the original amount, would result in the total amount of tax with compounding.  
-    >
-    > **Example:**  
-    > A tax has two components. Both components have a rate of 10%, and one component is compound. In this case, there is a total tax rate of 20% but an effective tax rate of 21%. [Also see _Compound tax example_](#section-compound-tax-example).
-    > - For QuickBooks Online, Codat doesn't use compound rates. Instead, the calculated effective tax rate for each component is shown. This means that the effective and total rates are the same because the total tax rate is a sum of the component rates.
-    """
     
-    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
-    components: Optional[list[GetTaxRate200ApplicationJSONComponents]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('components'), 'exclude': lambda f: f is None }})
-    effective_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('effectiveTaxRate'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    metadata: Optional[GetTaxRate200ApplicationJSONMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status: Optional[GetTaxRate200ApplicationJSONStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    total_tax_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalTaxRate'), 'exclude': lambda f: f is None }})
-    valid_datatype_links: Optional[list[GetTaxRate200ApplicationJSONValidDataTypeLinks]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validDatatypeLinks'), 'exclude': lambda f: f is None }})
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-
-@dataclasses.dataclass
-class GetTaxRateResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_tax_rate_200_application_json_object: Optional[GetTaxRate200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    supplemental_data: Optional[shared_supplementaldata.SupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""  
+    to: Optional[shared_transferaccount.TransferAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to'), 'exclude': lambda f: f is None }})  
+    tracking_category_refs: Optional[list[shared_trackingcategoryref.TrackingCategoryRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trackingCategoryRefs'), 'exclude': lambda f: f is None }})
+    r"""Reference to the tracking categories this transfer is being tracked against."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/is_aged_creditors_report_available.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_purchase_order.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import purchaseorder as shared_purchaseorder
 from typing import Optional
 
 
 @dataclasses.dataclass
-class IsAgedCreditorsReportAvailableRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+class GetPurchaseOrderRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    purchase_order_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'purchaseOrderId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class IsAgedCreditorsReportAvailableResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    is_aged_creditors_report_available_200_application_json_boolean: Optional[bool] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetPurchaseOrderResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    purchase_order: Optional[shared_purchaseorder.PurchaseOrder] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/is_aged_debtor_report_available.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_bill_credit_note.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import billcreditnote as shared_billcreditnote
 from typing import Optional
 
 
 @dataclasses.dataclass
-class IsAgedDebtorReportAvailableRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
+class GetBillCreditNoteRequest:
+    
+    bill_credit_note_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'billCreditNoteId', 'style': 'simple', 'explode': False }})  
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class IsAgedDebtorReportAvailableResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    is_aged_debtor_report_available_200_application_json_boolean: Optional[bool] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetBillCreditNoteResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    bill_credit_note: Optional[shared_billcreditnote.BillCreditNote] = dataclasses.field(default=None)
+    r"""Success"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/list_journal_entries.py` & `codat-accounting-0.9.6/src/codat/models/shared/bill.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,222 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import billlineitem as shared_billlineitem
+from ..shared import billstatus_enum as shared_billstatus_enum
+from ..shared import metadata as shared_metadata
+from ..shared import paymentallocationpayment as shared_paymentallocationpayment
+from ..shared import purchaseorderref as shared_purchaseorderref
+from ..shared import supplierref as shared_supplierref
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Any, Optional
 
 
-@dataclasses.dataclass
-class ListJournalEntriesRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
-    page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
-    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListJournalEntriesLinksLinksCurrent:
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})
+class BillPaymentAllocationAllocation:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksLinksNext:
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+    allocated_on_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allocatedOnDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksLinksPrevious:
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksLinksSelf:
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksLinks:
-    current: ListJournalEntriesLinksLinksCurrent = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})
-    self_: ListJournalEntriesLinksLinksSelf = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})
-    next: Optional[ListJournalEntriesLinksLinksNext] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[ListJournalEntriesLinksLinksPrevious] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateJournalLinesAccountRef:
-    r"""ListJournalEntriesLinksSourceModifiedDateJournalLinesAccountRef
-    Data types that reference an account, for example bill and invoice line items, use an accountRef that includes the ID and name of the linked account.
-    """
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateJournalLinesTracking:
-    r"""ListJournalEntriesLinksSourceModifiedDateJournalLinesTracking
-    List of record refs associated with the tracking information for the line (eg to a Tracking Category, or customer etc.)
-    """
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
+    r"""The currency data type in Codat is the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code, e.g. _GBP_.
     
-    record_refs: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRefs'), 'exclude': lambda f: f is None }})
+    ## Unknown currencies
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateJournalLines:
-    net_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('netAmount') }})
-    account_ref: Optional[ListJournalEntriesLinksSourceModifiedDateJournalLinesAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    tracking: Optional[ListJournalEntriesLinksSourceModifiedDateJournalLinesTracking] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking'), 'exclude': lambda f: f is None }})
+    In line with the ISO 4217 specification, the code _XXX_ is used when the data source does not return a currency for a transaction. 
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateJournalRef:
-    r"""ListJournalEntriesLinksSourceModifiedDateJournalRef
-    Links journal entries to the relevant journal in accounting integrations that use multi-book accounting (multiple journals).
-    """
+    There are only a very small number of edge cases where this currency code is returned by the Codat system.
+    """  
+    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
+    r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
+    
+    Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
+    
+    For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
+    
+    ## Examples with base currency of GBP
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **USD**          | $20            | 0.781         | £15.62                     |
+    | **EUR**          | €20            | 0.885         | £17.70                     |
+    | **RUB**          | ₽20            | 0.011         | £0.22                      |
+    
+    ## Examples with base currency of USD
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **GBP**          | £20            | 1.277         | $25.54                     |
+    | **EUR**          | €20            | 1.134         | $22.68                     |
+    | **RUB**          | ₽20            | 0.015         | $0.30                      |
+    """  
+    total_amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount'), 'exclude': lambda f: f is None }})
+    r"""The total amount that has been allocated."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateMetadata:
-    is_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDeleted'), 'exclude': lambda f: f is None }})
+class BillPaymentAllocation:
+    
+    allocation: BillPaymentAllocationAllocation = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allocation') }})  
+    payment: shared_paymentallocationpayment.PaymentAllocationPayment = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateRecordRef:
-    r"""ListJournalEntriesLinksSourceModifiedDateRecordRef
-    Links to the underlying record or data type.
-    
-    Found on:
-    
-    - Journal entries
-    - Account transactions
-    - Invoices
-    - Transfers
-    """
+class BillSupplementalData:
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""
     
-    data_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDateSupplementalData:
-    r"""ListJournalEntriesLinksSourceModifiedDateSupplementalData
-    Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more.
-    """
+class BillWithholdingTax:
     
-    content: Optional[dict[str, dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListJournalEntriesLinksSourceModifiedDate:
-    r"""ListJournalEntriesLinksSourceModifiedDate
-    > **Language tip:** For the top-level record of a company's financial transactions, refer to the [Journals](https://docs.codat.io/accounting-api#/schemas/Journal) data type
+class Bill:
+    r"""> **Invoices or bills?**
+    >
+    > In Codat, bills are for accounts payable only. For the accounts receivable equivalent of bills, see [Invoices](https://docs.codat.io/accounting-api#/schemas/Invoice).
     
-    > View the coverage for journal entries in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=journalEntries\" target=\"_blank\">Data coverage explorer</a>.
+    View the coverage for bills in the <a className=\"external\" href=\"https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bills\" target=\"_blank\">Data coverage explorer</a>.
     
     ## Overview
     
-    A journal entry report shows the entries made in a company's general ledger, or [accounts](https://api.codat.io/swagger/index.html#/Accounts/get_companies__companyId__data_accounts), when transactions are approved. The journal line items for each journal entry should balance.
-    
-    A journal entry line item is a single transaction line on the journal entry. For example: 
-    
-    - When a journal entry is recording a receipt of cash, the credit to accounts receivable and the debit to cash are separate line items. 
-    - When a company needs to recognise revenue from an annual contract on a monthly basis, on receipt of cash for month one, they make a debit to deferred income and a credit to revenue.
-    
-    In Codat a journal entry contains details of:
+    In Codat, a bill contains details of:
+    * When the bill was recorded in the accounting system.
+    * How much the bill is for and the currency of the amount.
+    * Who the bill was received from — the *supplier*.
+    * What the bill is for — the *line items*.
+    
+    Some accounting platforms give a separate name to purchases where the payment is made immediately, such as something bought with a credit card or online payment. One example of this would be QuickBooks Online's *expenses*.
+    
+    You can find these types of transactions in our [Direct costs](https://docs.codat.io/accounting-api#/schemas/DirectCost) data model.
+    """
+    
+    issue_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('issueDate') }})  
+    status: shared_billstatus_enum.BillStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    r"""Current state of the bill."""  
+    sub_total: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subTotal') }})
+    r"""Total amount of the bill, excluding any taxes."""  
+    tax_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxAmount') }})
+    r"""Amount of tax on the bill."""  
+    total_amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalAmount') }})
+    r"""Amount of the bill, including tax."""  
+    amount_due: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amountDue'), 'exclude': lambda f: f is None }})
+    r"""Amount outstanding on the bill."""  
+    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})  
+    currency_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currencyRate'), 'exclude': lambda f: f is None }})
+    r"""Rate to convert the total amount of the payment into the base currency for the company at the time of the payment.
+    
+    Currency rates in Codat are implemented as the multiple of foreign currency units to each base currency unit.  
+    
+    Where the currency rate is provided by the underlying accounting platform, it will be available from Codat with the same precision (up to a maximum of 9 decimal places). 
+    
+    For accounting platforms which do not provide an explicit currency rate, it is calculated as `baseCurrency / foreignCurrency` and will be returned to 9 decimal places.
+    
+    ## Examples with base currency of GBP
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (GBP) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **USD**          | $20            | 0.781         | £15.62                     |
+    | **EUR**          | €20            | 0.885         | £17.70                     |
+    | **RUB**          | ₽20            | 0.011         | £0.22                      |
+    
+    ## Examples with base currency of USD
+    
+    | Foreign Currency | Foreign Amount | Currency Rate | Base Currency Amount (USD) |
+    | :--------------- | :------------- | :------------ | :------------------------- |
+    | **GBP**          | £20            | 1.277         | $25.54                     |
+    | **EUR**          | €20            | 1.134         | $22.68                     |
+    | **RUB**          | ₽20            | 0.015         | $0.30                      |
+    """  
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the bill, unique for the company in the accounting platform."""  
+    line_items: Optional[list[shared_billlineitem.BillLineItem]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lineItems'), 'exclude': lambda f: f is None }})
+    r"""Array of Bill line items."""  
+    metadata: Optional[shared_metadata.Metadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    - The date on which the entry was created and posted.
-    - Itemised lines, including amounts and currency.
-    - A reference to the associated accounts.
-    - A reference to the underlying record. For example, the invoice, bill, or other data type that triggered the posting of the journal entry to the general ledger. 
     
-    > **Pushing journal entries **  
-    > Codat only supports journal entries in the base currency of the company that are pushed into accounts denominated in the same base currency.
-    """
     
-    created_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    journal_lines: Optional[list[ListJournalEntriesLinksSourceModifiedDateJournalLines]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('journalLines'), 'exclude': lambda f: f is None }})
-    journal_ref: Optional[ListJournalEntriesLinksSourceModifiedDateJournalRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('journalRef'), 'exclude': lambda f: f is None }})
-    metadata: Optional[ListJournalEntriesLinksSourceModifiedDateMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    posted_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postedOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    record_ref: Optional[ListJournalEntriesLinksSourceModifiedDateRecordRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('recordRef'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    supplemental_data: Optional[ListJournalEntriesLinksSourceModifiedDateSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
-    updated_on: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedOn'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    note: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
+    r"""Any private, company notes about the bill, such as payment information."""  
+    payment_allocations: Optional[list[BillPaymentAllocation]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('paymentAllocations'), 'exclude': lambda f: f is None }})
+    r"""An array of payment allocations."""  
+    purchase_order_refs: Optional[list[shared_purchaseorderref.PurchaseOrderRef]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purchaseOrderRefs'), 'exclude': lambda f: f is None }})  
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    r"""User-friendly reference for the bill."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListJournalEntriesLinks:
-    r"""ListJournalEntriesLinks
-    Codat's Paging Model
-    """
     
-    links: ListJournalEntriesLinksLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})
-    results: Optional[list[ListJournalEntriesLinksSourceModifiedDate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
     
-
-@dataclasses.dataclass
-class ListJournalEntriesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    links: Optional[ListJournalEntriesLinks] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    supplemental_data: Optional[BillSupplementalData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplementalData'), 'exclude': lambda f: f is None }})
+    r"""Reference to a configured dynamic key value pair that is unique to the accounting platform. This feature is in private beta, contact us if you would like to learn more."""  
+    supplier_ref: Optional[shared_supplierref.SupplierRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('supplierRef'), 'exclude': lambda f: f is None }})
+    r"""Reference to the supplier the record relates to."""  
+    withholding_tax: Optional[list[BillWithholdingTax]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('withholdingTax'), 'exclude': lambda f: f is None }})
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/post_direct_cost_attachment.py` & `codat-accounting-0.9.6/src/codat/models/shared/purchaseorderref.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
+from codat import utils
+from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostDirectCostAttachmentRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    direct_cost_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directCostId', 'style': 'simple', 'explode': False }})
+class PurchaseOrderRef:
     
-
-@dataclasses.dataclass
-class PostDirectCostAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""Identifier for the purchase order, unique for the company in the accounting platform."""  
+    purchase_order_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purchaseOrderNumber'), 'exclude': lambda f: f is None }})
+    r"""Friendly reference for the purchase order, commonly generated by the accounting platform."""
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/post_direct_income_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_create_update_customers_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import pushoption as shared_pushoption
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PostDirectIncomeAttachmentRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    direct_income_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'directIncomeId', 'style': 'simple', 'explode': False }})
+class GetCreateUpdateCustomersModelRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class PostDirectIncomeAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetCreateUpdateCustomersModelResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    push_option: Optional[shared_pushoption.PushOption] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/models/operations/push_invoice_attachment.py` & `codat-accounting-0.9.6/src/codat/models/operations/get_create_update_invoices_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import pushoption as shared_pushoption
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PushInvoiceAttachmentRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    invoice_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'invoiceId', 'style': 'simple', 'explode': False }})
+class GetCreateUpdateInvoicesModelRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class PushInvoiceAttachmentResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class GetCreateUpdateInvoicesModelResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    push_option: Optional[shared_pushoption.PushOption] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `codat-accounting-0.5.1/src/codat/payment_methods.py` & `codat-accounting-0.9.6/src/codat/payment_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class PaymentMethods:
+    r"""Payment methods"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,39 +22,37 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_payment_method(self, request: operations.GetPaymentMethodRequest) -> operations.GetPaymentMethodResponse:
         r"""Get payment method
         Gets the specified payment method for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetPaymentMethodRequest, base_url, '/companies/{companyId}/data/paymentMethods/{paymentMethodId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPaymentMethodResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetPaymentMethodSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentMethod])
+                res.payment_method = out
 
         return res
 
     def list_payment_methods(self, request: operations.ListPaymentMethodsRequest) -> operations.ListPaymentMethodsResponse:
         r"""List all payment methods
         Gets the payment methods for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListPaymentMethodsRequest, base_url, '/companies/{companyId}/data/paymentMethods', request)
         
         query_params = utils.get_query_params(operations.ListPaymentMethodsRequest, request)
         
         client = self._security_client
@@ -59,13 +60,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListPaymentMethodsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListPaymentMethodsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentMethods])
+                res.payment_methods = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/payments.py` & `codat-accounting-0.9.6/src/codat/payments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Payments:
+    r"""Payments"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,98 +28,94 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create payment model](https://docs.codat.io/accounting-api#/operations/get-create-payments-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=payments) for integrations that support creating payments.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePaymentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/payments', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "payment", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreatePaymentRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreatePaymentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreatePayment200ApplicationJSON])
-                res.create_payment_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreatePaymentResponse])
+                res.create_payment_response = out
 
         return res
 
     def get_create_payments_model(self, request: operations.GetCreatePaymentsModelRequest) -> operations.GetCreatePaymentsModelResponse:
         r"""Get create payment model
         Get create payment model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=payments) for integrations that support creating payments.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreatePaymentsModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/payments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreatePaymentsModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreatePaymentsModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_payment(self, request: operations.GetPaymentRequest) -> operations.GetPaymentResponse:
         r"""Get payment
         Get payment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetPaymentRequest, base_url, '/companies/{companyId}/data/payments/{paymentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPaymentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetPaymentSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Payment])
+                res.payment = out
 
         return res
 
     def list_payments(self, request: operations.ListPaymentsRequest) -> operations.ListPaymentsResponse:
         r"""List payments
         Gets the latest payments for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListPaymentsRequest, base_url, '/companies/{companyId}/data/payments', request)
         
         query_params = utils.get_query_params(operations.ListPaymentsRequest, request)
         
         client = self._security_client
@@ -124,13 +123,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListPaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListPaymentsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Payments])
+                res.payments = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/purchase_orders.py` & `codat-accounting-0.9.6/src/codat/purchase_orders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class PurchaseOrders:
+    r"""Purchase orders"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,98 +28,94 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create/update purchase order model](https://docs.codat.io/accounting-api#/operations/get-create-update-purchaseOrders-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=purchaseOrders) for integrations that support creating purchase orders.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePurchaseOrderRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/purchaseOrders', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "purchase_order", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.CreatePurchaseOrderRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreatePurchaseOrderResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreatePurchaseOrder200ApplicationJSON])
-                res.create_purchase_order_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreatePurchaseOrderResponse])
+                res.create_purchase_order_response = out
 
         return res
 
     def get_create_update_purchase_orders_model(self, request: operations.GetCreateUpdatePurchaseOrdersModelRequest) -> operations.GetCreateUpdatePurchaseOrdersModelResponse:
         r"""Get create/update purchase order model
         Get create/update purchase order model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=purchaseOrders) for integrations that support creating and updating purchase orders.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdatePurchaseOrdersModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/purchaseOrders', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdatePurchaseOrdersModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdatePurchaseOrdersModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_purchase_order(self, request: operations.GetPurchaseOrderRequest) -> operations.GetPurchaseOrderResponse:
         r"""Get purchase order
         Get purchase order
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetPurchaseOrderRequest, base_url, '/companies/{companyId}/data/purchaseOrders/{purchaseOrderId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPurchaseOrderResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetPurchaseOrderSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PurchaseOrder])
+                res.purchase_order = out
 
         return res
 
     def list_purchase_orders(self, request: operations.ListPurchaseOrdersRequest) -> operations.ListPurchaseOrdersResponse:
         r"""List purchase orders
         Get purchase orders
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListPurchaseOrdersRequest, base_url, '/companies/{companyId}/data/purchaseOrders', request)
         
         query_params = utils.get_query_params(operations.ListPurchaseOrdersRequest, request)
         
         client = self._security_client
@@ -124,48 +123,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListPurchaseOrdersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListPurchaseOrdersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PurchaseOrders])
+                res.purchase_orders = out
 
         return res
 
     def update_purchase_order(self, request: operations.UpdatePurchaseOrderRequest) -> operations.UpdatePurchaseOrderResponse:
         r"""Update purchase order
         Posts an updated purchase order to the accounting package for a given company.
         
         Required data may vary by integration. To see what data to post, first call []().
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=purchaseOrders) for integrations that support updating purchase orders.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdatePurchaseOrderRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/purchaseOrders/{purchaseOrderId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "purchase_order", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.UpdatePurchaseOrderRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdatePurchaseOrderResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdatePurchaseOrder200ApplicationJSON])
-                res.update_purchase_order_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.UpdatePurchaseOrderResponse])
+                res.update_purchase_order_response = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/reports.py` & `codat-accounting-0.9.6/src/codat/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Reports:
+    r"""Reports"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,15 +22,14 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_aged_creditors_report(self, request: operations.GetAgedCreditorsReportRequest) -> operations.GetAgedCreditorsReportResponse:
         r"""Aged creditors report
         Returns aged creditors report for company that shows the total balance owed by a business to its suppliers over time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAgedCreditorsReportRequest, base_url, '/companies/{companyId}/reports/agedCreditor', request)
         
         query_params = utils.get_query_params(operations.GetAgedCreditorsReportRequest, request)
         
         client = self._security_client
@@ -35,24 +37,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAgedCreditorsReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAgedCreditorsReportAgedCreditorsReport])
-                res.aged_creditors_report = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AgedCreditorReport])
+                res.aged_creditor_report = out
 
         return res
 
     def get_aged_debtors_report(self, request: operations.GetAgedDebtorsReportRequest) -> operations.GetAgedDebtorsReportResponse:
         r"""Aged debtors report
         Returns aged debtors report for company that shows the total outstanding balance due from customers to the business over time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAgedDebtorsReportRequest, base_url, '/companies/{companyId}/reports/agedDebtor', request)
         
         query_params = utils.get_query_params(operations.GetAgedDebtorsReportRequest, request)
         
         client = self._security_client
@@ -60,24 +61,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAgedDebtorsReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAgedDebtorsReportAgedDebtorsReport])
-                res.aged_debtors_report = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AgedDebtorReport])
+                res.aged_debtor_report = out
 
         return res
 
     def is_aged_creditors_report_available(self, request: operations.IsAgedCreditorsReportAvailableRequest) -> operations.IsAgedCreditorsReportAvailableResponse:
         r"""Aged creditors report available
         Indicates whether the aged creditor report is available for the company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.IsAgedCreditorsReportAvailableRequest, base_url, '/companies/{companyId}/reports/agedCreditor/available', request)
         
         
         client = self._security_client
         
@@ -93,15 +93,14 @@
 
         return res
 
     def is_aged_debtor_report_available(self, request: operations.IsAgedDebtorReportAvailableRequest) -> operations.IsAgedDebtorReportAvailableResponse:
         r"""Aged debtors report available
         Indicates whether the aged debtor report is available for the company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.IsAgedDebtorReportAvailableRequest, base_url, '/companies/{companyId}/reports/agedDebtor/available', request)
         
         
         client = self._security_client
```

### Comparing `codat-accounting-0.5.1/src/codat/sales_orders.py` & `codat-accounting-0.9.6/src/codat/sales_orders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class SalesOrders:
+    r"""Sales orders"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,39 +22,37 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_sales_order(self, request: operations.GetSalesOrderRequest) -> operations.GetSalesOrderResponse:
         r"""Get sales order
         Get sales order
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSalesOrderRequest, base_url, '/companies/{companyId}/data/salesOrders/{salesOrderId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetSalesOrderResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSalesOrderSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SalesOrder])
+                res.sales_order = out
 
         return res
 
     def list_sales_orders(self, request: operations.ListSalesOrdersRequest) -> operations.ListSalesOrdersResponse:
         r"""List sales orders
         Get sales orders
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSalesOrdersRequest, base_url, '/companies/{companyId}/data/salesOrders', request)
         
         query_params = utils.get_query_params(operations.ListSalesOrdersRequest, request)
         
         client = self._security_client
@@ -59,13 +60,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListSalesOrdersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListSalesOrdersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SalesOrders])
+                res.sales_orders = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/sdk.py` & `codat-accounting-0.9.6/src/codat/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-__doc__ = """ SDK Documentation: A flexible API for pulling accounting data, normalized and aggregated from 20 accounting integrations.
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-Standardize how you connect to your customers’ accounting software. View, create, update, and delete data in the same way for all the leading accounting platforms.
-
-[Read more...](https://docs.codat.io/accounting-api/overview)
-
-[See our OpenAPI spec](https://github.com/codatio/oas)    """
 import requests as requests_http
 from . import utils
 from .account_transactions import AccountTransactions
 from .accounts import Accounts
 from .bank_account_transactions import BankAccountTransactions
 from .bank_accounts import BankAccounts
 from .bill_credit_notes import BillCreditNotes
@@ -32,65 +27,105 @@
 from .suppliers import Suppliers
 from .tax_rates import TaxRates
 from .tracking_categories import TrackingCategories
 from .transfers import Transfers
 from codat.models import shared
 
 SERVERS = [
-	"https://api.codat.io",
+    "https://api.codat.io",
+    r"""Production"""
 ]
+"""Contains the list of servers available to the SDK"""
 
 class Codat:
-    r"""SDK Documentation: A flexible API for pulling accounting data, normalized and aggregated from 20 accounting integrations.
+    r"""A flexible API for pulling accounting data, normalized and aggregated from 20 accounting integrations.
     
     Standardize how you connect to your customers’ accounting software. View, create, update, and delete data in the same way for all the leading accounting platforms.
     
     [Read more...](https://docs.codat.io/accounting-api/overview)
     
-    [See our OpenAPI spec](https://github.com/codatio/oas)    """
+    [See our OpenAPI spec](https://github.com/codatio/oas)
+    """
     account_transactions: AccountTransactions
+    r"""Account transactions"""
     accounts: Accounts
+    r"""Accounts"""
     bank_account_transactions: BankAccountTransactions
+    r"""Bank transactions for bank accounts"""
     bank_accounts: BankAccounts
+    r"""Bank accounts"""
     bill_credit_notes: BillCreditNotes
+    r"""Bill credit notes"""
     bill_payments: BillPayments
+    r"""Bill payments"""
     bills: Bills
+    r"""Bills"""
     company_info: CompanyInfo
+    r"""Company info"""
     credit_notes: CreditNotes
+    r"""Credit notes"""
     customers: Customers
+    r"""Customers"""
     direct_costs: DirectCosts
+    r"""Direct costs"""
     direct_incomes: DirectIncomes
+    r"""Direct incomes"""
     financials: Financials
+    r"""Financials"""
     invoices: Invoices
+    r"""Invoices"""
     items: Items
+    r"""Items"""
     journal_entries: JournalEntries
+    r"""Journal entries"""
     journals: Journals
+    r"""Journals"""
     payment_methods: PaymentMethods
+    r"""Payment methods"""
     payments: Payments
+    r"""Payments"""
     purchase_orders: PurchaseOrders
+    r"""Purchase orders"""
     reports: Reports
+    r"""Reports"""
     sales_orders: SalesOrders
+    r"""Sales orders"""
     suppliers: Suppliers
+    r"""Suppliers"""
     tax_rates: TaxRates
+    r"""Tax rates"""
     tracking_categories: TrackingCategories
+    r"""Tracking categories"""
     transfers: Transfers
-    
+    r"""Transfers"""
+
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.5.1"
-    _gen_version: str = "1.12.1"
+    _sdk_version: str = "0.9.6"
+    _gen_version: str = "2.16.7"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
+        """Instantiates the SDK configuring it with the provided parameters.
+        
+        :param security: The security details required for authentication
+        :type security: shared.Security
+        :param server_url: The server URL to use for all operations
+        :type server_url: str
+        :param url_params: Parameters to optionally template the server URL with
+        :type url_params: dict[str, str]
+        :param client: The requests.Session HTTP client to use for all operations
+        :type client: requests_http.Session        
+        """
         self._client = requests_http.Session()
         
         
         if server_url is not None:
             if url_params is not None:
                 self._server_url = utils.template_url(server_url, url_params)
             else:
```

### Comparing `codat-accounting-0.5.1/src/codat/suppliers.py` & `codat-accounting-0.9.6/src/codat/suppliers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Suppliers:
+    r"""Suppliers"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,178 +18,172 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def create_suppliers(self, request: operations.CreateSuppliersRequest) -> operations.CreateSuppliersResponse:
+    def create_supplier(self, request: operations.CreateSupplierRequest) -> operations.CreateSupplierResponse:
         r"""Create suppliers
         Push suppliers
         
         Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/accounting-api#/operations/get-create-update-suppliers-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating suppliers.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.CreateSuppliersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers', request)
+        url = utils.generate_url(operations.CreateSupplierRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "supplier", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.CreateSuppliersRequest, request)
+        query_params = utils.get_query_params(operations.CreateSupplierRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.CreateSuppliersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateSupplierResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateSuppliers200ApplicationJSON])
-                res.create_suppliers_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateSupplierResponse])
+                res.create_supplier_response = out
 
         return res
 
     def download_supplier_attachment(self, request: operations.DownloadSupplierAttachmentRequest) -> operations.DownloadSupplierAttachmentResponse:
         r"""Download supplier attachment
         Download supplier attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.DownloadSupplierAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/suppliers/{supplierId}/attachments/{attachmentId}/download', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DownloadSupplierAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.data = http_res.content
 
         return res
 
     def get_create_update_suppliers_model(self, request: operations.GetCreateUpdateSuppliersModelRequest) -> operations.GetCreateUpdateSuppliersModelResponse:
         r"""Get create/update supplier model
         Get create/update supplier model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support creating and updating suppliers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateUpdateSuppliersModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/suppliers', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateUpdateSuppliersModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateUpdateSuppliersModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_supplier(self, request: operations.GetSupplierRequest) -> operations.GetSupplierResponse:
         r"""Get supplier
         Gets a single supplier corresponding to the given ID.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSupplierRequest, base_url, '/companies/{companyId}/data/suppliers/{supplierId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetSupplierResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSupplierSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Supplier])
+                res.supplier = out
 
         return res
 
     def get_supplier_attachment(self, request: operations.GetSupplierAttachmentRequest) -> operations.GetSupplierAttachmentResponse:
         r"""Get supplier attachment
         Get supplier attachment
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSupplierAttachmentRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/suppliers/{supplierId}/attachments/{attachmentId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetSupplierAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSupplierAttachmentAttachment])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
 
         return res
 
     def list_supplier_attachments(self, request: operations.ListSupplierAttachmentsRequest) -> operations.ListSupplierAttachmentsResponse:
         r"""List supplier attachments
         Get supplier attachments
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSupplierAttachmentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/suppliers/{supplierId}/attachments', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListSupplierAttachmentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListSupplierAttachmentsAttachments])
-                res.attachments = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AttachmentsDataset])
+                res.attachments_dataset = out
 
         return res
 
     def list_suppliers(self, request: operations.ListSuppliersRequest) -> operations.ListSuppliersResponse:
         r"""List suppliers
         Gets the latest suppliers for a company, with pagination
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSuppliersRequest, base_url, '/companies/{companyId}/data/suppliers', request)
         
         query_params = utils.get_query_params(operations.ListSuppliersRequest, request)
         
         client = self._security_client
@@ -194,36 +191,35 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListSuppliersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListSuppliersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Suppliers])
+                res.suppliers = out
 
         return res
 
     def put_supplier(self, request: operations.PutSupplierRequest) -> operations.PutSupplierResponse:
         r"""Update supplier
         Push supplier
         
         Required data may vary by integration. To see what data to post, first call [Get create/update supplier model](https://docs.codat.io/accounting-api#/operations/get-create-update-suppliers-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=suppliers) for integrations that support updating suppliers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PutSupplierRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/suppliers/{supplierId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "supplier", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.PutSupplierRequest, request)
         
         client = self._security_client
         
         http_res = client.request('PUT', url, params=query_params, data=data, files=form, headers=headers)
```

### Comparing `codat-accounting-0.5.1/src/codat/tax_rates.py` & `codat-accounting-0.9.6/src/codat/tax_rates.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class TaxRates:
+    r"""Tax rates"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,39 +22,37 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_tax_rate(self, request: operations.GetTaxRateRequest) -> operations.GetTaxRateResponse:
         r"""Get tax rate
         Gets the specified tax rate for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetTaxRateRequest, base_url, '/companies/{companyId}/data/taxRates/{taxRateId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetTaxRateResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetTaxRate200ApplicationJSON])
-                res.get_tax_rate_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TaxRate])
+                res.tax_rate = out
 
         return res
 
     def list_tax_rates(self, request: operations.ListTaxRatesRequest) -> operations.ListTaxRatesResponse:
         r"""List all tax rates
         Gets the latest tax rates for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListTaxRatesRequest, base_url, '/companies/{companyId}/data/taxRates', request)
         
         query_params = utils.get_query_params(operations.ListTaxRatesRequest, request)
         
         client = self._security_client
@@ -59,13 +60,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListTaxRatesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListTaxRatesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TaxRates])
+                res.tax_rates = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/tracking_categories.py` & `codat-accounting-0.9.6/src/codat/tracking_categories.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class TrackingCategories:
+    r"""Tracking categories"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,39 +22,37 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_tracking_category(self, request: operations.GetTrackingCategoryRequest) -> operations.GetTrackingCategoryResponse:
         r"""Get tracking categories
         Gets the specified tracking categories for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetTrackingCategoryRequest, base_url, '/companies/{companyId}/data/trackingCategories/{trackingCategoryId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetTrackingCategoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetTrackingCategorySourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TrackingCategoryTree])
+                res.tracking_category_tree = out
 
         return res
 
     def list_tracking_categories(self, request: operations.ListTrackingCategoriesRequest) -> operations.ListTrackingCategoriesResponse:
         r"""List tracking categories
         Gets the latest tracking categories for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListTrackingCategoriesRequest, base_url, '/companies/{companyId}/data/trackingCategories', request)
         
         query_params = utils.get_query_params(operations.ListTrackingCategoriesRequest, request)
         
         client = self._security_client
@@ -59,13 +60,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListTrackingCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListTrackingCategoriesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TrackingCategories])
+                res.tracking_categories = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/transfers.py` & `codat-accounting-0.9.6/src/codat/transfers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Transfers:
+    r"""Transfers"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -25,97 +28,93 @@
         
         Required data may vary by integration. To see what data to post, first call [Get create transfer model](https://docs.codat.io/accounting-api#/operations/get-create-transfers-model).
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=transfers) for integrations that support creating transfers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateTransferRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/transfers', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "transfer", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateTransferResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateTransfer200ApplicationJSON])
-                res.create_transfer_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateTransferResponse])
+                res.create_transfer_response = out
 
         return res
 
     def get_create_transfers_model(self, request: operations.GetCreateTransfersModelRequest) -> operations.GetCreateTransfersModelResponse:
         r"""Get create transfer model
         Get create transfer model. Returns the expected data for the request payload.
         
         See the examples for integration-specific indicative models.
         
         > **Supported Integrations**
         > 
         > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=transfers) for integrations that support creating transfers.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCreateTransfersModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/transfers', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCreateTransfersModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCreateTransfersModelPushOption])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
                 res.push_option = out
 
         return res
 
     def get_transfer(self, request: operations.GetTransferRequest) -> operations.GetTransferResponse:
         r"""Get transfer
         Gets the specified transfer for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetTransferRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/transfers/{transferId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetTransferResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetTransferSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transfer])
+                res.transfer = out
 
         return res
 
     def list_transfers(self, request: operations.ListTransfersRequest) -> operations.ListTransfersResponse:
         r"""List transfers
         Gets the transfers for a given company.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListTransfersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/transfers', request)
         
         query_params = utils.get_query_params(operations.ListTransfersRequest, request)
         
         client = self._security_client
@@ -123,13 +122,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListTransfersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListTransfersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transfers])
+                res.transfers = out
 
         return res
```

### Comparing `codat-accounting-0.5.1/src/codat/utils/retries.py` & `codat-accounting-0.9.6/src/codat/utils/retries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
```

### Comparing `codat-accounting-0.5.1/src/codat/utils/utils.py` & `codat-accounting-0.9.6/src/codat/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
```

### Comparing `codat-accounting-0.5.1/src/codat_accounting.egg-info/PKG-INFO` & `codat-accounting-0.9.6/src/codat_accounting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-accounting
-Version: 0.5.1
+Version: 0.9.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,100 +28,100 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCreateUpdateAccountTransactionsModelRequest(
-    account_transaction_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+req = operations.GetAccountTransactionRequest(
+    account_transaction_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.account_transactions.get_create_update_account_transactions_model(req)
+res = s.account_transactions.get_account_transaction(req)
 
-if res.source_modified_date is not None:
+if res.account_transaction is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### account_transactions
 
-* `get_create_update_account_transactions_model` - Get account transaction
+* `get_account_transaction` - Get account transaction
 * `list_account_transactions` - List account transactions
 
 ### accounts
 
 * `create_account` - Create account
 * `get_account` - Get account
-* `get_accounts` - List accounts
 * `get_create_chart_of_accounts_model` - Get create account model
+* `list_accounts` - List accounts
 
 ### bank_account_transactions
 
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
 * `list_bank_transactions` - List all bank transactions
-* `post_bank_transactions` - Create bank transactions
 
 ### bank_accounts
 
 * `create_bank_account` - Create bank account
 * `get_all_bank_account` - Get bank account
 * `get_bank_account` - Get bank account
 * `get_create_update_bank_accounts_model` - Get create/update bank account model
 * `list_bank_accounts` - List bank accounts
-* `put_bank_account` - Update bank account
+* `update_bank_account` - Update bank account
 
 ### bill_credit_notes
 
 * `create_bill_credit_note` - Create bill credit note
 * `get_bill_credit_note` - Get bill credit note
 * `get_create_update_bill_credit_notes_model` - Get create/update bill credit note model
 * `list_bill_credit_notes` - List bill credit notes
 * `update_bill_credit_note` - Update bill credit note
 
 ### bill_payments
 
 * `create_bill_payment` - Create bill payments
-* `delete_companies_company_id_connections_connection_id_push_bill_payments_bill_payment_id` - Delete bill payment
+* `delete_bill_payment` - Delete bill payment
 * `get_bill_payments` - Get bill payment
 * `get_create_bill_payments_model` - Get create bill payment model
 * `list_bill_payments` - List bill payments
 
 ### bills
 
 * `create_bill` - Create bill
-* `create_bill_attachments` - Create bill attachments
-* `delete_companies_company_id_connections_connection_id_push_bills_bill_id` - Delete bill
+* `delete_bill` - Delete bill
 * `download_bill_attachment` - Download bill attachment
 * `get_bill` - Get bill
 * `get_bill_attachment` - Get bill attachment
 * `get_bill_attachments` - List bill attachments
 * `get_create_update_bills_model` - Get create/update bill model
 * `list_bills` - List bills
 * `update_bill` - Update bill
+* `upload_bill_attachments` - Upload bill attachments
 
 ### company_info
 
 * `get_company_info` - Get company info
 * `post_sync_info` - Refresh company info
 
 ### credit_notes
 
-* `create_credit_note` - Update creditNote
+* `create_credit_note` - Create credit note
 * `get_create_update_credit_notes_model` - Get create/update credit note model
 * `get_credit_note` - Get credit note
 * `list_credit_notes` - List credit notes
-* `push_credit_note` - Create credit note
+* `update_credit_note` - Update creditNote
 
 ### customers
 
 * `create_customer` - Create customer
 * `download_customer_attachment` - Download customer attachment
 * `get_create_update_customers_model` - Get create/update customer model
 * `get_customer` - Get customer
@@ -135,45 +135,45 @@
 * `create_direct_cost` - Create direct cost
 * `download_direct_cost_attachment` - Download direct cost attachment
 * `get_create_direct_costs_model` - Get create direct cost model
 * `get_direct_cost` - Get direct cost
 * `get_direct_cost_attachment` - Get direct cost attachment
 * `get_direct_costs` - List direct costs
 * `list_direct_cost_attachments` - List direct cost attachments
-* `post_direct_cost_attachment` - Create direct cost attachment
+* `upload_direct_cost_attachment` - Upload direct cost attachment
 
 ### direct_incomes
 
 * `create_direct_income` - Create direct income
 * `download_direct_income_attachment` - Download direct income attachment
 * `get_create_direct_incomes_model` - Get create direct income model
 * `get_direct_income` - Get direct income
 * `get_direct_income_attachment` - Get direct income attachment
 * `get_direct_incomes` - Get direct incomes
 * `list_direct_income_attachments` - List direct income attachments
-* `post_direct_income_attachment` - Create direct income attachment
+* `upload_direct_income_attachment` - Create direct income attachment
 
 ### financials
 
 * `get_balance_sheet` - Get balance sheet
 * `get_cash_flow_statement` - Get cash flow statement
 * `get_profit_and_loss` - Get profit and loss
 
 ### invoices
 
+* `download_invoice_pdf` - Get invoice as PDF
 * `create_invoice` - Create invoice
-* `donwload_invoice_attachment` - Download invoice attachment
+* `download_invoice_attachment` - Download invoice attachment
 * `get_create_update_invoices_model` - Get create/update invoice model
 * `get_invoice` - Get invoice
 * `get_invoice_attachment` - Get invoice attachment
 * `get_invoice_attachments` - Get invoice attachments
-* `get_invoice_pdf` - Get invoice as PDF
 * `list_invoices` - List invoices
-* `push_invoice_attachment` - Push invoice attachment
 * `update_invoice` - Update invoice
+* `upload_invoice_attachment` - Push invoice attachment
 
 ### items
 
 * `create_item` - Create item
 * `get_create_items_model` - Get create item model
 * `get_item` - Get item
 * `list_items` - List items
@@ -222,15 +222,15 @@
 ### sales_orders
 
 * `get_sales_order` - Get sales order
 * `list_sales_orders` - List sales orders
 
 ### suppliers
 
-* `create_suppliers` - Create suppliers
+* `create_supplier` - Create suppliers
 * `download_supplier_attachment` - Download supplier attachment
 * `get_create_update_suppliers_model` - Get create/update supplier model
 * `get_supplier` - Get supplier
 * `get_supplier_attachment` - Get supplier attachment
 * `list_supplier_attachments` - List supplier attachments
 * `list_suppliers` - List suppliers
 * `put_supplier` - Update supplier
```

