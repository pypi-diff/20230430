# Comparing `tmp/vesselapi-3.2.2.tar.gz` & `tmp/vesselapi-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vesselapi-3.2.2.tar", last modified: Tue Feb 28 21:03:39 2023, max compression
+gzip compressed data, was "vesselapi-3.5.2.tar", last modified: Tue Mar  7 22:17:16 2023, max compression
```

## Comparing `vesselapi-3.2.2.tar` & `vesselapi-3.5.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.762658 vesselapi-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-02-28 21:03:39.762658 vesselapi-3.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3842 2023-02-28 21:03:30.000000 vesselapi-3.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 21:03:39.762658 vesselapi-3.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-02-28 21:03:30.000000 vesselapi-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.742656 vesselapi-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.746657 vesselapi-3.2.2/src/vesselapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8121 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7666 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3614 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7882 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8035 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7918 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7968 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1966 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.746657 vesselapi-3.2.2/src/vesselapi/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.754657 vesselapi-3.2.2/src/vesselapi/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11827 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/delete_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      973 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/delete_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1831 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1656 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1580 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1352 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1522 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1425 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/get_one_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1007 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2454 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1274 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2133 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_link_exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_link_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/post_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1354 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1354 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5729 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4448 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4924 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5756 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3952 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4701 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4601 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3803 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4439 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.758657 vesselapi-3.2.2/src/vesselapi/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3630 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/accountcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/accountupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/address.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/booleanfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1676 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/contactcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/contactupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/datefilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/dealcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/dealupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3973 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/emailcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      984 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/emailupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/eventattendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/eventattendeecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/eventattendeeupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2466 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/eventcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1882 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/eventupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2586 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1611 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/leadcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1667 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/leadupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/notecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/noteupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1606 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/numberfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      401 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/stringfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/stringlistfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2881 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2345 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/taskcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/taskupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2461 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/webhookmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/models/shared/webhookmetadatacreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7960 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1945 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5821 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8010 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1663 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5668 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.758657 vesselapi-3.2.2/src/vesselapi/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3471 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22673 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3715 2023-02-28 21:03:30.000000 vesselapi-3.2.2/src/vesselapi/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:03:39.746657 vesselapi-3.2.2/src/vesselapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-02-28 21:03:39.000000 vesselapi-3.2.2/src/vesselapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-02-28 21:03:39.000000 vesselapi-3.2.2/src/vesselapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:03:39.000000 vesselapi-3.2.2/src/vesselapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-28 21:03:39.000000 vesselapi-3.2.2/src/vesselapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 21:03:39.000000 vesselapi-3.2.2/src/vesselapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.837517 vesselapi-3.5.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3842 2023-03-07 22:17:08.000000 vesselapi-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 22:17:16.837517 vesselapi-3.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.821517 vesselapi-3.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8486 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8065 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3794 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8448 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8247 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8283 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.833517 vesselapi-3.5.2/src/vesselapi/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11828 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1836 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1644 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1674 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5923 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5950 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4875 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4609 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1979 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1915 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/booleanfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4053 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeeupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2518 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2634 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3485 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/numberfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8325 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8375 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/top_level.txt
```

### Comparing `vesselapi-3.2.2/PKG-INFO` & `vesselapi-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vesselapi
-Version: 3.2.2
+Version: 3.5.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: vesselapi
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `vesselapi-3.2.2/README.md` & `vesselapi-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `vesselapi-3.2.2/setup.py` & `vesselapi-3.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="vesselapi",
-    version="3.2.2",
+    version="3.5.2",
     author="vesselapi",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
@@ -26,11 +26,12 @@
         "pyparsing==3.0.9",
         "python-dateutil==2.8.2",
         "requests==2.28.1",
         "six==1.16.0",
         "typing-inspect==0.8.0",
         "typing_extensions==4.3.0",
         "urllib3==1.26.12",
+        "pylint==2.16.2",
     ],
     package_dir={'': 'src'},
     python_requires='>=3.9'
 )
```

### Comparing `vesselapi-3.2.2/src/vesselapi/accounts.py` & `vesselapi-3.5.2/src/vesselapi/accounts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,217 +1,210 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Accounts:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def batch(self, request: operations.GetBatchCrmAccountRequest) -> operations.GetBatchCrmAccountResponse:
         r"""Get Batch Accounts
         Retrieve Accounts by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/account/batch"
+        url = base_url.removesuffix('/') + '/crm/account/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmAccountResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmAccountResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def create(self, request: operations.PostCrmAccountRequest) -> operations.PostCrmAccountResponse:
         r"""Create Account
         Create a new Account
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/account"
+        url = base_url.removesuffix('/') + '/crm/account'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmAccountResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmAccountResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmAccountRequest) -> operations.GetDetailsCrmAccountResponse:
         r"""Get Account Details
         Get details about all accounts. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/account/details"
+        url = base_url.removesuffix('/') + '/crm/account/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmAccountResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmAccountResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmAccountRequest) -> operations.GetOneCrmAccountResponse:
         r"""Get Account
         Retrieve a single Account by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/account"
+        url = base_url.removesuffix('/') + '/crm/account'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmAccountResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmAccountResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmAccountsRequest) -> operations.GetAllCrmAccountsResponse:
         r"""Get All Accounts
         Retrieve all Accounts
         *CRM Caveats*:
         - Pipedrive: dealIds + contactIds not supported when querying for all accounts
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/accounts"
+        url = base_url.removesuffix('/') + '/crm/accounts'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmAccountsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmAccountsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmAccountsRequest) -> operations.SearchCrmAccountsResponse:
         r"""Search Accounts
         Search all Accounts using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/accounts/search"
+        url = base_url.removesuffix('/') + '/crm/accounts/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmAccountsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmAccountsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def update(self, request: operations.PutCrmAccountRequest) -> operations.PutCrmAccountResponse:
         r"""Update Account
         Update an existing Account
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/account"
+        url = base_url.removesuffix('/') + '/crm/account'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmAccountResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmAccountResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmAccountResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/attendees.py` & `vesselapi-3.5.2/src/vesselapi/deals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,208 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Attendees:
-    _client: requests.Session
-    _security_client: requests.Session
+class Deals:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def batch(self, request: operations.GetBatchCrmEventAttendeeRequest) -> operations.GetBatchCrmEventAttendeeResponse:
-        r"""Get Batch Event Attendees
-        Retrieve Event Attendees by a set of Id's
+        
+    def batch(self, request: operations.GetBatchCrmDealRequest) -> operations.GetBatchCrmDealResponse:
+        r"""Get Batch Deals
+        Retrieve Deals by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendee/batch"
+        url = base_url.removesuffix('/') + '/crm/deal/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmEventAttendeeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmEventAttendeeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self) -> operations.PostCrmEventAttendeeResponse:
-        r"""Create Event Attendee
-        Add an Attendee to an Event
+    def create(self, request: operations.PostCrmDealRequest) -> operations.PostCrmDealResponse:
+        r"""Create Deal
+        Create a new Deal
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendee"
+        url = base_url.removesuffix('/') + '/crm/deal'
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request)
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmEventAttendeeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmEventAttendeeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmEventAttendeeRequest) -> operations.GetDetailsCrmEventAttendeeResponse:
-        r"""Get Event Attendee Details
-        Get details about all event attendees. 
+    def details(self, request: operations.GetDetailsCrmDealRequest) -> operations.GetDetailsCrmDealResponse:
+        r"""Get Deal Details
+        Get details about all deals or a particular deal. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendee/details"
+        url = base_url.removesuffix('/') + '/crm/deal/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmEventAttendeeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmEventAttendeeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmEventAttendeeRequest) -> operations.GetOneCrmEventAttendeeResponse:
-        r"""Get Event Attendee
-        Retrieve a single Event Attendee by Id
+    def find(self, request: operations.GetOneCrmDealRequest) -> operations.GetOneCrmDealResponse:
+        r"""Get Deal
+        Retrieve a single Deal by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendee"
+        url = base_url.removesuffix('/') + '/crm/deal'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmEventAttendeeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmEventAttendeeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmEventAttendeesRequest) -> operations.GetAllCrmEventAttendeesResponse:
-        r"""Get All Event Attendees
-        Retrieve all Attendees for all Events
+    def list(self, request: operations.GetAllCrmDealsRequest) -> operations.GetAllCrmDealsResponse:
+        r"""Get All Deals
+        Retrieve all Deals
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendees"
+        url = base_url.removesuffix('/') + '/crm/deals'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmEventAttendeesResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmEventAttendeesResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmEventAttendeesRequest) -> operations.SearchCrmEventAttendeesResponse:
-        r"""Search Event Attendees
-        Search all Event Attendees using filters
+    def search(self, request: operations.SearchCrmDealsRequest) -> operations.SearchCrmDealsResponse:
+        r"""Search Deals
+        Search all Deals using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendees/search"
+        url = base_url.removesuffix('/') + '/crm/deals/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmEventAttendeesResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmEventAttendeesResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self) -> operations.PutCrmEventAttendeeResponse:
-        r"""Update Event Attendee
-        Update the status of an event attendee
+    def update(self, request: operations.PutCrmDealRequest) -> operations.PutCrmDealResponse:
+        r"""Update Deal
+        Update an existing Deal
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/attendee"
+        url = base_url.removesuffix('/') + '/crm/deal'
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request)
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmEventAttendeeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmEventAttendeeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmDealResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/connections.py` & `vesselapi-3.5.2/src/vesselapi/connections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,97 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Connections:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def delete(self, request: operations.DeleteConnectionRequest) -> operations.DeleteConnectionResponse:
         r"""Delete Connection
         Remove a connection for a given `connectionId`. Removing a connection disconnects the user's CRM so they'll need to re-authenticate should they want to re-connect their CRM.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/connection/connection"
+        url = base_url.removesuffix('/') + '/connection/connection'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = utils.configure_security_client(self._client, request.security)
         
-        r = client.request("DELETE", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteConnectionResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
+        if http_res.status_code == 200:
             pass
 
         return res
 
-    
     def find(self, request: operations.GetOneConnectionRequest) -> operations.GetOneConnectionResponse:
         r"""Get Connection
         Get info about a connection for a given accessToken.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/connection/connection"
+        url = base_url.removesuffix('/') + '/connection/connection'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneConnectionResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneConnectionResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneConnectionResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self) -> operations.GetAllCrmConnectionsResponse:
         r"""Get All Connections
         List all established connections for a workspace
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/connection/connections"
+        url = base_url.removesuffix('/') + '/connection/connections'
         
         
         client = self._security_client
         
-        r = client.request("GET", url)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmConnectionsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmConnectionsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmConnectionsResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/contacts.py` & `vesselapi-3.5.2/src/vesselapi/leads.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,215 +1,210 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Contacts:
-    _client: requests.Session
-    _security_client: requests.Session
+class Leads:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def batch(self, request: operations.GetBatchCrmContactRequest) -> operations.GetBatchCrmContactResponse:
-        r"""Get Batch Contacts
-        Retrieve Contacts by a set of Id's
+        
+    def batch(self, request: operations.GetBatchCrmLeadRequest) -> operations.GetBatchCrmLeadResponse:
+        r"""Get Batch Leads
+        Retrieve Leads by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contact/batch"
+        url = base_url.removesuffix('/') + '/crm/lead/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmContactResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmContactResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmContactRequest) -> operations.PostCrmContactResponse:
-        r"""Create Contact
-        Create a new contact.
+    def create(self, request: operations.PostCrmLeadRequest) -> operations.PostCrmLeadResponse:
+        r"""Create Lead
+        Create a new Lead
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contact"
+        url = base_url.removesuffix('/') + '/crm/lead'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmContactResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmContactResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmContactRequest) -> operations.GetDetailsCrmContactResponse:
-        r"""Get Contact Details
-        Get details about all contacts. 
+    def details(self, request: operations.GetDetailsCrmLeadRequest) -> operations.GetDetailsCrmLeadResponse:
+        r"""Get Lead Details
+        Get details about all leads. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contact/details"
+        url = base_url.removesuffix('/') + '/crm/lead/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmContactResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmContactResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmContactRequest) -> operations.GetOneCrmContactResponse:
-        r"""Get Contact
-        Retrieve a Contact by either Id or email. When both email and Id are included, Id will take priority.
+    def find(self, request: operations.GetOneCrmLeadRequest) -> operations.GetOneCrmLeadResponse:
+        r"""Get Lead
+        Retrieve a single Lead by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contact"
+        url = base_url.removesuffix('/') + '/crm/lead'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmContactResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmContactResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmContactsRequest) -> operations.GetAllCrmContactsResponse:
-        r"""Get All Contacts
-        Retrieve all Contacts
+    def list(self, request: operations.GetAllCrmLeadsRequest) -> operations.GetAllCrmLeadsResponse:
+        r"""Get All Leads
+        Retrieve all leads.
+        *CRM Caveats*:
+        - Pipedrive: Only `jobTitle` is returned when querying for all leads
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contacts"
+        url = base_url.removesuffix('/') + '/crm/leads'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmContactsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmContactsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmContactsRequest) -> operations.SearchCrmContactsResponse:
-        r"""Search Contacts
-        Search all Contacts using filters
+    def search(self, request: operations.SearchCrmLeadsRequest) -> operations.SearchCrmLeadsResponse:
+        r"""Search Leads
+        Search all Leads using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contacts/search"
+        url = base_url.removesuffix('/') + '/crm/leads/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmContactsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmContactsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmContactRequest) -> operations.PutCrmContactResponse:
-        r"""Update Contact
-        Update an existing Contact.
+    def update(self, request: operations.PutCrmLeadRequest) -> operations.PutCrmLeadResponse:
+        r"""Update Lead
+        Update an existing Lead by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/contact"
+        url = base_url.removesuffix('/') + '/crm/lead'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmContactResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmContactResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmLeadResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/deals.py` & `vesselapi-3.5.2/src/vesselapi/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,208 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Deals:
-    _client: requests.Session
-    _security_client: requests.Session
+class Events:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def batch(self, request: operations.GetBatchCrmDealRequest) -> operations.GetBatchCrmDealResponse:
-        r"""Get Batch Deals
-        Retrieve Deals by a set of Id's
+        
+    def batch(self, request: operations.GetBatchCrmEventRequest) -> operations.GetBatchCrmEventResponse:
+        r"""Get Batch Events
+        Retrieve Events by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deal/batch"
+        url = base_url.removesuffix('/') + '/crm/event/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmDealResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmDealResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmDealRequest) -> operations.PostCrmDealResponse:
-        r"""Create Deal
-        Create a new Deal
+    def create(self, request: operations.PostCrmEventRequest) -> operations.PostCrmEventResponse:
+        r"""Create Event
+        Create a new Event.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deal"
+        url = base_url.removesuffix('/') + '/crm/event'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmDealResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmDealResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmDealRequest) -> operations.GetDetailsCrmDealResponse:
-        r"""Get Deal Details
-        Get details about all deals or a particular deal. 
+    def details(self, request: operations.GetDetailsCrmEventRequest) -> operations.GetDetailsCrmEventResponse:
+        r"""Get Event Details
+        Get details about all events. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deal/details"
+        url = base_url.removesuffix('/') + '/crm/event/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmDealResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmDealResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmDealRequest) -> operations.GetOneCrmDealResponse:
-        r"""Get Deal
-        Retrieve a single Deal by Id
+    def find(self, request: operations.GetOneCrmEventRequest) -> operations.GetOneCrmEventResponse:
+        r"""Get Event
+        Retrieve a single Event by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deal"
+        url = base_url.removesuffix('/') + '/crm/event'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmDealResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmDealResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmDealsRequest) -> operations.GetAllCrmDealsResponse:
-        r"""Get All Deals
-        Retrieve all Deals
+    def list(self, request: operations.GetAllCrmEventsRequest) -> operations.GetAllCrmEventsResponse:
+        r"""Get All Events
+        Retrieve all Events
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deals"
+        url = base_url.removesuffix('/') + '/crm/events'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmDealsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmDealsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmDealsRequest) -> operations.SearchCrmDealsResponse:
-        r"""Search Deals
-        Search all Deals using filters
+    def search(self, request: operations.SearchCrmEventsRequest) -> operations.SearchCrmEventsResponse:
+        r"""Search Events
+        Search all Events using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deals/search"
+        url = base_url.removesuffix('/') + '/crm/events/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmDealsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmDealsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmDealRequest) -> operations.PutCrmDealResponse:
-        r"""Update Deal
-        Update an existing Deal
+    def update(self, request: operations.PutCrmEventRequest) -> operations.PutCrmEventResponse:
+        r"""Update Event
+        Update an existing Event by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/deal"
+        url = base_url.removesuffix('/') + '/crm/event'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmDealResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmDealResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEventResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/emails.py` & `vesselapi-3.5.2/src/vesselapi/emails.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,220 +1,213 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Emails:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def batch(self, request: operations.GetBatchCrmEmailRequest) -> operations.GetBatchCrmEmailResponse:
         r"""Get Batch Emails
         Retrieve Email by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/email/batch"
+        url = base_url.removesuffix('/') + '/crm/email/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmEmailResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmEmailResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def create(self, request: operations.PostCrmEmailRequest) -> operations.PostCrmEmailResponse:
         r"""Create Email
         Create a new Email.
         *CRM Caveats*:
         
         - Pipedrive: Not supported.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/email"
+        url = base_url.removesuffix('/') + '/crm/email'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmEmailResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmEmailResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmEmailRequest) -> operations.GetDetailsCrmEmailResponse:
         r"""Get Email Details
         Get details about all emails. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/email/details"
+        url = base_url.removesuffix('/') + '/crm/email/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmEmailResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmEmailResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmEmailRequest) -> operations.GetOneCrmEmailResponse:
         r"""Get Email
         Retrieve a single Task by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/email"
+        url = base_url.removesuffix('/') + '/crm/email'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmEmailResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmEmailResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmEmailsRequest) -> operations.GetAllCrmEmailsResponse:
         r"""Get All Emails
         Retrieve all Emails
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/emails"
+        url = base_url.removesuffix('/') + '/crm/emails'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmEmailsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmEmailsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEmailsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmEmailsRequest) -> operations.SearchCrmEmailsResponse:
         r"""Search Emails
         Search all Emails using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/emails/search"
+        url = base_url.removesuffix('/') + '/crm/emails/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmEmailsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmEmailsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEmailsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def update(self, request: operations.PutCrmEmailRequest) -> operations.PutCrmEmailResponse:
         r"""Update Email
         Update an Email by Id.
         *CRM Caveats*:
         - Pipedrive: Not supported.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/email"
+        url = base_url.removesuffix('/') + '/crm/email'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmEmailResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmEmailResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEmailResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/events.py` & `vesselapi-3.5.2/src/vesselapi/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,215 +1,210 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Events:
-    _client: requests.Session
-    _security_client: requests.Session
+class Tasks:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def batch(self, request: operations.GetBatchCrmEventRequest) -> operations.GetBatchCrmEventResponse:
-        r"""Get Batch Events
-        Retrieve Events by a set of Id's
+        
+    def batch(self, request: operations.GetBatchCrmTaskRequest) -> operations.GetBatchCrmTaskResponse:
+        r"""Get Batch Tasks
+        Retrieve Tasks by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/batch"
+        url = base_url.removesuffix('/') + '/crm/task/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmEventResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmEventResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmEventRequest) -> operations.PostCrmEventResponse:
-        r"""Create Event
-        Create a new Event.
+    def create(self, request: operations.PostCrmTaskRequest) -> operations.PostCrmTaskResponse:
+        r"""Create Task
+        Create a new Task.
+        *CRM Caveats*:
+        - Salesforce: You may only associate a Task with either a Lead or a Contact *and* either a Deal or an Account.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event"
+        url = base_url.removesuffix('/') + '/crm/task'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmEventResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmEventResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmEventRequest) -> operations.GetDetailsCrmEventResponse:
-        r"""Get Event Details
-        Get details about all events. 
+    def details(self, request: operations.GetDetailsCrmTaskRequest) -> operations.GetDetailsCrmTaskResponse:
+        r"""Get Task Details
+        Get details about all tasks. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event/details"
+        url = base_url.removesuffix('/') + '/crm/task/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmEventResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmEventResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmEventRequest) -> operations.GetOneCrmEventResponse:
-        r"""Get Event
-        Retrieve a single Event by Id
+    def find(self, request: operations.GetOneCrmTaskRequest) -> operations.GetOneCrmTaskResponse:
+        r"""Get Task
+        Retrieve a single Task by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event"
+        url = base_url.removesuffix('/') + '/crm/task'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmEventResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmEventResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmEventsRequest) -> operations.GetAllCrmEventsResponse:
-        r"""Get All Events
-        Retrieve all Events
+    def list(self, request: operations.GetAllCrmTasksRequest) -> operations.GetAllCrmTasksResponse:
+        r"""Get All Tasks
+        Retrieve all Tasks
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/events"
+        url = base_url.removesuffix('/') + '/crm/tasks'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmEventsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmEventsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmEventsRequest) -> operations.SearchCrmEventsResponse:
-        r"""Search Events
-        Search all Events using filters
+    def search(self, request: operations.SearchCrmTasksRequest) -> operations.SearchCrmTasksResponse:
+        r"""Search Tasks
+        Search all Tasks using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/events/search"
+        url = base_url.removesuffix('/') + '/crm/tasks/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmEventsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmEventsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmEventRequest) -> operations.PutCrmEventResponse:
-        r"""Update Event
-        Update an existing Event by Id
+    def update(self, request: operations.PutCrmTaskRequest) -> operations.PutCrmTaskResponse:
+        r"""Update Task
+        Update an existing Task by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/event"
+        url = base_url.removesuffix('/') + '/crm/task'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmEventResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmEventResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmTaskResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/integrations.py` & `vesselapi-3.5.2/src/vesselapi/links.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Integrations:
-    _client: requests.Session
-    _security_client: requests.Session
+class Links:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def list(self) -> operations.GetAllCrmIntegrationsResponse:
-        r"""Get CRM Integrations
-        Return all of the CRM integrations supported by Vessel.
+        
+    def create(self, request: operations.PostLinkExchangeRequest) -> operations.PostLinkExchangeResponse:
+        r"""Exchange Public Token for Access Token
+        Exchanges the public token for an access token used to interact with the account. Store the access token in a secure location.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/connection/crm/integrations"
+        url = base_url.removesuffix('/') + '/link/exchange'
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request)
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
-        client = self._security_client
+        client = utils.configure_security_client(self._client, request.security)
         
-        r = client.request("GET", url)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmIntegrationsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostLinkExchangeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmIntegrationsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostLinkExchangeResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/leads.py` & `vesselapi-3.5.2/src/vesselapi/contacts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,208 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Leads:
-    _client: requests.Session
-    _security_client: requests.Session
+class Contacts:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def batch(self, request: operations.GetBatchCrmLeadRequest) -> operations.GetBatchCrmLeadResponse:
-        r"""Get Batch Leads
-        Retrieve Leads by a set of Id's
+        
+    def batch(self, request: operations.GetBatchCrmContactRequest) -> operations.GetBatchCrmContactResponse:
+        r"""Get Batch Contacts
+        Retrieve Contacts by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/lead/batch"
+        url = base_url.removesuffix('/') + '/crm/contact/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmLeadResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmLeadResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmLeadRequest) -> operations.PostCrmLeadResponse:
-        r"""Create Lead
-        Create a new Lead
+    def create(self, request: operations.PostCrmContactRequest) -> operations.PostCrmContactResponse:
+        r"""Create Contact
+        Create a new contact.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/lead"
+        url = base_url.removesuffix('/') + '/crm/contact'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmLeadResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmLeadResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmLeadRequest) -> operations.GetDetailsCrmLeadResponse:
-        r"""Get Lead Details
-        Get details about all leads. 
+    def details(self, request: operations.GetDetailsCrmContactRequest) -> operations.GetDetailsCrmContactResponse:
+        r"""Get Contact Details
+        Get details about all contacts. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/lead/details"
+        url = base_url.removesuffix('/') + '/crm/contact/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmLeadResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmLeadResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmLeadRequest) -> operations.GetOneCrmLeadResponse:
-        r"""Get Lead
-        Retrieve a single Lead by Id
+    def find(self, request: operations.GetOneCrmContactRequest) -> operations.GetOneCrmContactResponse:
+        r"""Get Contact
+        Retrieve a Contact by either Id or email. When both email and Id are included, Id will take priority.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/lead"
+        url = base_url.removesuffix('/') + '/crm/contact'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmLeadResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmLeadResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmLeadsRequest) -> operations.GetAllCrmLeadsResponse:
-        r"""Get All Leads
-        Retrieve all leads.
-        *CRM Caveats*:
-        - Pipedrive: Only `jobTitle` is returned when querying for all leads
+    def list(self, request: operations.GetAllCrmContactsRequest) -> operations.GetAllCrmContactsResponse:
+        r"""Get All Contacts
+        Retrieve all Contacts
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/leads"
+        url = base_url.removesuffix('/') + '/crm/contacts'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmLeadsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmLeadsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmLeadsRequest) -> operations.SearchCrmLeadsResponse:
-        r"""Search Leads
-        Search all Leads using filters
+    def search(self, request: operations.SearchCrmContactsRequest) -> operations.SearchCrmContactsResponse:
+        r"""Search Contacts
+        Search all Contacts using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/leads/search"
+        url = base_url.removesuffix('/') + '/crm/contacts/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmLeadsResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmLeadsResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmLeadRequest) -> operations.PutCrmLeadResponse:
-        r"""Update Lead
-        Update an existing Lead by Id
+    def update(self, request: operations.PutCrmContactRequest) -> operations.PutCrmContactResponse:
+        r"""Update Contact
+        Update an existing Contact.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/lead"
+        url = base_url.removesuffix('/') + '/crm/contact'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmLeadResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmLeadResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmContactResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/links.py` & `vesselapi-3.5.2/src/vesselapi/integrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,46 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Links:
-    _client: requests.Session
-    _security_client: requests.Session
+class Integrations:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
-    def create(self, request: operations.PostLinkExchangeRequest) -> operations.PostLinkExchangeResponse:
-        r"""Exchange Public Token for Access Token
-        Exchanges the public token for an access token used to interact with the account. Store the access token in a secure location.
+        
+    def list(self) -> operations.GetAllCrmIntegrationsResponse:
+        r"""Get CRM Integrations
+        Return all of the CRM integrations supported by Vessel.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/link/exchange"
+        url = base_url.removesuffix('/') + '/connection/crm/integrations'
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
         
-        client = utils.configure_security_client(self._client, request.security)
+        client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostLinkExchangeResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostLinkExchangeResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmIntegrationsResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/__init__.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -73,8 +73,8 @@
 from .search_crm_event_attendees import *
 from .search_crm_events import *
 from .search_crm_leads import *
 from .search_crm_notes import *
 from .search_crm_tasks import *
 from .search_crm_users import *
 
-__all__ = ["DeleteConnectionRequest","DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequest","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsQueryParams","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsQueryParams","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsQueryParams","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsQueryParams","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesQueryParams","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsQueryParams","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsQueryParams","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesQueryParams","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksQueryParams","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersQueryParams","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountQueryParams","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmContactQueryParams","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealQueryParams","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailQueryParams","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeQueryParams","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventQueryParams","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadQueryParams","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteQueryParams","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskQueryParams","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserQueryParams","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountQueryParams","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmContactQueryParams","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealQueryParams","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailQueryParams","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeQueryParams","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventQueryParams","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadQueryParams","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteQueryParams","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskQueryParams","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserQueryParams","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionQueryParams","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountQueryParams","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmContactQueryParams","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealQueryParams","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailQueryParams","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeQueryParams","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventQueryParams","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadQueryParams","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteQueryParams","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskQueryParams","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserQueryParams","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookQueryParams","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequest","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmContactRequest","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequest","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequest","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequest","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequest","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequest","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequest","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyMethodEnum","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmTaskRequest","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequest","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationIDEnum","PostLinkExchangeSecurity","PostLinkTokenRequest","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequest","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequest","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmContactRequest","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequest","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequest","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequest","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequest","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequest","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequest","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsQueryParams","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmContactsQueryParams","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsQueryParams","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsQueryParams","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesQueryParams","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsQueryParams","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsQueryParams","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesQueryParams","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksQueryParams","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersQueryParams","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
+__all__ = ["DeleteConnectionRequest","DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequest","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsQueryParams","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsQueryParams","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsQueryParams","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsQueryParams","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesQueryParams","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsQueryParams","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsQueryParams","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesQueryParams","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksQueryParams","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersQueryParams","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountQueryParams","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmContactQueryParams","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealQueryParams","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailQueryParams","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeQueryParams","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventQueryParams","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadQueryParams","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteQueryParams","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskQueryParams","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserQueryParams","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountQueryParams","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmContactQueryParams","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealQueryParams","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailQueryParams","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeQueryParams","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventQueryParams","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadQueryParams","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteQueryParams","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskQueryParams","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserQueryParams","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionQueryParams","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountQueryParams","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmContactQueryParams","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealQueryParams","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailQueryParams","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeQueryParams","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventQueryParams","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadQueryParams","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteQueryParams","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskQueryParams","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserQueryParams","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookQueryParams","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequest","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmContactRequest","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequest","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequest","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequest","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequest","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequest","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequest","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyMethodEnum","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmTaskRequest","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequest","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationIDEnum","PostLinkExchangeSecurity","PostLinkTokenRequest","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequest","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequest","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmContactRequest","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequest","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequest","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequest","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequest","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequest","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequest","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsQueryParams","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmContactsQueryParams","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsQueryParams","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsQueryParams","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesQueryParams","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsQueryParams","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsQueryParams","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesQueryParams","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksQueryParams","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersQueryParams","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/delete_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteConnectionRequestBody:
-    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('connectionId') }})
+class DeleteConnectionSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteConnectionSecurity:
-    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
+class DeleteConnectionRequestBody:
+    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
     
 
 @dataclasses.dataclass
 class DeleteConnectionRequest:
     security: DeleteConnectionSecurity = dataclasses.field()
     request: Optional[DeleteConnectionRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
 class DeleteConnectionResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/delete_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DeleteWebhookRequestBody:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken'), 'exclude': lambda f: f is None }})
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('webhookId'), 'exclude': lambda f: f is None }})
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class DeleteWebhookRequest:
     request: Optional[DeleteWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
 class DeleteWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmAccountsRequest:
     query_params: GetAllCrmAccountsQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmAccountsResponseBody:
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accounts'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmAccountsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmAccountsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_connections.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import connection as shared_connection
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmConnectionsResponseBody:
-    connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('connections'), 'exclude': lambda f: f is None }})
+    connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connections'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmConnectionsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmConnectionsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import contact as shared_contact
+import requests as requests_http
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmContactsQueryParams:
+class GetBatchCrmAccountQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetAllCrmContactsRequest:
-    query_params: GetAllCrmContactsQueryParams = dataclasses.field()
+class GetBatchCrmAccountRequest:
+    query_params: GetBatchCrmAccountQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmContactsResponseBody:
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contacts'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmAccountResponseBody:
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmContactsResponse:
+class GetBatchCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetAllCrmContactsResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetBatchCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import deal as shared_deal
+import requests as requests_http
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmDealsQueryParams:
+class GetBatchCrmNoteQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetAllCrmDealsRequest:
-    query_params: GetAllCrmDealsQueryParams = dataclasses.field()
+class GetBatchCrmNoteRequest:
+    query_params: GetBatchCrmNoteQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmDealsResponseBody:
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('deals'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmNoteResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmDealsResponse:
+class GetBatchCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetAllCrmDealsResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmEmailsRequest:
     query_params: GetAllCrmEmailsQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmEmailsResponseBody:
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('emails'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmEmailsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmEmailsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmEventAttendeesRequest:
     query_params: GetAllCrmEventAttendeesQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmEventAttendeesResponseBody:
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendees'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmEventAttendeesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmEventsRequest:
     query_params: GetAllCrmEventsQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmEventsResponseBody:
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('events'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmEventsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmEventsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_integrations.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import integration as shared_integration
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponseBody:
-    integrations: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('integrations'), 'exclude': lambda f: f is None }})
+    integrations: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrations'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmIntegrationsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmLeadsRequest:
     query_params: GetAllCrmLeadsQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmLeadsResponseBody:
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('leads'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmLeadsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import note as shared_note
+import requests as requests_http
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmNotesQueryParams:
+class GetBatchCrmUserQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetAllCrmNotesRequest:
-    query_params: GetAllCrmNotesQueryParams = dataclasses.field()
+class GetBatchCrmUserRequest:
+    query_params: GetBatchCrmUserQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmNotesResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('notes'), 'exclude': lambda f: f is None }})
+class GetBatchCrmUserResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmNotesResponse:
+class GetBatchCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetAllCrmNotesResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_tasks.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmTasksRequest:
     query_params: GetAllCrmTasksQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmTasksResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('tasks'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmTasksResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_all_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -18,17 +19,18 @@
 class GetAllCrmUsersRequest:
     query_params: GetAllCrmUsersQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmUsersResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('users'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmUsersResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_lead.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import account as shared_account
+import requests as requests_http
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmAccountQueryParams:
+class GetBatchCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmAccountRequest:
-    query_params: GetBatchCrmAccountQueryParams = dataclasses.field()
+class GetBatchCrmLeadRequest:
+    query_params: GetBatchCrmLeadQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmAccountResponseBody:
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accounts'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+class GetBatchCrmLeadResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmAccountResponse:
+class GetBatchCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmAccountResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetBatchCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import contact as shared_contact
+import requests as requests_http
+from ..shared import webhookmetadata as shared_webhookmetadata
+from ..shared import webhookmetadatacreate as shared_webhookmetadatacreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmContactQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
+class PostWebhookRequestBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    webhook: Optional[shared_webhookmetadatacreate.WebhookMetadataCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmContactRequest:
-    query_params: GetBatchCrmContactQueryParams = dataclasses.field()
+class PostWebhookRequest:
+    request: Optional[PostWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmContactResponseBody:
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contacts'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+class PostWebhookResponseBody:
+    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmContactResponse:
+class PostWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmContactResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostWebhookResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_deal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmDealQueryParams:
+class GetOneCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmDealRequest:
-    query_params: GetBatchCrmDealQueryParams = dataclasses.field()
+class GetOneCrmDealRequest:
+    query_params: GetOneCrmDealQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmDealResponseBody:
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('deals'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+class GetOneCrmDealResponseBody:
+    deal: Optional[shared_deal.Deal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmDealResponse:
+class GetOneCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -17,17 +18,18 @@
 class GetBatchCrmEmailRequest:
     query_params: GetBatchCrmEmailQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetBatchCrmEmailResponseBody:
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('emails'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetBatchCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetBatchCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import event as shared_event
+import requests as requests_http
+from ..shared import eventupdate as shared_eventupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmEventQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
+class PutCrmEventRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmEventRequest:
-    query_params: GetBatchCrmEventQueryParams = dataclasses.field()
+class PutCrmEventRequest:
+    request: Optional[PutCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmEventResponseBody:
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('events'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+class PutCrmEventResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmEventResponse:
+class PutCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmEventResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -17,17 +18,18 @@
 class GetBatchCrmEventAttendeeRequest:
     query_params: GetBatchCrmEventAttendeeQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetBatchCrmEventAttendeeResponseBody:
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendees'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetBatchCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetBatchCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmLeadQueryParams:
+class GetOneCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmLeadRequest:
-    query_params: GetBatchCrmLeadQueryParams = dataclasses.field()
+class GetOneCrmLeadRequest:
+    query_params: GetOneCrmLeadQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmLeadResponseBody:
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('leads'), 'exclude': lambda f: f is None }})
+class GetOneCrmLeadResponseBody:
+    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmLeadResponse:
+class GetOneCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmLeadResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmNoteQueryParams:
+class GetOneCrmNoteQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmNoteRequest:
-    query_params: GetBatchCrmNoteQueryParams = dataclasses.field()
+class GetOneCrmNoteRequest:
+    query_params: GetOneCrmNoteQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmNoteResponseBody:
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('notes'), 'exclude': lambda f: f is None }})
+class GetOneCrmNoteResponseBody:
+    note: Optional[shared_note.Note] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmNoteResponse:
+class GetOneCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -17,17 +18,18 @@
 class GetBatchCrmTaskRequest:
     query_params: GetBatchCrmTaskQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetBatchCrmTaskResponseBody:
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('tasks'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetBatchCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetBatchCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_batch_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmUserQueryParams:
+class GetOneCrmUserQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmUserRequest:
-    query_params: GetBatchCrmUserQueryParams = dataclasses.field()
+class GetOneCrmUserRequest:
+    query_params: GetOneCrmUserQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmUserResponseBody:
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('users'), 'exclude': lambda f: f is None }})
+class GetOneCrmUserResponseBody:
+    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmUserResponse:
+class GetOneCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmAccountQueryParams:
+class GetDetailsCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmAccountRequest:
-    query_params: GetDetailsCrmAccountQueryParams = dataclasses.field()
+class GetDetailsCrmDealRequest:
+    query_params: GetDetailsCrmDealQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmDealResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponse:
+class GetDetailsCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetDetailsCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -17,17 +18,18 @@
 class GetDetailsCrmContactRequest:
     query_params: GetDetailsCrmContactQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetDetailsCrmContactResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetDetailsCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetDetailsCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import field as shared_field
+import requests as requests_http
+from ..shared import emailupdate as shared_emailupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmDealQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+class PutCrmEmailRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    email: Optional[shared_emailupdate.EmailUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmDealRequest:
-    query_params: GetDetailsCrmDealQueryParams = dataclasses.field()
+class PutCrmEmailRequest:
+    request: Optional[PutCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmDealResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class PutCrmEmailResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmDealResponse:
+class PutCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmDealResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -17,17 +18,18 @@
 class GetDetailsCrmEmailRequest:
     query_params: GetDetailsCrmEmailQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetDetailsCrmEmailResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetDetailsCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetDetailsCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmEventQueryParams:
+class GetDetailsCrmAccountQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmEventRequest:
-    query_params: GetDetailsCrmEventQueryParams = dataclasses.field()
+class GetDetailsCrmAccountRequest:
+    query_params: GetDetailsCrmAccountQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEventResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmAccountResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmEventResponse:
+class GetDetailsCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmEventResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeQueryParams:
+class GetDetailsCrmUserQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeRequest:
-    query_params: GetDetailsCrmEventAttendeeQueryParams = dataclasses.field()
+class GetDetailsCrmUserRequest:
+    query_params: GetDetailsCrmUserQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmUserResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponse:
+class GetDetailsCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import field as shared_field
+import requests as requests_http
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmLeadQueryParams:
+class GetOneCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmLeadRequest:
-    query_params: GetDetailsCrmLeadQueryParams = dataclasses.field()
+class GetOneCrmTaskRequest:
+    query_params: GetOneCrmTaskQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmTaskResponseBody:
+    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponse:
+class GetOneCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmNoteQueryParams:
+class GetDetailsCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmNoteRequest:
-    query_params: GetDetailsCrmNoteQueryParams = dataclasses.field()
+class GetDetailsCrmTaskRequest:
+    query_params: GetDetailsCrmTaskQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmTaskResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponse:
+class GetDetailsCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmNoteResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import field as shared_field
+import requests as requests_http
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmTaskQueryParams:
+class GetOneCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmTaskRequest:
-    query_params: GetDetailsCrmTaskQueryParams = dataclasses.field()
+class GetOneCrmEmailRequest:
+    query_params: GetOneCrmEmailQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmEmailResponseBody:
+    email: Optional[shared_email.Email] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponse:
+class GetOneCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_details_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import field as shared_field
+import requests as requests_http
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmUserQueryParams:
+class GetOneCrmAccountQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmUserRequest:
-    query_params: GetDetailsCrmUserQueryParams = dataclasses.field()
+class GetOneCrmAccountRequest:
+    query_params: GetOneCrmAccountQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmUserResponseBody:
-    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmAccountResponseBody:
+    account: Optional[shared_account.Account] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmUserResponse:
+class GetOneCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import connection as shared_connection
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -15,16 +16,17 @@
 class GetOneConnectionRequest:
     query_params: GetOneConnectionQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetOneConnectionResponseBody:
-    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('connection'), 'exclude': lambda f: f is None }})
+    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetOneConnectionResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetOneConnectionResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import account as shared_account
+import requests as requests_http
+from ..shared import emailcreate as shared_emailcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmAccountQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+class PostCrmEmailRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmAccountRequest:
-    query_params: GetOneCrmAccountQueryParams = dataclasses.field()
+class PostCrmEmailRequest:
+    request: Optional[PostCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmAccountResponseBody:
-    account: Optional[shared_account.Account] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('account'), 'exclude': lambda f: f is None }})
+class PostCrmEmailResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmAccountResponse:
+class PostCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmAccountResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import contact as shared_contact
+import requests as requests_http
+from ..shared import accountcreate as shared_accountcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmContactQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'email', 'style': 'form', 'explode': True }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+class PostCrmAccountRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    account: shared_accountcreate.AccountCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmContactRequest:
-    query_params: GetOneCrmContactQueryParams = dataclasses.field()
+class PostCrmAccountRequest:
+    request: Optional[PostCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmContactResponseBody:
-    contact: Optional[shared_contact.Contact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contact'), 'exclude': lambda f: f is None }})
+class PostCrmAccountResponseBody:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmContactResponse:
+class PostCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmContactResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import deal as shared_deal
+import requests as requests_http
+from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmDealQueryParams:
+class GetOneCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetOneCrmDealRequest:
-    query_params: GetOneCrmDealQueryParams = dataclasses.field()
+class GetOneCrmEventRequest:
+    query_params: GetOneCrmEventQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmDealResponseBody:
-    deal: Optional[shared_deal.Deal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('deal'), 'exclude': lambda f: f is None }})
+class GetOneCrmEventResponseBody:
+    event: Optional[shared_event.Event] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmDealResponse:
+class GetOneCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmDealResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import email as shared_email
+import requests as requests_http
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmEmailQueryParams:
+class GetOneCrmEventAttendeeQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEmailRequest:
-    query_params: GetOneCrmEmailQueryParams = dataclasses.field()
+class GetOneCrmEventAttendeeRequest:
+    query_params: GetOneCrmEventAttendeeQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmEmailResponseBody:
-    email: Optional[shared_email.Email] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
+class GetOneCrmEventAttendeeResponseBody:
+    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEmailResponse:
+class GetOneCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmEmailResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import event as shared_event
+import requests as requests_http
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmEventQueryParams:
+class GetOneCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'email', 'style': 'form', 'explode': True }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEventRequest:
-    query_params: GetOneCrmEventQueryParams = dataclasses.field()
+class GetOneCrmContactRequest:
+    query_params: GetOneCrmContactQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmEventResponseBody:
-    event: Optional[shared_event.Event] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('event'), 'exclude': lambda f: f is None }})
+class GetOneCrmContactResponseBody:
+    contact: Optional[shared_contact.Contact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEventResponse:
+class GetOneCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmEventResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetOneCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import eventattendee as shared_eventattendee
+import requests as requests_http
+from ..shared import eventattendeeupdate as shared_eventattendeeupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetOneCrmEventAttendeeQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    
-
-@dataclasses.dataclass
-class GetOneCrmEventAttendeeRequest:
-    query_params: GetOneCrmEventAttendeeQueryParams = dataclasses.field()
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeResponseBody:
-    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendee'), 'exclude': lambda f: f is None }})
+class PutCrmEventAttendeeResponseBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeResponse:
+class PutCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import lead as shared_lead
+import requests as requests_http
+from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmLeadQueryParams:
+class GetBatchCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
 @dataclasses.dataclass
-class GetOneCrmLeadRequest:
-    query_params: GetOneCrmLeadQueryParams = dataclasses.field()
+class GetBatchCrmDealRequest:
+    query_params: GetBatchCrmDealQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmLeadResponseBody:
-    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lead'), 'exclude': lambda f: f is None }})
+class GetBatchCrmDealResponseBody:
+    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmLeadResponse:
+class GetBatchCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import note as shared_note
+import requests as requests_http
+from ..shared import taskcreate as shared_taskcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmNoteQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+class PostCrmTaskRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmNoteRequest:
-    query_params: GetOneCrmNoteQueryParams = dataclasses.field()
+class PostCrmTaskRequest:
+    request: Optional[PostCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmNoteResponseBody:
-    note: Optional[shared_note.Note] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('note'), 'exclude': lambda f: f is None }})
+class PostCrmTaskResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmNoteResponse:
+class PostCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmNoteResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import task as shared_task
+import requests as requests_http
+from ..shared import notecreate as shared_notecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmTaskQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+class PostCrmNoteRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmTaskRequest:
-    query_params: GetOneCrmTaskQueryParams = dataclasses.field()
+class PostCrmNoteRequest:
+    request: Optional[PostCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmTaskResponseBody:
-    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('task'), 'exclude': lambda f: f is None }})
+class PostCrmNoteResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmTaskResponse:
+class PostCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetOneCrmUserQueryParams:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    
-
-@dataclasses.dataclass
-class GetOneCrmUserRequest:
-    query_params: GetOneCrmUserQueryParams = dataclasses.field()
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmUserResponseBody:
-    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('user'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetOneCrmUserResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
+class EmailUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/get_one_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import webhookmetadata as shared_webhookmetadata
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
@@ -16,16 +17,17 @@
 class GetOneWebhookRequest:
     query_params: GetOneWebhookQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetOneWebhookResponseBody:
-    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('webhook'), 'exclude': lambda f: f is None }})
+    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetOneWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetOneWebhookResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import accountcreate as shared_accountcreate
+import requests as requests_http
+from ..shared import accountupdate as shared_accountupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmAccountRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    account: shared_accountcreate.AccountCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('account') }})
+class PutCrmAccountRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    account: shared_accountupdate.AccountUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmAccountRequest:
-    request: Optional[PostCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmAccountRequest:
+    request: Optional[PutCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmAccountResponseBody:
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
+class PutCrmAccountResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmAccountResponse:
+class PutCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmAccountResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import contactcreate as shared_contactcreate
+import requests as requests_http
+from ..shared import dealupdate as shared_dealupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmContactRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contact') }})
+class PutCrmDealRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    deal: shared_dealupdate.DealUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmContactRequest:
-    request: Optional[PostCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmDealRequest:
+    request: Optional[PutCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmContactResponseBody:
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
+class PutCrmDealResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmContactResponse:
+class PutCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/note.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import dealcreate as shared_dealcreate
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmDealRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('deal') }})
-    
-
-@dataclasses.dataclass
-class PostCrmDealRequest:
-    request: Optional[PostCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class NoteAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmDealResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class Note:
+    r"""Note
+    A Note attached to some CRM Object. 
+    """
     
-
-@dataclasses.dataclass
-class PostCrmDealResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
+    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import emailcreate as shared_emailcreate
+import requests as requests_http
+from ..shared import leadcreate as shared_leadcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEmailRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
+class PostCrmLeadRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead') }})
     
 
 @dataclasses.dataclass
-class PostCrmEmailRequest:
-    request: Optional[PostCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PostCrmLeadRequest:
+    request: Optional[PostCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEmailResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PostCrmLeadResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmEmailResponse:
+class PostCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import eventcreate as shared_eventcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmEventRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('event'), 'exclude': lambda f: f is None }})
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostCrmEventRequest:
     request: Optional[PostCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmEventResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
 class PostCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import eventattendeecreate as shared_eventattendeecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmEventAttendeeResponseBody:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken'), 'exclude': lambda f: f is None }})
-    event_attendee: Optional[shared_eventattendeecreate.EventAttendeeCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendee'), 'exclude': lambda f: f is None }})
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    event_attendee: Optional[shared_eventattendeecreate.EventAttendeeCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import leadcreate as shared_leadcreate
+import requests as requests_http
+from ..shared import contactcreate as shared_contactcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmLeadRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('lead') }})
+class PostCrmContactRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
     
 
 @dataclasses.dataclass
-class PostCrmLeadRequest:
-    request: Optional[PostCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PostCrmContactRequest:
+    request: Optional[PostCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmLeadResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PostCrmContactResponseBody:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PostCrmLeadResponse:
+class PostCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import notecreate as shared_notecreate
+import requests as requests_http
+from ..shared import dealcreate as shared_dealcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmNoteRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('note') }})
+class PostCrmDealRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     
 
 @dataclasses.dataclass
-class PostCrmNoteRequest:
-    request: Optional[PostCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PostCrmDealRequest:
+    request: Optional[PostCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmNoteResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PostCrmDealResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmNoteResponse:
+class PostCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_passthrough.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
 class PostCrmPassthroughRequestBodyMethodEnum(str, Enum):
     GET = "GET"
@@ -12,34 +13,35 @@
     PATCH = "PATCH"
     DELETE = "DELETE"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmPassthroughRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    method: PostCrmPassthroughRequestBodyMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('method') }})
-    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('path') }})
-    body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    query: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('query'), 'exclude': lambda f: f is None }})
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    method: PostCrmPassthroughRequestBodyMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
+    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path') }})
+    body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    query: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostCrmPassthroughRequest:
     request: Optional[PostCrmPassthroughRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmPassthroughResponseBody:
-    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    headers: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('headers'), 'exclude': lambda f: f is None }})
-    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('statusCode'), 'exclude': lambda f: f is None }})
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('url'), 'exclude': lambda f: f is None }})
+    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    headers: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('headers'), 'exclude': lambda f: f is None }})
+    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostCrmPassthroughResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostCrmPassthroughResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import taskcreate as shared_taskcreate
+import requests as requests_http
+from ..shared import noteupdate as shared_noteupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmTaskRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('task'), 'exclude': lambda f: f is None }})
+class PutCrmNoteRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
 @dataclasses.dataclass
-class PostCrmTaskRequest:
-    request: Optional[PostCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmNoteRequest:
+    request: Optional[PutCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmTaskResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PutCrmNoteResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmTaskResponse:
+class PutCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_link_exchange.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostLinkExchangeRequestBody:
-    public_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('publicToken') }})
+class PostLinkExchangeSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostLinkExchangeSecurity:
-    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
+class PostLinkExchangeRequestBody:
+    public_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('publicToken') }})
     
 
 @dataclasses.dataclass
 class PostLinkExchangeRequest:
     security: PostLinkExchangeSecurity = dataclasses.field()
     request: Optional[PostLinkExchangeRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
@@ -28,20 +29,21 @@
     HUBSPOT = "hubspot"
     PIPEDRIVE = "pipedrive"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostLinkExchangeResponseBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('connectionId') }})
-    integration_id: PostLinkExchangeResponseBodyIntegrationIDEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('integrationId') }})
-    native_org_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeOrgId') }})
-    native_org_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeOrgURL') }})
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
+    integration_id: PostLinkExchangeResponseBodyIntegrationIDEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
+    native_org_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgId') }})
+    native_org_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL') }})
     
 
 @dataclasses.dataclass
 class PostLinkExchangeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostLinkExchangeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/post_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventattendee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import webhookmetadata as shared_webhookmetadata
-from ..shared import webhookmetadatacreate as shared_webhookmetadatacreate
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostWebhookRequestBody:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken'), 'exclude': lambda f: f is None }})
-    webhook: Optional[shared_webhookmetadatacreate.WebhookMetadataCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('webhook'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class PostWebhookRequest:
-    request: Optional[PostWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class EventAttendeeAssociations:
+    association_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associationId') }})
+    event_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostWebhookResponseBody:
-    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('webhook'), 'exclude': lambda f: f is None }})
+class EventAttendee:
+    r"""EventAttendee
+    Event Attendees hold information about someone who attendeed or was invited to an event. Attendees are always associated with some Event and another person object such as a Contact, Lead, or Other.
+    """
     
-
-@dataclasses.dataclass
-class PostWebhookResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PostWebhookResponseBody] = dataclasses.field(default=None)
+    associated_object_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType') }})
+    associations: EventAttendeeAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import accountupdate as shared_accountupdate
+import requests as requests_http
+from ..shared import contactupdate as shared_contactupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmAccountRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    account: shared_accountupdate.AccountUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('account') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PutCrmContactRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmAccountRequest:
-    request: Optional[PutCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmContactRequest:
+    request: Optional[PutCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmAccountResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PutCrmContactResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmAccountResponse:
+class PutCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmAccountResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeecreate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,17 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import contactupdate as shared_contactupdate
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmContactRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contact') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    
-
-@dataclasses.dataclass
-class PutCrmContactRequest:
-    request: Optional[PutCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PutCrmContactResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    
-
-@dataclasses.dataclass
-class PutCrmContactResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
+class EventAttendeeCreate:
+    associated_object_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType') }})
+    event_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    association_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associationId'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import emailupdate as shared_emailupdate
+import requests as requests_http
+from ..shared import taskupdate as shared_taskupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEmailRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    email: Optional[shared_emailupdate.EmailUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
+class PutCrmTaskRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PutCrmEmailRequest:
-    request: Optional[PutCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmTaskRequest:
+    request: Optional[PutCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEmailResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PutCrmTaskResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmEmailResponse:
+class PutCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmEmailResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import eventupdate as shared_eventupdate
+import requests as requests_http
+from ..shared import leadupdate as shared_leadupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('event'), 'exclude': lambda f: f is None }})
+class PutCrmLeadRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PutCrmEventRequest:
-    request: Optional[PutCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PutCrmLeadRequest:
+    request: Optional[PutCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PutCrmLeadResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmEventResponse:
+class PutCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import eventattendeeupdate as shared_eventattendeeupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventAttendeeResponseBody:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken'), 'exclude': lambda f: f is None }})
-    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendee'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class PutCrmEventAttendeeResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+class WebhookMetadata:
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
+    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import leadupdate as shared_leadupdate
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmLeadRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lead'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class PutCrmLeadRequest:
-    request: Optional[PutCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PutCrmLeadResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    
-
-@dataclasses.dataclass
-class PutCrmLeadResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
+class LeadCreate:
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/numberfilter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,19 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import noteupdate as shared_noteupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmNoteRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('note') }})
-    
-
-@dataclasses.dataclass
-class PutCrmNoteRequest:
-    request: Optional[PutCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PutCrmNoteResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    
-
-@dataclasses.dataclass
-class PutCrmNoteResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
+class NumberFilter:
+    equals: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    gt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
+    gte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    lt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
+    lte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
+    not_: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/put_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_link_token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import taskupdate as shared_taskupdate
+import requests as requests_http
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmTaskRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('task'), 'exclude': lambda f: f is None }})
+class PostLinkTokenSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
 @dataclasses.dataclass
-class PutCrmTaskRequest:
-    request: Optional[PutCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class PostLinkTokenRequest:
+    security: PostLinkTokenSecurity = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmTaskResponseBody:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
+class PostLinkTokenResponseBody:
+    link_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkToken'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PutCrmTaskResponse:
+class PostLinkTokenResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostLinkTokenResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import account as shared_account
 from ..shared import datefilter as shared_datefilter
 from ..shared import numberfilter as shared_numberfilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
@@ -16,50 +17,51 @@
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBodyFilters:
-    annual_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    city: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('country'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    industry: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('industry'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('postalCode'), 'exclude': lambda f: f is None }})
-    state: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('state'), 'exclude': lambda f: f is None }})
-    street: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('street'), 'exclude': lambda f: f is None }})
-    website: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('website'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    city: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    country: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    industry: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    postal_code: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
+    state: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    street: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
+    website: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBody:
-    filters: Optional[SearchCrmAccountsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+    filters: Optional[SearchCrmAccountsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmAccountsRequest:
     query_params: SearchCrmAccountsQueryParams = dataclasses.field()
     request: Optional[SearchCrmAccountsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsResponseBody:
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accounts'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmAccountsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmAccountsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import contact as shared_contact
 from ..shared import datefilter as shared_datefilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
@@ -15,44 +16,45 @@
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsRequestBodyFilters:
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsRequestBody:
-    filters: Optional[SearchCrmContactsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+    filters: Optional[SearchCrmContactsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmContactsRequest:
     query_params: SearchCrmContactsQueryParams = dataclasses.field()
     request: Optional[SearchCrmContactsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsResponseBody:
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contacts'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmContactsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmContactsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import deal as shared_deal
-from ..shared import numberfilter as shared_numberfilter
+from ..shared import event as shared_event
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class SearchCrmDealsQueryParams:
+class SearchCrmEventsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsRequestBodyFilters:
-    amount: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('amount'), 'exclude': lambda f: f is None }})
-    close_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('closeDate'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    expected_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    is_closed: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isClosed'), 'exclude': lambda f: f is None }})
-    is_won: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isWon'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    probability: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('probability'), 'exclude': lambda f: f is None }})
-    stage: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('stage'), 'exclude': lambda f: f is None }})
+class SearchCrmEventsRequestBodyFilters:
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsRequestBody:
-    filters: Optional[SearchCrmDealsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmEventsRequestBody:
+    filters: Optional[SearchCrmEventsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmDealsRequest:
-    query_params: SearchCrmDealsQueryParams = dataclasses.field()
-    request: Optional[SearchCrmDealsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmEventsRequest:
+    query_params: SearchCrmEventsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsResponseBody:
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('deals'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class SearchCrmEventsResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmDealsResponse:
+class SearchCrmEventsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[SearchCrmDealsResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[SearchCrmEventsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
 from ..shared import email as shared_email
 from ..shared import stringfilter as shared_stringfilter
 from ..shared import stringlistfilter as shared_stringlistfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
@@ -17,50 +18,51 @@
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBodyFilters:
-    bcc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bcc'), 'exclude': lambda f: f is None }})
-    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    body_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bodyHtml'), 'exclude': lambda f: f is None }})
-    cc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('cc'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    from_: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('from'), 'exclude': lambda f: f is None }})
-    has_attachment: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('hasAttachment'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    is_bounced: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isBounced'), 'exclude': lambda f: f is None }})
-    is_incoming: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    message_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('messageDate'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
-    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
-    to: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('to'), 'exclude': lambda f: f is None }})
+    bcc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    from_: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from'), 'exclude': lambda f: f is None }})
+    has_attachment: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    is_bounced: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    message_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    to: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBody:
-    filters: Optional[SearchCrmEmailsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+    filters: Optional[SearchCrmEmailsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEmailsRequest:
     query_params: SearchCrmEmailsQueryParams = dataclasses.field()
     request: Optional[SearchCrmEmailsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsResponseBody:
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('emails'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEmailsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEmailsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import eventattendee as shared_eventattendee
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
@@ -15,41 +16,42 @@
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBodyFilters:
-    associated_object_type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('associatedObjectType'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+    associated_object_type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBody:
-    filters: Optional[SearchCrmEventAttendeesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+    filters: Optional[SearchCrmEventAttendeesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequest:
     query_params: SearchCrmEventAttendeesQueryParams = dataclasses.field()
     request: Optional[SearchCrmEventAttendeesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponseBody:
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendees'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import booleanfilter as shared_booleanfilter
+import requests as requests_http
 from ..shared import datefilter as shared_datefilter
-from ..shared import event as shared_event
+from ..shared import lead as shared_lead
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class SearchCrmEventsQueryParams:
+class SearchCrmLeadsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmEventsRequestBodyFilters:
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('endDateTime'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    location: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('location'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    start_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('startDateTime'), 'exclude': lambda f: f is None }})
-    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('type'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsRequestBodyFilters:
+    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmEventsRequestBody:
-    filters: Optional[SearchCrmEventsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsRequestBody:
+    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmEventsRequest:
-    query_params: SearchCrmEventsQueryParams = dataclasses.field()
-    request: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmLeadsRequest:
+    query_params: SearchCrmLeadsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmEventsResponseBody:
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('events'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsResponseBody:
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmEventsResponse:
+class SearchCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[SearchCrmEventsResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
+from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import lead as shared_lead
 from ..shared import stringfilter as shared_stringfilter
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class SearchCrmLeadsQueryParams:
+class SearchCrmTasksQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBodyFilters:
-    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('account'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksRequestBodyFilters:
+    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    due_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    is_done: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    priority: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBody:
-    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksRequestBody:
+    filters: Optional[SearchCrmTasksRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmLeadsRequest:
-    query_params: SearchCrmLeadsQueryParams = dataclasses.field()
-    request: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmTasksRequest:
+    query_params: SearchCrmTasksQueryParams = dataclasses.field()
+    request: Optional[SearchCrmTasksRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsResponseBody:
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('leads'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksResponseBody:
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmLeadsResponse:
+class SearchCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[SearchCrmTasksResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import note as shared_note
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
@@ -15,41 +16,42 @@
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmNotesRequestBodyFilters:
-    content: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('content'), 'exclude': lambda f: f is None }})
-    content_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contentHtml'), 'exclude': lambda f: f is None }})
-    content_text: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contentText'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
+    content: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    content_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentHtml'), 'exclude': lambda f: f is None }})
+    content_text: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentText'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmNotesRequestBody:
-    filters: Optional[SearchCrmNotesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+    filters: Optional[SearchCrmNotesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmNotesRequest:
     query_params: SearchCrmNotesQueryParams = dataclasses.field()
     request: Optional[SearchCrmNotesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmNotesResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('notes'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmNotesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmNotesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_tasks.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import booleanfilter as shared_booleanfilter
+import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import stringfilter as shared_stringfilter
-from ..shared import task as shared_task
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class SearchCrmTasksQueryParams:
+class SearchCrmUsersQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksRequestBodyFilters:
-    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    due_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('dueDate'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    is_done: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isDone'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    priority: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('priority'), 'exclude': lambda f: f is None }})
-    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
-    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
+class SearchCrmUsersRequestBodyFilters:
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksRequestBody:
-    filters: Optional[SearchCrmTasksRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmUsersRequestBody:
+    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmTasksRequest:
-    query_params: SearchCrmTasksQueryParams = dataclasses.field()
-    request: Optional[SearchCrmTasksRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmUsersRequest:
+    query_params: SearchCrmUsersQueryParams = dataclasses.field()
+    request: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('tasks'), 'exclude': lambda f: f is None }})
+class SearchCrmUsersResponseBody:
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmTasksResponse:
+class SearchCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[SearchCrmTasksResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/operations/search_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import datefilter as shared_datefilter
-from ..shared import stringfilter as shared_stringfilter
-from ..shared import user as shared_user
+import requests as requests_http
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class SearchCrmUsersQueryParams:
+class GetDetailsCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SearchCrmUsersRequestBodyFilters:
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SearchCrmUsersRequestBody:
-    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmUsersRequest:
-    query_params: SearchCrmUsersQueryParams = dataclasses.field()
-    request: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class GetDetailsCrmLeadRequest:
+    query_params: GetDetailsCrmLeadQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmUsersResponseBody:
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('users'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmLeadResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmUsersResponse:
+class GetDetailsCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/__init__.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 from .task import *
 from .taskcreate import *
 from .taskupdate import *
 from .user import *
 from .webhookmetadata import *
 from .webhookmetadatacreate import *
 
-__all__ = ["Account","AccountAssociations","AccountCreate","AccountUpdate","Address","BooleanFilter","Connection","ConnectionIntegrationIDEnum","ConnectionStatusEnum","Contact","ContactAssociations","ContactCreate","ContactUpdate","DateFilter","Deal","DealAssociations","DealCreate","DealUpdate","Email","EmailAssociations","EmailCreate","EmailCreateContact","EmailCreateLead","EmailUpdate","Event","EventAssociations","EventAttendee","EventAttendeeAssociations","EventAttendeeCreate","EventAttendeeUpdate","EventCreate","EventUpdate","Field","FieldOptions","FieldTypeEnum","Integration","IntegrationIntegrationIDEnum","Lead","LeadAssociations","LeadCreate","LeadUpdate","Note","NoteAssociations","NoteCreate","NoteUpdate","NumberFilter","SchemeVesselAPIToken","Security","StringFilter","StringListFilter","Task","TaskAssociations","TaskCreate","TaskUpdate","User","UserAssociations","WebhookMetadata","WebhookMetadataCreate"]
+__all__ = ["Account","AccountAssociations","AccountCreate","AccountUpdate","Address","BooleanFilter","Connection","ConnectionIntegrationIDEnum","ConnectionStatusEnum","Contact","ContactAssociations","ContactCreate","ContactUpdate","DateFilter","Deal","DealAssociations","DealCreate","DealUpdate","Email","EmailAssociations","EmailCreate","EmailCreateContact","EmailCreateLead","EmailUpdate","Event","EventAssociations","EventAttendee","EventAttendeeAssociations","EventAttendeeCreate","EventAttendeeUpdate","EventCreate","EventUpdate","Field","FieldOptions","FieldTypeEnum","Integration","IntegrationIntegrationIDEnum","Lead","LeadAssociations","LeadCreate","LeadUpdate","Note","NoteAssociations","NoteCreate","NoteUpdate","NumberFilter","SchemeVesselAPIToken","Security","StringFilter","StringListFilter","Task","TaskAssociations","TaskCreate","TaskUpdate","User","UserAssociations","WebhookMetadata","WebhookMetadataCreate"]
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/account.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/lead.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountAssociations:
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('noteIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('taskIds') }})
+class LeadAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Account:
-    r"""Account
-    (Alias: company, organization) An organization involved with your business.
+class Lead:
+    r"""Lead
+    A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal). 
+    *CRM Caveats*:
+    - HubSpot: we consider contacts with the `leadStatus` set to be leads.
     """
     
-    associations: AccountAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('industry'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('website'), 'exclude': lambda f: f is None }})
+    associations: LeadAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/accountcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountCreate:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('name') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('industry'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('website'), 'exclude': lambda f: f is None }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/accountupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AccountUpdate:
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('industry'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('website'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/address.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/address.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Address:
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('country'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('postalCode'), 'exclude': lambda f: f is None }})
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('state'), 'exclude': lambda f: f is None }})
-    street: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('street'), 'exclude': lambda f: f is None }})
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
+    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    street: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/booleanfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/booleanfilter.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class BooleanFilter:
-    equals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('equals'), 'exclude': lambda f: f is None }})
-    not_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('not'), 'exclude': lambda f: f is None }})
+    equals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    not_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/connection.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     INITIAL_SYNC = "INITIAL_SYNC"
     READY = "READY"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Connection:
-    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('connectionId'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime'), 'exclude': lambda f: f is None }})
-    integration_id: Optional[ConnectionIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('integrationId'), 'exclude': lambda f: f is None }})
-    last_activity_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastActivityDate'), 'exclude': lambda f: f is None }})
-    native_org_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeOrgURL'), 'exclude': lambda f: f is None }})
-    status: Optional[ConnectionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[ConnectionIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    last_activity_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastActivityDate'), 'exclude': lambda f: f is None }})
+    native_org_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL'), 'exclude': lambda f: f is None }})
+    status: Optional[ConnectionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/contact.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,32 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ContactAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendeeIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('noteIds') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('taskIds') }})
+class UserAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Contact:
-    r"""Contact
-    Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)
+class User:
+    r"""User
+    Users of the connected CRM platform. These are *not* the contacts or leads, but rather the user accounts from the connected CRM.
     """
     
-    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+    associations: UserAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/contactcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ContactCreate:
-    r"""ContactCreate
-    Properties that a contact can be created with
-    """
-    
-    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+class DealUpdate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    close_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/contactupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ContactUpdate:
     r"""ContactUpdate
     Update a Contact.
     """
     
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/datefilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DateFilter:
-    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('equals'), 'exclude': lambda f: f is None }})
-    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('gt'), 'exclude': lambda f: f is None }})
-    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('gte'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('in'), 'exclude': lambda f: f is None }})
-    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lt'), 'exclude': lambda f: f is None }})
-    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lte'), 'exclude': lambda f: f is None }})
-    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('notIn'), 'exclude': lambda f: f is None }})
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
+    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
+    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/deal.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DealAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('noteIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('taskIds') }})
-    event_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventIds'), 'exclude': lambda f: f is None }})
+class EventAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Deal:
-    r"""Deal
-    (Alias: Opportunity) An object representing either the opportunity to sell a product to an Account, or in the case of an `isWon` deal, a product sold to an Account.
-    *CRM Caveats*:
-    - Pipedrive: Users must have \"Deal probability\" turned on for the given pipeline for probability to be configurable and returned.
+class Event:
+    r"""Event
+    Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
+    For the currently supported CRMs, these are the objects Events most closely maps to:
+    - Salesforce = Events
+    - HubSpot = Meetings
+    - Pipedrive = Activities
     """
     
-    associations: DealAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('closeDate') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('name') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    stage: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('stage') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('amount'), 'exclude': lambda f: f is None }})
-    expected_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
-    is_closed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isClosed'), 'exclude': lambda f: f is None }})
-    is_won: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isWon'), 'exclude': lambda f: f is None }})
-    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('probability'), 'exclude': lambda f: f is None }})
+    associations: EventAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/dealcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DealCreate:
-    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('closeDate') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('name') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountId'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('amount'), 'exclude': lambda f: f is None }})
-    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('probability'), 'exclude': lambda f: f is None }})
-    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('stage'), 'exclude': lambda f: f is None }})
+    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/dealupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DealUpdate:
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountId'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('amount'), 'exclude': lambda f: f is None }})
-    close_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('closeDate'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('probability'), 'exclude': lambda f: f is None }})
-    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('stage'), 'exclude': lambda f: f is None }})
+class StringFilter:
+    contains: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contains'), 'exclude': lambda f: f is None }})
+    ends_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endsWith'), 'exclude': lambda f: f is None }})
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+    starts_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startsWith'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/email.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/email.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EmailAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Email:
     r"""Email
     An email is a message sent from one person to another through an email service. Emails involve participants - the person who the email was sent to, or the person that sent it. Participants are usually a Contact, Lead, or User but in certain CRMs, can be a person not yet associated with a CRM object.
     """
     
-    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('from') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject') }})
-    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('to') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bcc'), 'exclude': lambda f: f is None }})
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bodyHtml'), 'exclude': lambda f: f is None }})
-    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('cc'), 'exclude': lambda f: f is None }})
-    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('hasAttachment'), 'exclude': lambda f: f is None }})
-    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isBounced'), 'exclude': lambda f: f is None }})
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('messageDate'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
+    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
+    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/emailcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/emailcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EmailCreateContact:
     r"""EmailCreateContact
     Associated Contacts must participate in the email (i.e., have a role).
     """
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('role'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EmailCreateLead:
     r"""EmailCreateLead
     Associated Leads must participate in the email (i.e., have a role).
     """
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('id'), 'exclude': lambda f: f is None }})
-    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('role'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EmailCreate:
-    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('from') }})
-    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject') }})
-    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('to') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountId'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bcc'), 'exclude': lambda f: f is None }})
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('bodyHtml'), 'exclude': lambda f: f is None }})
-    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('cc'), 'exclude': lambda f: f is None }})
-    contact: Optional[EmailCreateContact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contact'), 'exclude': lambda f: f is None }})
-    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealId'), 'exclude': lambda f: f is None }})
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    lead: Optional[EmailCreateLead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lead'), 'exclude': lambda f: f is None }})
-    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('messageDate'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
+    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    contact: Optional[EmailCreateContact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    lead: Optional[EmailCreateLead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
+    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/emailupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from enum import Enum
+from typing import Optional
 from vesselapi import utils
 
+class IntegrationIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EmailUpdate:
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+class Integration:
+    icon_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iconURL'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[IntegrationIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/event.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendeeIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
+class FieldOptions:
+    key: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
+class FieldTypeEnum(str, Enum):
+    STRING = "string"
+    NUMBER = "number"
+    DATETIME = "datetime"
+    DATE = "date"
+    BOOLEAN = "boolean"
+    REFERENCE = "reference"
+    PHONE = "phone"
+    URL = "url"
+    ID = "id"
+    EMAIL = "email"
+    PERCENT = "percent"
+    SINGLESELECT = "singleselect"
+    MULTISELECT = "multiselect"
+    ADDRESS = "address"
+    DECIMAL = "decimal"
+    TIME = "time"
+    DATERANGE = "daterange"
+    OBJECT = "object"
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Event:
-    r"""Event
-    Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
-    For the currently supported CRMs, these are the objects Events most closely maps to:
-    - Salesforce = Events
-    - HubSpot = Meetings
-    - Pipedrive = Activities
+class Field:
+    r"""Field
+    (Alias: property) A field is a key-value pair on a CRM Object that provides information about that object.
     """
     
-    associations: EventAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('endDateTime'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('location'), 'exclude': lambda f: f is None }})
-    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('startDateTime'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('type'), 'exclude': lambda f: f is None }})
+    creatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creatable') }})
+    custom: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom') }})
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
+    type: FieldTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    universal: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('universal') }})
+    updatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatable') }})
+    is_array: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isArray'), 'exclude': lambda f: f is None }})
+    options: Optional[list[FieldOptions]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/eventattendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,20 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventAttendeeAssociations:
-    association_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associationId') }})
-    event_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventId') }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class EventAttendee:
-    r"""EventAttendee
-    Event Attendees hold information about someone who attendeed or was invited to an event. Attendees are always associated with some Event and another person object such as a Contact, Lead, or Other.
+class NoteCreate:
+    r"""NoteCreate
+    Create a new Note. You may only associate a note with at most one entity of each type upon creation.
     """
     
-    associated_object_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associatedObjectType') }})
-    associations: EventAttendeeAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/eventattendeecreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventAttendeeCreate:
-    associated_object_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associatedObjectType') }})
-    event_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    association_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('associationId'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
+class LeadUpdate:
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/eventcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EventCreate:
-    end_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('endDateTime') }})
-    start_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('startDateTime') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountId'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactId'), 'exclude': lambda f: f is None }})
-    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealId'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadId'), 'exclude': lambda f: f is None }})
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('location'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('type'), 'exclude': lambda f: f is None }})
+    end_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime') }})
+    start_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/eventupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventUpdate:
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('endDateTime'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('location'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('startDateTime'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('type'), 'exclude': lambda f: f is None }})
+class TaskCreate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/field.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,20 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class FieldOptions:
-    key: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('key'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
-    
-class FieldTypeEnum(str, Enum):
-    STRING = "string"
-    NUMBER = "number"
-    DATETIME = "datetime"
-    DATE = "date"
-    BOOLEAN = "boolean"
-    REFERENCE = "reference"
-    PHONE = "phone"
-    URL = "url"
-    ID = "id"
-    EMAIL = "email"
-    PERCENT = "percent"
-    SINGLESELECT = "singleselect"
-    MULTISELECT = "multiselect"
-    ADDRESS = "address"
-    DECIMAL = "decimal"
-    TIME = "time"
-    DATERANGE = "daterange"
-    OBJECT = "object"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class Field:
-    r"""Field
-    (Alias: property) A field is a key-value pair on a CRM Object that provides information about that object.
-    """
-    
-    creatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('creatable') }})
-    custom: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('custom') }})
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('key') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('name') }})
-    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('required') }})
-    type: FieldTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('type') }})
-    universal: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('universal') }})
-    updatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('updatable') }})
-    is_array: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isArray'), 'exclude': lambda f: f is None }})
-    options: Optional[list[FieldOptions]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('options'), 'exclude': lambda f: f is None }})
+class EventUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/integration.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
-class IntegrationIntegrationIDEnum(str, Enum):
-    SALESFORCE = "salesforce"
-    HUBSPOT = "hubspot"
-    PIPEDRIVE = "pipedrive"
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Integration:
-    icon_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('iconURL'), 'exclude': lambda f: f is None }})
-    integration_id: Optional[IntegrationIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('integrationId'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('name'), 'exclude': lambda f: f is None }})
+class StringListFilter:
+    has: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has'), 'exclude': lambda f: f is None }})
+    has_every: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasEvery'), 'exclude': lambda f: f is None }})
+    has_some: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasSome'), 'exclude': lambda f: f is None }})
+    is_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isEmpty'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/account.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class LeadAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventAttendeeIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('eventIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('noteIds') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('taskIds') }})
+class AccountAssociations:
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Lead:
-    r"""Lead
-    A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal). 
-    *CRM Caveats*:
-    - HubSpot: we consider contacts with the `leadStatus` set to be leads.
+class Account:
+    r"""Account
+    (Alias: company, organization) An organization involved with your business.
     """
     
-    associations: LeadAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('account'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+    associations: AccountAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/leadcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class LeadCreate:
-    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName') }})
-    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('account'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+class ContactCreate:
+    r"""ContactCreate
+    Properties that a contact can be created with
+    """
+    
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/leadupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class LeadUpdate:
-    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('account'), 'exclude': lambda f: f is None }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('phone'), 'exclude': lambda f: f is None }})
+class TaskUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/note.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,30 +3,35 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NoteAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
+class TaskAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Note:
-    r"""Note
-    A Note attached to some CRM Object. 
+class Task:
+    r"""Task
+    A task attached to some CRM object
     """
     
-    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('content'), 'exclude': lambda f: f is None }})
+    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/noteupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class NoteUpdate:
     r"""NoteUpdate
     Update an existing Note. Please note that updating associations is not currently supported.
     """
     
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('content'), 'exclude': lambda f: f is None }})
-    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('userId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/task.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contact.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,37 @@
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TaskAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('ownerUserId') }})
+class ContactAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Task:
-    r"""Task
-    A task attached to some CRM object
+class Contact:
+    r"""Contact
+    Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)
     """
     
-    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('createdTime') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('id') }})
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('modifiedTime') }})
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.field_name('nativeId') }})
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('additional'), 'exclude': lambda f: f is None }})
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('body'), 'exclude': lambda f: f is None }})
-    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('dueDate'), 'exclude': lambda f: f is None }})
-    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('isDone'), 'exclude': lambda f: f is None }})
-    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('priority'), 'exclude': lambda f: f is None }})
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('status'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('subject'), 'exclude': lambda f: f is None }})
+    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/models/shared/webhookmetadatacreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WebhookMetadataCreate:
     r"""WebhookMetadataCreate
     Information describing a webhook
     """
     
-    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.field_name('webhookUrl'), 'exclude': lambda f: f is None }})
+    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.2.2/src/vesselapi/notes.py` & `vesselapi-3.5.2/src/vesselapi/notes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,217 +1,210 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Notes:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def batch(self, request: operations.GetBatchCrmNoteRequest) -> operations.GetBatchCrmNoteResponse:
         r"""Get Batch Notes
         Retrieve Notes by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/note/batch"
+        url = base_url.removesuffix('/') + '/crm/note/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmNoteResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmNoteResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def create(self, request: operations.PostCrmNoteRequest) -> operations.PostCrmNoteResponse:
         r"""Create Note
         Create a new Note.
         *CRM Caveats*:
         - Salesforce: You may only associate a Note with one entity.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/note"
+        url = base_url.removesuffix('/') + '/crm/note'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmNoteResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmNoteResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmNoteRequest) -> operations.GetDetailsCrmNoteResponse:
         r"""Get Note Details
         Get details about all notes. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/note/details"
+        url = base_url.removesuffix('/') + '/crm/note/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmNoteResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmNoteResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmNoteRequest) -> operations.GetOneCrmNoteResponse:
         r"""Get Note
         Retrieve a single Note by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/note"
+        url = base_url.removesuffix('/') + '/crm/note'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmNoteResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmNoteResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmNotesRequest) -> operations.GetAllCrmNotesResponse:
         r"""Get All Notes
         Retrieve all Notes
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/notes"
+        url = base_url.removesuffix('/') + '/crm/notes'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmNotesResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmNotesResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmNotesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmNotesRequest) -> operations.SearchCrmNotesResponse:
         r"""Search Notes
         Search all Notes using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/notes/search"
+        url = base_url.removesuffix('/') + '/crm/notes/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmNotesResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmNotesResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmNotesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def update(self, request: operations.PutCrmNoteRequest) -> operations.PutCrmNoteResponse:
         r"""Update Note
         Update an existing Note by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/note"
+        url = base_url.removesuffix('/') + '/crm/note'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("PATCH", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmNoteResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PutCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PutCrmNoteResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmNoteResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/passthrough.py` & `vesselapi-3.5.2/src/vesselapi/passthrough.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Passthrough:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def create(self, request: operations.PostCrmPassthroughRequest) -> operations.PostCrmPassthroughResponse:
         r"""Passthrough Request
         Send an authenticated passthrough request to the downstream CRM. This is useful for making requests to endpoints that are not yet supported by Vessel.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/passthrough"
+        url = base_url.removesuffix('/') + '/crm/passthrough'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        r = client.request("POST", url, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmPassthroughResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostCrmPassthroughResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostCrmPassthroughResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmPassthroughResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/tokens.py` & `vesselapi-3.5.2/src/vesselapi/tokens.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Tokens:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def create(self, request: operations.PostLinkTokenRequest) -> operations.PostLinkTokenResponse:
         r"""Create Link Token
         Generates a link token to be used during the authentication flow. This token is passed to either the Vessel Link Component or `useVesselLink` hook.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/link/token"
+        url = base_url.removesuffix('/') + '/link/token'
         
         
         client = utils.configure_security_client(self._client, request.security)
         
-        r = client.request("POST", url)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostLinkTokenResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.PostLinkTokenResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.PostLinkTokenResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostLinkTokenResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/users.py` & `vesselapi-3.5.2/src/vesselapi/users.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,152 @@
-import requests
+import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Users:
-    _client: requests.Session
-    _security_client: requests.Session
+    _client: requests_http.Session
+    _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
-    def __init__(self, client: requests.Session, security_client: requests.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
-
-    
+        
     def batch(self, request: operations.GetBatchCrmUserRequest) -> operations.GetBatchCrmUserResponse:
         r"""Get Batch Users
         Retrieve Users by a set of Id's
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/user/batch"
+        url = base_url.removesuffix('/') + '/crm/user/batch'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmUserResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetBatchCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetBatchCrmUserResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmUserRequest) -> operations.GetDetailsCrmUserResponse:
         r"""Get User Details
         Get details about all users. 
         Details include the type, possible values, and other meta data about the fields.
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/user/details"
+        url = base_url.removesuffix('/') + '/crm/user/details'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmUserResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetDetailsCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetDetailsCrmUserResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmUserRequest) -> operations.GetOneCrmUserResponse:
         r"""Get User
         Retrieve a single User by Id
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/user"
+        url = base_url.removesuffix('/') + '/crm/user'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmUserResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetOneCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetOneCrmUserResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmUsersRequest) -> operations.GetAllCrmUsersResponse:
         r"""Get All Users
         Retrieve all Users
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/users"
+        url = base_url.removesuffix('/') + '/crm/users'
         
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("GET", url, params=query_params)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmUsersResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.GetAllCrmUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.GetAllCrmUsersResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmUsersResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmUsersRequest) -> operations.SearchCrmUsersResponse:
         r"""Search Users
         Search all Users using filters
         """
         
         base_url = self._server_url
         
-        url = base_url.removesuffix("/") + "/crm/users/search"
+        url = base_url.removesuffix('/') + '/crm/users/search'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request)
-        if req_content_type != "multipart/form-data" and req_content_type != "multipart/mixed":
-            headers["content-type"] = req_content_type
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        r = client.request("POST", url, params=query_params, data=data, files=form, headers=headers)
-        content_type = r.headers.get("Content-Type")
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmUsersResponse(status_code=r.status_code, content_type=content_type)
+        res = operations.SearchCrmUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if r.status_code == 200:
-            if utils.match_content_type(content_type, "application/json"):
-                out = utils.unmarshal_json(r.text, Optional[operations.SearchCrmUsersResponseBody])
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmUsersResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.2.2/src/vesselapi/utils/utils.py` & `vesselapi-3.5.2/src/vesselapi/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,68 +37,85 @@
             continue
 
         metadata = sec_field.metadata.get('security')
         if metadata is None:
             continue
         if metadata.get('option'):
             _parse_security_option(client, value)
-            return
-        elif metadata.get('scheme'):
-            _parse_security_scheme(client, metadata, value)
+            return client
+        if metadata.get('scheme'):
+            # Special case for basic auth which could be a flattened struct
+            if metadata.get("sub_type") == "basic" and not is_dataclass(value):
+                _parse_security_scheme(client, metadata, security)
+            else:
+                _parse_security_scheme(client, metadata, value)
 
     return client
 
 
 def _parse_security_option(client: SecurityClient, option: dataclass):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
         metadata = opt_field.metadata.get('security')
         if metadata is None or metadata.get('scheme') is None:
             continue
-        _parse_security_scheme(client, metadata.get(
-            'scheme'), getattr(option, opt_field.name))
+        _parse_security_scheme(
+            client, metadata, getattr(option, opt_field.name))
 
 
-def _parse_security_scheme(client: SecurityClient, scheme_metadata: dict, scheme: dataclass):
+def _parse_security_scheme(client: SecurityClient, scheme_metadata: dict, scheme: any):
     scheme_type = scheme_metadata.get('type')
     sub_type = scheme_metadata.get('sub_type')
 
-    if scheme_type == 'http' and sub_type == 'basic':
-        _parse_basic_auth_scheme(client, scheme)
-        return
+    if is_dataclass(scheme):
+        if scheme_type == 'http' and sub_type == 'basic':
+            _parse_basic_auth_scheme(client, scheme)
+            return
 
-    scheme_fields: Tuple[Field, ...] = fields(scheme)
-    for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
-            continue
+        scheme_fields: Tuple[Field, ...] = fields(scheme)
+        for scheme_field in scheme_fields:
+            metadata = scheme_field.metadata.get('security')
+            if metadata is None or metadata.get('field_name') is None:
+                continue
 
-        header_name = metadata.get('field_name')
-        value = getattr(scheme, scheme_field.name)
+            value = getattr(scheme, scheme_field.name)
 
-        if scheme_type == "apiKey":
-            if sub_type == 'header':
-                client.client.headers[header_name] = value
-            elif sub_type == 'query':
-                client.query_params[header_name] = value
-            elif sub_type == 'cookie':
-                client.client.cookies[header_name] = value
-            else:
-                raise Exception('not supported')
-        elif scheme_type == "openIdConnect":
+            _parse_security_scheme_value(
+                client, scheme_metadata, metadata, value)
+    else:
+        _parse_security_scheme_value(
+            client, scheme_metadata, scheme_metadata, scheme)
+
+
+def _parse_security_scheme_value(client: SecurityClient, scheme_metadata: dict, security_metadata: dict, value: any):
+    scheme_type = scheme_metadata.get('type')
+    sub_type = scheme_metadata.get('sub_type')
+
+    header_name = security_metadata.get('field_name')
+
+    if scheme_type == "apiKey":
+        if sub_type == 'header':
             client.client.headers[header_name] = value
-        elif scheme_type == 'oauth2':
+        elif sub_type == 'query':
+            client.query_params[header_name] = value
+        elif sub_type == 'cookie':
+            client.client.cookies[header_name] = value
+        else:
+            raise Exception('not supported')
+    elif scheme_type == "openIdConnect":
+        client.client.headers[header_name] = value
+    elif scheme_type == 'oauth2':
+        client.client.headers[header_name] = value
+    elif scheme_type == 'http':
+        if sub_type == 'bearer':
             client.client.headers[header_name] = value
-        elif scheme_type == 'http':
-            if sub_type == 'bearer':
-                client.client.headers[header_name] = value
-            else:
-                raise Exception('not supported')
         else:
             raise Exception('not supported')
+    else:
+        raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
@@ -117,97 +134,99 @@
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
 def generate_url(server_url: str, path: str, path_params: dataclass) -> str:
     path_param_fields: Tuple[Field, ...] = fields(path_params)
-    for f in path_param_fields:
-        param_metadata = f.metadata.get('path_param')
+    for field in path_param_fields:
+        param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
         if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(path_params, f.name)
+            param = getattr(path_params, field.name)
             if param is None:
                 continue
 
-            if type(param) is list:
+            if isinstance(param, list):
                 pp_vals: list[str] = []
                 for pp_val in param:
                     if pp_val is None:
                         continue
-                    pp_vals.append(val_to_string(pp_val))
+                    pp_vals.append(_val_to_string(pp_val))
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', f.name) + '}', ",".join(pp_vals), 1)
-            elif type(param) is dict:
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif isinstance(param, dict):
                 pp_vals: list[str] = []
                 for pp_key in param:
                     if param[pp_key] is None:
                         continue
                     if param_metadata.get('explode'):
                         pp_vals.append(
-                            f"{pp_key}={val_to_string(param[pp_key])}")
+                            f"{pp_key}={_val_to_string(param[pp_key])}")
                     else:
                         pp_vals.append(
-                            f"{pp_key},{val_to_string(param[pp_key])}")
+                            f"{pp_key},{_val_to_string(param[pp_key])}")
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', f.name) + '}', ",".join(pp_vals), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
             elif not isinstance(param, (str, int, float, complex, bool)):
                 pp_vals: list[str] = []
                 param_fields: Tuple[Field, ...] = fields(param)
-                for field in param_fields:
-                    param_value_metadata = field.metadata.get('path_param')
+                for param_field in param_fields:
+                    param_value_metadata = param_field.metadata.get(
+                        'path_param')
                     if not param_value_metadata:
                         continue
 
-                    parm_name = param_value_metadata.get('field_name', f.name)
+                    parm_name = param_value_metadata.get(
+                        'field_name', field.name)
 
-                    param_field_val = getattr(param, field.name)
+                    param_field_val = getattr(param, param_field.name)
                     if param_field_val is None:
                         continue
-                    elif param_metadata.get('explode'):
+                    if param_metadata.get('explode'):
                         pp_vals.append(
-                            f"{parm_name}={val_to_string(param_field_val)}")
+                            f"{parm_name}={_val_to_string(param_field_val)}")
                     else:
                         pp_vals.append(
-                            f"{parm_name},{val_to_string(param_field_val)}")
+                            f"{parm_name},{_val_to_string(param_field_val)}")
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', f.name) + '}', ",".join(pp_vals), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
             else:
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', f.name) + '}', val_to_string(param), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
-def replace_parameters(string_with_params: str, params: dict[str, str]) -> str:
+def template_url(url_with_params: str, params: dict[str, str]) -> str:
     for key, value in params.items():
-        string_with_params = string_with_params.replace(
+        url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
-    return string_with_params
+    return url_with_params
 
 
 def get_query_params(query_params: dataclass) -> dict[str, list[str]]:
     if query_params is None:
         return {}
 
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(query_params)
-    for f in param_fields:
-        metadata = f.metadata.get('query_param')
+    for field in param_fields:
+        metadata = field.metadata.get('query_param')
         if not metadata:
             continue
 
-        param_name = f.name
+        param_name = field.name
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
             params = params | _get_serialized_query_params(
                 metadata, f_name, getattr(query_params, param_name))
         else:
             style = metadata.get('style', 'form')
@@ -225,24 +244,24 @@
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
         return {}
 
     headers: dict[str, str] = {}
 
     param_fields: Tuple[Field, ...] = fields(headers_params)
-    for f in param_fields:
-        metadata = f.metadata.get('header')
+    for field in param_fields:
+        metadata = field.metadata.get('header')
         if not metadata:
             continue
 
         value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, f.name))
+            'explode', False), getattr(headers_params, field.name))
 
         if value != '':
-            headers[metadata.get('field_name', f.name)] = value
+            headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
 def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
@@ -262,33 +281,33 @@
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_param_metadata = obj_field.metadata.get('query_param')
             if not obj_param_metadata:
                 continue
 
-            val = getattr(obj, obj_field.name)
-            if val is None:
+            obj_val = getattr(obj, obj_field.name)
+            if obj_val is None:
                 continue
 
-            if isinstance(val, list):
-                for v in val:
-                    if v is None:
+            if isinstance(obj_val, list):
+                for val in obj_val:
+                    if val is None:
                         continue
 
                     if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
                         params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(val_to_string(v))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    val_to_string(val)]
+                    _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, list):
                 for val in value:
@@ -296,18 +315,18 @@
                         continue
 
                     if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
                         params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    val_to_string(value)]
+                    _val_to_string(value)]
     return params
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
     obj_param_metadata = obj_field.metadata.get('query_param')
 
     if not obj_param_metadata:
@@ -327,43 +346,43 @@
     request_val = getattr(request, "request")
     if request_val is None:
         raise Exception("request body not found")
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
-    for f in request_fields:
-        if f.name == "request":
-            request_metadata = f.metadata.get('request')
+    for field in request_fields:
+        if field.name == "request":
+            request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is not None:
         # single request
         return serialize_content_type('request', request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
     request_fields: Tuple[Field, ...] = fields(request_val)
-    for f in request_fields:
-        req = getattr(request_val, f.name)
+    for field in request_fields:
+        req = getattr(request_val, field.name)
         if req is None:
             continue
 
-        request_metadata = f.metadata.get('request')
+        request_metadata = field.metadata.get('request')
         if request_metadata is None:
             raise Exception(
-                f'missing request tag on request body field {f.name}')
+                f'missing request tag on request body field {field.name}')
 
-        return serialize_content_type(f.name, request_metadata.get('media_type', 'application/octet-stream'), req)
+        return serialize_content_type(field.name, request_metadata.get('media_type', 'application/octet-stream'), req)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) != None:
+    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
-    if re.match(r'multipart\/.*', media_type) != None:
+    if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) != None:
+    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
@@ -413,35 +432,35 @@
             field_name = field_metadata.get(
                 "field_name", field.name)
             if isinstance(val, list):
                 for value in val:
                     if value is None:
                         continue
                     form.append(
-                        [field_name + "[]", [None, val_to_string(value)]])
+                        [field_name + "[]", [None, _val_to_string(value)]])
             else:
-                form.append([field_name, [None, val_to_string(val)]])
+                form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
         str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
-        for k, v in original.items():
-            if k not in existing:
-                existing[k] = []
-            existing[k].append(v)
+        for key, val in original.items():
+            if key not in existing:
+                existing[key] = []
+            existing[key].append(val)
     else:
         temp = []
-        for k, v in original.items():
-            temp.append(str(k))
-            temp.append(str(v))
+        for key, val in original.items():
+            temp.append(str(key))
+            temp.append(str(val))
         if field_name not in existing:
             existing[field_name] = []
         existing[field_name].append(",".join(temp))
     return existing
 
 
 def serialize_form_data(field_name: str, data: dataclass) -> dict[str, any]:
@@ -466,15 +485,15 @@
                     form = form | _populate_form(
                         field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
-            form[key] = [val_to_string(value)]
+            form[key] = [_val_to_string(value)]
     else:
         raise Exception(f'Invalid request body type for field {field_name}')
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
@@ -483,15 +502,15 @@
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
 def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
-    params: dict[str, str | list[str]] = {}
+    params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
 
@@ -502,57 +521,57 @@
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [val_to_string(val)]
+                params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name},{val_to_string(val)}')
+                    f'{obj_field_name},{_val_to_string(val)}')
 
         if len(items) > 0:
             params[field_name] = [','.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = val_to_string(value)
+                params[key] = _val_to_string(value)
             else:
-                items.append(f'{key},{val_to_string(value)}')
+                items.append(f'{key},{_val_to_string(value)}')
 
         if len(items) > 0:
             params[field_name] = [','.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
                 if not field_name in params:
                     params[field_name] = []
-                params[field_name].append(val_to_string(value))
+                params[field_name].append(_val_to_string(value))
             else:
-                items.append(val_to_string(value))
+                items.append(_val_to_string(value))
 
         if len(items) > 0:
             params[field_name] = [','.join([str(item) for item in items])]
     else:
-        params[field_name] = val_to_string(obj)
+        params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
-def _serialize_header(explode: boolean, obj: any) -> str:
+def _serialize_header(explode: bool, obj: any) -> str:
     if obj is None:
         return ''
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
@@ -568,116 +587,119 @@
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
                 items.append(
-                    f'{obj_field_name}={val_to_string(val)}')
+                    f'{obj_field_name}={_val_to_string(val)}')
             else:
                 items.append(obj_field_name)
-                items.append(val_to_string(val))
+                items.append(_val_to_string(val))
 
         if len(items) > 0:
             return ','.join(items)
     elif isinstance(obj, dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={val_to_string(value)}')
+                items.append(f'{key}={_val_to_string(value)}')
             else:
                 items.append(key)
-                items.append(val_to_string(value))
+                items.append(_val_to_string(value))
 
         if len(items) > 0:
             return ','.join([str(item) for item in items])
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
-            items.append(val_to_string(value))
+            items.append(_val_to_string(value))
 
-        return ','.join(items)
+        if len(items) > 0:
+            return ','.join(items)
     else:
-        return f'{val_to_string(obj)}'
+        return f'{_val_to_string(obj)}'
+
+    return ''
 
 
-def unmarshal_json(data, t):
-    Unmarhsal = make_dataclass('Unmarhsal', [('res', t)],
+def unmarshal_json(data, typ):
+    unmarhsal = make_dataclass('Unmarhsal', [('res', typ)],
                                bases=(DataClassJsonMixin,))
-    d = json.loads(data)
-    out = Unmarhsal.from_dict({"res": d})
+    json_dict = json.loads(data)
+    out = unmarhsal.from_dict({"res": json_dict})
     return out.res
 
 
-def marshal_json(c):
-    Marshal = make_dataclass('Marshal', [('res', type(c))],
+def marshal_json(val):
+    marshal = make_dataclass('Marshal', [('res', type(val))],
                              bases=(DataClassJsonMixin,))
-    m = Marshal(res=c)
-    d = m.to_dict()
-    return json.dumps(d["res"])
+    marshaller = marshal(res=val)
+    json_dict = marshaller.to_dict()
+    return json.dumps(json_dict["res"])
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
-    if content_type == pattern or pattern == "*" or pattern == "*/*":
+    if pattern in (content_type, "*", "*/*"):
         return True
 
-    m = Message()
-    m['content-type'] = content_type
-    media_type = m.get_content_type()
+    msg = Message()
+    msg['content-type'] = content_type
+    media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if f'{parts[0]}/*' == pattern or f'*/{parts[1]}' == pattern:
+        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
             return True
 
     return False
 
 
 def datetimeisoformat(optional: bool):
-    def isoformatoptional(v):
-        if optional and v is None:
+    def isoformatoptional(val):
+        if optional and val is None:
             return None
-        return val_to_string(v)
+        return _val_to_string(val)
 
     return isoformatoptional
 
 
 def dateisoformat(optional: bool):
-    def isoformatoptional(v):
-        if optional and v is None:
+    def isoformatoptional(val):
+        if optional and val is None:
             return None
-        return date.isoformat(v)
+        return date.isoformat(val)
 
     return isoformatoptional
 
 
-def datefromisoformat(date: str):
-    return dateutil.parser.parse(date).date()
+def datefromisoformat(date_str: str):
+    return dateutil.parser.parse(date_str).date()
 
 
-def field_name(name):
+def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
-def val_to_string(val):
+def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
-    elif isinstance(val, datetime):
+    if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
-    elif isinstance(val, Enum):
+    if isinstance(val, Enum):
         return val.value
 
     return str(val)
```

### Comparing `vesselapi-3.2.2/src/vesselapi.egg-info/PKG-INFO` & `vesselapi-3.5.2/src/vesselapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vesselapi
-Version: 3.2.2
+Version: 3.5.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: vesselapi
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `vesselapi-3.2.2/src/vesselapi.egg-info/SOURCES.txt` & `vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

