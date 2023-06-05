# Comparing `tmp/tpdk-2.0.0b2.tar.gz` & `tmp/tpdk-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpdk-2.0.0b2.tar", last modified: Fri Apr 28 14:20:43 2023, max compression
+gzip compressed data, was "tpdk-2.0.7.tar", last modified: Mon Jun  5 15:35:17 2023, max compression
```

## Comparing `tpdk-2.0.0b2.tar` & `tpdk-2.0.7.tar`

### file list

```diff
@@ -1,202 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.374167 tpdk-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 14:20:43.374167 tpdk-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 14:20:43.374167 tpdk-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.362166 tpdk-2.0.0b2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_address_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_address_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_address_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evidence_read_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_media_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_notification_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_notification_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_independent_write_seller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_offer_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_update_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_organization_write_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_parcel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_independent_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_read_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_update_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_persona_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_support_read_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_user_write_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/test/test_webhook_subscription_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.362166 tpdk-2.0.0b2/tpdk/
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.362166 tpdk-2.0.0b2/tpdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33170 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29899 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48994 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/persona_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   106167 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   147579 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    47612 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41123 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.374167 tpdk-2.0.0b2/tpdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/address_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/address_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/address_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evidence_read_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/media_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/notification_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/notification_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_independent_write_seller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/offer_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_update_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/organization_write_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/parcel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_independent_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_read_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_update_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/persona_write_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_support_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_support_read_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/user_write_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/models/webhook_subscription_write.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-04-28 14:20:30.000000 tpdk-2.0.0b2/tpdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:20:43.362166 tpdk-2.0.0b2/tpdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 14:20:43.000000 tpdk-2.0.0b2/tpdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-28 14:20:43.000000 tpdk-2.0.0b2/tpdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:20:43.000000 tpdk-2.0.0b2/tpdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 14:20:43.000000 tpdk-2.0.0b2/tpdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 14:20:43.000000 tpdk-2.0.0b2/tpdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.973115 tpdk-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-05 15:35:17.977115 tpdk-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20037 2023-06-05 15:35:09.000000 tpdk-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-05 15:35:09.000000 tpdk-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:35:17.977115 tpdk-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-05 15:35:09.000000 tpdk-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_address_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_ai_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_read_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_media_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_independent_write_seller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_update_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_organization_write_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_independent_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_read_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_update_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_persona_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_support_read_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_user_write_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-05 15:35:09.000000 tpdk-2.0.7/test/test_webhook_subscription_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/tpdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.965115 tpdk-2.0.7/tpdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50992 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107228 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158178 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41484 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.973115 tpdk-2.0.7/tpdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/address_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/ai_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_read_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/media_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_independent_write_seller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_update_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/organization_write_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_independent_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_read_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_update_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/persona_write_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_support_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_support_read_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/user_write_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/models/webhook_subscription_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-05 15:35:09.000000 tpdk-2.0.7/tpdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:35:17.961115 tpdk-2.0.7/tpdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-05 15:35:17.000000 tpdk-2.0.7/tpdk.egg-info/top_level.txt
```

### Comparing `tpdk-2.0.0b2/README.md` & `tpdk-2.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tpdk
 Our API suite for the **Resolution Center** and the **Safe Checkout** features.
 Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.0-b2
-- Package version: 2.0.0-b2
+- API version: 2.0.7
+- Package version: 2.0.7
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://tripartie.com](https://tripartie.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -47,15 +47,14 @@
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from __future__ import print_function
 
 import time
 import tpdk
 from tpdk.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://staging-api.tripartie.com
@@ -65,60 +64,72 @@
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
+# Configure API key authorization: jwtPersonalKey
+configuration.api_key['jwtPersonalKey'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['jwtPersonalKey'] = 'Bearer'
+
+# Configure API key authorization: personaAuthKey
+configuration.api_key['personaAuthKey'] = os.environ["API_KEY"]
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['personaAuthKey'] = 'Bearer'
+
 configuration.access_token = os.environ["ACCESS_TOKEN"]
 
 
 # Enter a context with an instance of the API client
 with tpdk.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = tpdk.BrandingApi(api_client)
-    id = 'id_example' # str | Organization identifier
-    organization_update = tpdk.OrganizationUpdate() # OrganizationUpdate | The updated Organization resource
+    api_instance = tpdk.AIApi(api_client)
+    ai_hint = tpdk.AiHint() # AiHint | The new AiHint resource
 
     try:
-        # Update your Organization details, branding or parameters
-        api_response = api_instance.api_organizations_id_patch(id, organization_update)
-        print("The response of BrandingApi->api_organizations_id_patch:\n")
+        # Dedicated endpoint for our artificial intelligence bot
+        api_response = api_instance.api_ai_hints_post(ai_hint)
+        print("The response of AIApi->api_ai_hints_post:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling BrandingApi->api_organizations_id_patch: %s\n" % e)
+        print("Exception when calling AIApi->api_ai_hints_post: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://staging-api.tripartie.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*AIApi* | [**api_ai_hints_post**](docs/AIApi.md#api_ai_hints_post) | **POST** /ai-hints | Dedicated endpoint for our artificial intelligence bot
 *BrandingApi* | [**api_organizations_id_patch**](docs/BrandingApi.md#api_organizations_id_patch) | **PATCH** /organizations/{id} | Update your Organization details, branding or parameters
 *BrandingApi* | [**api_organizations_idicon_delete**](docs/BrandingApi.md#api_organizations_idicon_delete) | **DELETE** /organizations/{id}/icon | Unset your Organization Icon
 *BrandingApi* | [**api_organizations_idicon_post**](docs/BrandingApi.md#api_organizations_idicon_post) | **POST** /organizations/{id}/icon | Upload your Organization Icon
 *BrandingApi* | [**api_organizations_idlogo_delete**](docs/BrandingApi.md#api_organizations_idlogo_delete) | **DELETE** /organizations/{id}/logo | Unset your Organization Logo
 *BrandingApi* | [**api_organizations_idlogo_post**](docs/BrandingApi.md#api_organizations_idlogo_post) | **POST** /organizations/{id}/logo | Upload your Organization logo
-*NotificationApi* | [**api_personas_idnotifications_get_collection**](docs/NotificationApi.md#api_personas_idnotifications_get_collection) | **GET** /personas/{id}/notifications | Retrieves the collection of Notification resources.
-*NotificationApi* | [**api_personas_persona_idnotifications_id_patch**](docs/NotificationApi.md#api_personas_persona_idnotifications_id_patch) | **PATCH** /personas/{personaId}/notifications/{id} | Updates the Notification resource.
+*NotificationApi* | [**api_personas_idnotifications_get_collection**](docs/NotificationApi.md#api_personas_idnotifications_get_collection) | **GET** /personas/{id}/notifications | Retrieve pending notifications for Persona
+*NotificationApi* | [**api_personas_persona_idnotifications_id_patch**](docs/NotificationApi.md#api_personas_persona_idnotifications_id_patch) | **PATCH** /personas/{personaId}/notifications/{id} | Mark as read/unread a notification for Persona
 *NotificationApi* | [**api_users_idnotifications_get_collection**](docs/NotificationApi.md#api_users_idnotifications_get_collection) | **GET** /users/{id}/notifications | Retrieves the collection of Notification resources.
-*NotificationApi* | [**api_users_user_idnotifications_id_patch**](docs/NotificationApi.md#api_users_user_idnotifications_id_patch) | **PATCH** /users/{userId}/notifications/{id} | Updates the Notification resource.
+*NotificationApi* | [**api_users_user_idnotifications_id_patch**](docs/NotificationApi.md#api_users_user_idnotifications_id_patch) | **PATCH** /users/{userId}/notifications/{id} | Mark as read/unread a notification for User
 *PersonaApi* | [**api_personas_get_collection**](docs/PersonaApi.md#api_personas_get_collection) | **GET** /personas | Retrieves the collection of Persona resources.
 *PersonaApi* | [**api_personas_id_delete**](docs/PersonaApi.md#api_personas_id_delete) | **DELETE** /personas/{id} | Unregister a Persona (Your customer)
 *PersonaApi* | [**api_personas_id_get**](docs/PersonaApi.md#api_personas_id_get) | **GET** /personas/{id} | Retrieves a Persona resource.
 *PersonaApi* | [**api_personas_id_patch**](docs/PersonaApi.md#api_personas_id_patch) | **PATCH** /personas/{id} | Updates the Persona resource.
 *PersonaApi* | [**api_personas_idtoken_post**](docs/PersonaApi.md#api_personas_idtoken_post) | **POST** /personas/{id}/token | Issue authenticated URL for single end-user
 *PersonaApi* | [**api_personas_post**](docs/PersonaApi.md#api_personas_post) | **POST** /personas | Register a Persona (Your customer)
 *ResolutionCenterApi* | [**api_disputes_get_collection**](docs/ResolutionCenterApi.md#api_disputes_get_collection) | **GET** /disputes | Retrieves the collection of Dispute resources.
 *ResolutionCenterApi* | [**api_disputes_post**](docs/ResolutionCenterApi.md#api_disputes_post) | **POST** /disputes | Draft a standalone Dispute
 *ResolutionCenterApi* | [**api_disputes_ulid_delete**](docs/ResolutionCenterApi.md#api_disputes_ulid_delete) | **DELETE** /disputes/{ulid} | Abandon claims on Dispute
 *ResolutionCenterApi* | [**api_disputes_ulid_get**](docs/ResolutionCenterApi.md#api_disputes_ulid_get) | **GET** /disputes/{ulid} | Retrieves a Dispute resource.
-*ResolutionCenterApi* | [**api_disputes_ulid_patch**](docs/ResolutionCenterApi.md#api_disputes_ulid_patch) | **PATCH** /disputes/{ulid} | Updates the Dispute resource.
+*ResolutionCenterApi* | [**api_disputes_ulid_patch**](docs/ResolutionCenterApi.md#api_disputes_ulid_patch) | **PATCH** /disputes/{ulid} | Update the Dispute
 *ResolutionCenterApi* | [**api_disputes_ulidevaluations_post**](docs/ResolutionCenterApi.md#api_disputes_ulidevaluations_post) | **POST** /disputes/{ulid}/evaluations | Submit an Evaluation for the Dispute
 *ResolutionCenterApi* | [**api_disputes_ulidevidences_get_collection**](docs/ResolutionCenterApi.md#api_disputes_ulidevidences_get_collection) | **GET** /disputes/{ulid}/evidences | Retrieve all Evidences in Dispute
 *ResolutionCenterApi* | [**api_disputes_ulidevidences_id_delete**](docs/ResolutionCenterApi.md#api_disputes_ulidevidences_id_delete) | **DELETE** /disputes/{ulid}/evidences/{id} | Withdraw an Evidence from a Dispute
 *ResolutionCenterApi* | [**api_disputes_ulidevidences_idmedia_post**](docs/ResolutionCenterApi.md#api_disputes_ulidevidences_idmedia_post) | **POST** /disputes/{ulid}/evidences/{id}/media | Upload attachment in regard of described Evidence
 *ResolutionCenterApi* | [**api_disputes_ulidevidences_post**](docs/ResolutionCenterApi.md#api_disputes_ulidevidences_post) | **POST** /disputes/{ulid}/evidences | Submit an Evidence to the Dispute case
 *ResolutionCenterApi* | [**api_disputes_ulidparcels_get_collection**](docs/ResolutionCenterApi.md#api_disputes_ulidparcels_get_collection) | **GET** /disputes/{ulid}/parcels | Retrieves the collection of Parcel resources.
 *ResolutionCenterApi* | [**api_disputes_ulidparcels_id_delete**](docs/ResolutionCenterApi.md#api_disputes_ulidparcels_id_delete) | **DELETE** /disputes/{ulid}/parcels/{id} | Removes the Parcel resource.
@@ -132,44 +143,44 @@
 *SafeCheckoutApi* | [**api_offers_ulidtransactions_get_collection**](docs/SafeCheckoutApi.md#api_offers_ulidtransactions_get_collection) | **GET** /offers/{ulid}/transactions | Retrieve Payment Intents for Offer
 *SafeCheckoutApi* | [**api_offers_ulidtransactions_idevaluations_post**](docs/SafeCheckoutApi.md#api_offers_ulidtransactions_idevaluations_post) | **POST** /offers/{ulid}/transactions/{id}/evaluations | Submit an Evaluation for the Offer
 *SafeCheckoutApi* | [**api_offers_ulidtransactions_post**](docs/SafeCheckoutApi.md#api_offers_ulidtransactions_post) | **POST** /offers/{ulid}/transactions | Create a Payment Intent for Offer
 *SafeCheckoutApi* | [**api_personas_idoffers_delete**](docs/SafeCheckoutApi.md#api_personas_idoffers_delete) | **DELETE** /personas/{id}/offers | Revoke an Offer for given Persona
 *SafeCheckoutApi* | [**api_personas_idoffers_get_collection**](docs/SafeCheckoutApi.md#api_personas_idoffers_get_collection) | **GET** /personas/{id}/offers | List or Search Offers for given Persona
 *SafeCheckoutApi* | [**api_personas_idoffers_patch**](docs/SafeCheckoutApi.md#api_personas_idoffers_patch) | **PATCH** /personas/{id}/offers | Update an Offer for given Persona
 *SafeCheckoutApi* | [**api_personas_idoffers_post**](docs/SafeCheckoutApi.md#api_personas_idoffers_post) | **POST** /personas/{id}/offers | Create an Offer for given Persona
+*SafeCheckoutApi* | [**api_transactions_get_collection**](docs/SafeCheckoutApi.md#api_transactions_get_collection) | **GET** /transactions | Retrieves the collection of Transaction resources.
 *SafeCheckoutApi* | [**api_transactions_uliddispute_delete**](docs/SafeCheckoutApi.md#api_transactions_uliddispute_delete) | **DELETE** /transactions/{ulid}/dispute | Abandon claims on Dispute
 *SafeCheckoutApi* | [**api_transactions_uliddispute_get**](docs/SafeCheckoutApi.md#api_transactions_uliddispute_get) | **GET** /transactions/{ulid}/dispute | Read Dispute from existing Transaction
 *SafeCheckoutApi* | [**api_transactions_uliddispute_patch**](docs/SafeCheckoutApi.md#api_transactions_uliddispute_patch) | **PATCH** /transactions/{ulid}/dispute | Interact with a Dispute
 *SafeCheckoutApi* | [**api_transactions_uliddispute_post**](docs/SafeCheckoutApi.md#api_transactions_uliddispute_post) | **POST** /transactions/{ulid}/dispute | Open a Dispute related to existing Transaction
 *SafeCheckoutApi* | [**api_transactions_ulidparcels_get_collection**](docs/SafeCheckoutApi.md#api_transactions_ulidparcels_get_collection) | **GET** /transactions/{ulid}/parcels | Read shipments from Transaction
 *SafeCheckoutApi* | [**api_transactions_ulidparcels_id_delete**](docs/SafeCheckoutApi.md#api_transactions_ulidparcels_id_delete) | **DELETE** /transactions/{ulid}/parcels/{id} | Withdraw shipment from Transaction
 *SafeCheckoutApi* | [**api_transactions_ulidparcels_post**](docs/SafeCheckoutApi.md#api_transactions_ulidparcels_post) | **POST** /transactions/{ulid}/parcels | Manually declare package shipped for Transaction
-*TransactionApi* | [**api_transactions_get_collection**](docs/TransactionApi.md#api_transactions_get_collection) | **GET** /transactions | Retrieves the collection of Transaction resources.
-*UserApi* | [**api_organizations_id_patch**](docs/UserApi.md#api_organizations_id_patch) | **PATCH** /organizations/{id} | Update your Organization details, branding or parameters
 *UserApi* | [**api_personasauthentication_post**](docs/UserApi.md#api_personasauthentication_post) | **POST** /personas/authentication | Persona Authentication
 *UserApi* | [**api_personasregister_post**](docs/UserApi.md#api_personasregister_post) | **POST** /personas/register | Persona external registration
 *UserApi* | [**api_register_post**](docs/UserApi.md#api_register_post) | **POST** /register | Organization onboarding
 *UserApi* | [**api_users_get_collection**](docs/UserApi.md#api_users_get_collection) | **GET** /users | Retrieves the collection of User resources.
 *UserApi* | [**api_users_id_get**](docs/UserApi.md#api_users_id_get) | **GET** /users/{id} | Retrieves a User resource.
 *UserApi* | [**api_users_idemail_validation_patch**](docs/UserApi.md#api_users_idemail_validation_patch) | **PATCH** /users/{id}/email-validation | Validate email ownership
 *WebhookApi* | [**api_webhook_histories_get_collection**](docs/WebhookApi.md#api_webhook_histories_get_collection) | **GET** /webhook-histories | Retrieves the collection of WebhookHistory resources.
 *WebhookApi* | [**api_webhook_histories_id_get**](docs/WebhookApi.md#api_webhook_histories_id_get) | **GET** /webhook-histories/{id} | Retrieves a WebhookHistory resource.
-*WebhookApi* | [**api_webhook_histories_id_put**](docs/WebhookApi.md#api_webhook_histories_id_put) | **PUT** /webhook-histories/{id} | Replay a Webhook that ended in failure
+*WebhookApi* | [**api_webhook_histories_id_put**](docs/WebhookApi.md#api_webhook_histories_id_put) | **PUT** /webhook-histories/{id} | Replay a Webhook that ended up in failure
 *WebhookApi* | [**api_webhook_subscriptions_get_collection**](docs/WebhookApi.md#api_webhook_subscriptions_get_collection) | **GET** /webhook-subscriptions | Retrieves the collection of WebhookSubscription resources.
 *WebhookApi* | [**api_webhook_subscriptions_id_delete**](docs/WebhookApi.md#api_webhook_subscriptions_id_delete) | **DELETE** /webhook-subscriptions/{id} | Removes the WebhookSubscription resource.
 *WebhookApi* | [**api_webhook_subscriptions_post**](docs/WebhookApi.md#api_webhook_subscriptions_post) | **POST** /webhook-subscriptions | Subscribe to Event(s)
 
 
 ## Documentation For Models
 
  - [Address](docs/Address.md)
  - [AddressIndependentWrite](docs/AddressIndependentWrite.md)
  - [AddressRead](docs/AddressRead.md)
  - [AddressUpdate](docs/AddressUpdate.md)
  - [AddressWrite](docs/AddressWrite.md)
+ - [AiHint](docs/AiHint.md)
  - [ApiClient](docs/ApiClient.md)
  - [Dispute](docs/Dispute.md)
  - [DisputeCollectionRead](docs/DisputeCollectionRead.md)
  - [DisputeIndependentWrite](docs/DisputeIndependentWrite.md)
  - [DisputePostCreationRead](docs/DisputePostCreationRead.md)
  - [DisputeRead](docs/DisputeRead.md)
  - [DisputeUpdate](docs/DisputeUpdate.md)
@@ -210,14 +221,16 @@
  - [ParcelRead](docs/ParcelRead.md)
  - [ParcelWrite](docs/ParcelWrite.md)
  - [Persona](docs/Persona.md)
  - [PersonaAddress](docs/PersonaAddress.md)
  - [PersonaCollectionRead](docs/PersonaCollectionRead.md)
  - [PersonaIndependentWrite](docs/PersonaIndependentWrite.md)
  - [PersonaIndependentWriteAddress](docs/PersonaIndependentWriteAddress.md)
+ - [PersonaPersonaAuthReturn](docs/PersonaPersonaAuthReturn.md)
+ - [PersonaPersonaExternalAuth](docs/PersonaPersonaExternalAuth.md)
  - [PersonaPostAuthRead](docs/PersonaPostAuthRead.md)
  - [PersonaRead](docs/PersonaRead.md)
  - [PersonaReadAddress](docs/PersonaReadAddress.md)
  - [PersonaRegister](docs/PersonaRegister.md)
  - [PersonaToken](docs/PersonaToken.md)
  - [PersonaUpdate](docs/PersonaUpdate.md)
  - [PersonaUpdateAddress](docs/PersonaUpdateAddress.md)
@@ -241,18 +254,21 @@
  - [WebhookHistoryCollectionRead](docs/WebhookHistoryCollectionRead.md)
  - [WebhookHistoryRead](docs/WebhookHistoryRead.md)
  - [WebhookObject](docs/WebhookObject.md)
  - [WebhookSubscriptionRead](docs/WebhookSubscriptionRead.md)
  - [WebhookSubscriptionWrite](docs/WebhookSubscriptionWrite.md)
 
 
+<a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
-## oauth
+Authentication schemes defined for the API:
+<a id="oauth"></a>
+### oauth
 
 - **Type**: OAuth
 - **Flow**: application
 - **Authorization URL**: 
 - **Scopes**: 
  - **OFFER_READ**: Read-only operations on safe-checkout offers
  - **OFFER_WRITE**: Write permissions on safe-checkout offers
@@ -261,27 +277,28 @@
  - **DISPUTE_ARBITRATION**: Update permission on disputes for manual arbitration only
  - **ORGANIZATION_READ**: Read organization details and stats
  - **RULING_READ**: Read custom rules applied to the dispute resolution program
  - **RULING_WRITE**: Write custom rules applied to the dispute resolution program
  - **PERSONA_READ**: Read operations on the shared user-base knowledge
  - **PERSONA_WRITE**: Write permissions on the shared user-base knowledge
  - **PERSONA_AUTH**: Capability to issue short-term lived authenticated URL
+ - **INTERNAL_WRITE**: Special internal scope
 
-
-## jwtPersonalKey
+<a id="jwtPersonalKey"></a>
+### jwtPersonalKey
 
 - **Type**: API key
 - **API key parameter name**: Authorization
 - **Location**: HTTP header
 
-
-## personaAuthKey
+<a id="personaAuthKey"></a>
+### personaAuthKey
 
 - **Type**: API key
-- **API key parameter name**: X-Persona-Auth
+- **API key parameter name**: X-Persona-Authorization
 - **Location**: HTTP header
 
 
 ## Author
 
 noc@tripartie.com
```

### Comparing `tpdk-2.0.0b2/pyproject.toml` & `tpdk-2.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "tpdk"
-version = "2.0.0-b2"
+version = "2.0.7"
 description = "Tripartie"
-authors = ["noc@tripartie.com"]
+authors = ["Tripartie SAS <noc@tripartie.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/tpdk/tripartie"
+repository = "https://github.com/tripartie/tpdk"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Tripartie"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
-pydantic = ">= 1.10.5"
+pydantic = "^1.10.5, <2"
 aenum = ">=3.1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2.1"
-tox = ">=4.4.6"
-flake8 = ">=6.0.0"
+tox = ">=3.9.0"
+flake8 = ">=4.0.0"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
+
+[tool.pylint.'MESSAGES CONTROL']
+extension-pkg-whitelist = "pydantic"
```

### Comparing `tpdk-2.0.0b2/setup.py` & `tpdk-2.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,20 +18,20 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "tpdk"
-VERSION = "2.0.0-b2"
+VERSION = "2.0.7"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
-    "pydantic",
+    "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Tripartie",
```

### Comparing `tpdk-2.0.0b2/test/test_address.py` & `tpdk-2.0.7/test/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_address_independent_write.py` & `tpdk-2.0.7/test/test_address_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_address_read.py` & `tpdk-2.0.7/test/test_address_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_address_update.py` & `tpdk-2.0.7/test/test_address_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_address_write.py` & `tpdk-2.0.7/test/test_address_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_api_client.py` & `tpdk-2.0.7/test/test_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,15 +39,14 @@
         model = tpdk.models.api_client.ApiClient()  # noqa: E501
         if include_optional :
             return ApiClient(
                 identifier = '', 
                 owner = '', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 secret = '', 
-                monthly_quota = 56, 
                 name = '', 
                 redirect_uris = [
                     tpdk.models.redirect_uri.RedirectUri()
                     ], 
                 grants = [
                     tpdk.models.grant.Grant()
                     ],
```

### Comparing `tpdk-2.0.0b2/test/test_branding_api.py` & `tpdk-2.0.7/test/test_branding_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_dispute.py` & `tpdk-2.0.7/test/test_dispute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -81,14 +81,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ], 
                 metadata = [
                     tpdk.models.metadata.Metadata(
                         id = 56, 
                         key = 'External-ID', 
                         value = '54412', )
@@ -123,14 +124,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ],
                 metadata = [
                     tpdk.models.metadata.Metadata(
                         id = 56, 
                         key = 'External-ID', 
                         value = '54412', )
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_collection_read.py` & `tpdk-2.0.7/test/test_dispute_collection_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_independent_write.py` & `tpdk-2.0.7/test/test_dispute_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -48,14 +48,15 @@
                         description = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.', 
                         unit_price = 125.54, 
                         currency_code = 'EUR', 
                         item_count = 1, 
                         condition = 'USED', 
                         weight_in_gram = 56, 
                         ean_code = '4718017388450', 
+                        can_be_sold_separately = True, 
                         metadata = [
                             tpdk.models.metadata_independent_write.Metadata-IndependentWrite(
                                 key = 'External-ID', 
                                 value = '54412', )
                             ], ), 
                     buyer = tpdk.models.persona_independent_write.Persona-IndependentWrite(
                         first_name = 'John',
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_post_creation_read.py` & `tpdk-2.0.7/test/test_dispute_post_creation_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_read.py` & `tpdk-2.0.7/test/test_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_update.py` & `tpdk-2.0.7/test/test_dispute_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_dispute_write.py` & `tpdk-2.0.7/test/test_dispute_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evaluation_read.py` & `tpdk-2.0.7/test/test_evaluation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evaluation_write.py` & `tpdk-2.0.7/test/test_evaluation_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evidence.py` & `tpdk-2.0.7/test/test_evidence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evidence_read.py` & `tpdk-2.0.7/test/test_evidence_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evidence_read_media.py` & `tpdk-2.0.7/test/test_evidence_read_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_evidence_write.py` & `tpdk-2.0.7/test/test_evidence_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_media.py` & `tpdk-2.0.7/test/test_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_media_read.py` & `tpdk-2.0.7/test/test_media_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_message.py` & `tpdk-2.0.7/test/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_metadata.py` & `tpdk-2.0.7/test/test_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_metadata_independent_write.py` & `tpdk-2.0.7/test/test_metadata_independent_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_metadata_read.py` & `tpdk-2.0.7/test/test_metadata_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_metadata_update.py` & `tpdk-2.0.7/test/test_metadata_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_metadata_write.py` & `tpdk-2.0.7/test/test_metadata_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_notification.py` & `tpdk-2.0.7/test/test_notification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_notification_api.py` & `tpdk-2.0.7/test/test_notification_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -28,35 +28,35 @@
 
     def tearDown(self):
         pass
 
     def test_api_personas_idnotifications_get_collection(self):
         """Test case for api_personas_idnotifications_get_collection
 
-        Retrieves the collection of Notification resources.  # noqa: E501
+        Retrieve pending notifications for Persona  # noqa: E501
         """
         pass
 
     def test_api_personas_persona_idnotifications_id_patch(self):
         """Test case for api_personas_persona_idnotifications_id_patch
 
-        Updates the Notification resource.  # noqa: E501
+        Mark as read/unread a notification for Persona  # noqa: E501
         """
         pass
 
     def test_api_users_idnotifications_get_collection(self):
         """Test case for api_users_idnotifications_get_collection
 
         Retrieves the collection of Notification resources.  # noqa: E501
         """
         pass
 
     def test_api_users_user_idnotifications_id_patch(self):
         """Test case for api_users_user_idnotifications_id_patch
 
-        Updates the Notification resource.  # noqa: E501
+        Mark as read/unread a notification for User  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tpdk-2.0.0b2/test/test_notification_read.py` & `tpdk-2.0.7/test/test_notification_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_notification_update.py` & `tpdk-2.0.7/test/test_notification_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_offer.py` & `tpdk-2.0.7/test/test_offer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -58,14 +58,15 @@
                 weight_in_gram = 56, 
                 shipping_allowed = True, 
                 hand_delivery_allowed = True, 
                 shipping_carriers = [
                     'SwissPost'
                     ], 
                 ean_code = '4718017388450', 
+                can_be_sold_separately = True, 
                 metadata = [
                     tpdk.models.metadata.Metadata(
                         id = 56, 
                         key = 'External-ID', 
                         value = '54412', )
                     ], 
                 medias = [
@@ -75,14 +76,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ], 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 iri = ''
             )
         else :
@@ -95,14 +97,15 @@
                 item_count = 1,
                 condition = 'USED',
                 shipping_allowed = True,
                 hand_delivery_allowed = True,
                 shipping_carriers = [
                     'SwissPost'
                     ],
+                can_be_sold_separately = True,
                 metadata = [
                     tpdk.models.metadata.Metadata(
                         id = 56, 
                         key = 'External-ID', 
                         value = '54412', )
                     ],
                 medias = [
@@ -112,14 +115,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ],
         )
         """
 
     def testOffer(self):
         """Test Offer"""
```

### Comparing `tpdk-2.0.0b2/test/test_offer_collection_read.py` & `tpdk-2.0.7/test/test_offer_collection_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_independent_write.py` & `tpdk-2.0.7/test/test_offer_independent_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -46,25 +46,27 @@
                 description = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.', 
                 unit_price = 125.54, 
                 currency_code = 'EUR', 
                 item_count = 1, 
                 condition = 'USED', 
                 weight_in_gram = 56, 
                 ean_code = '4718017388450', 
+                can_be_sold_separately = True, 
                 metadata = [
                     tpdk.models.metadata_independent_write.Metadata-IndependentWrite(
                         key = 'External-ID', 
                         value = '54412', )
                     ]
             )
         else :
             return OfferIndependentWrite(
                 nature = 'physical_item',
                 item_count = 1,
                 condition = 'USED',
+                can_be_sold_separately = True,
                 metadata = [
                     tpdk.models.metadata_independent_write.Metadata-IndependentWrite(
                         key = 'External-ID', 
                         value = '54412', )
                     ],
         )
         """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_independent_write_seller.py` & `tpdk-2.0.7/test/test_offer_independent_write_seller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_post_creation_read.py` & `tpdk-2.0.7/test/test_offer_post_creation_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_read.py` & `tpdk-2.0.7/test/test_offer_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_update.py` & `tpdk-2.0.7/test/test_offer_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -51,14 +51,15 @@
                 weight_in_gram = 56, 
                 shipping_allowed = True, 
                 hand_delivery_allowed = True, 
                 shipping_carriers = [
                     'SwissPost'
                     ], 
                 ean_code = '4718017388450', 
+                can_be_sold_separately = True, 
                 metadata = [
                     tpdk.models.metadata_update.Metadata-Update(
                         key = 'External-ID', 
                         value = '54412', )
                     ]
             )
         else :
@@ -67,14 +68,15 @@
                 override_rate_commission_safe_checkout = 1.337,
                 item_count = 1,
                 shipping_allowed = True,
                 hand_delivery_allowed = True,
                 shipping_carriers = [
                     'SwissPost'
                     ],
+                can_be_sold_separately = True,
                 metadata = [
                     tpdk.models.metadata_update.Metadata-Update(
                         key = 'External-ID', 
                         value = '54412', )
                     ],
         )
         """
```

### Comparing `tpdk-2.0.0b2/test/test_offer_write.py` & `tpdk-2.0.7/test/test_offer_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -52,14 +52,15 @@
                 weight_in_gram = 56, 
                 shipping_allowed = True, 
                 hand_delivery_allowed = True, 
                 shipping_carriers = [
                     'SwissPost'
                     ], 
                 ean_code = '4718017388450', 
+                can_be_sold_separately = True, 
                 metadata = [
                     tpdk.models.metadata_write.Metadata-Write(
                         key = 'External-ID', 
                         value = '54412', )
                     ]
             )
         else :
@@ -69,14 +70,15 @@
                 item_count = 1,
                 condition = 'USED',
                 shipping_allowed = True,
                 hand_delivery_allowed = True,
                 shipping_carriers = [
                     'SwissPost'
                     ],
+                can_be_sold_separately = True,
                 metadata = [
                     tpdk.models.metadata_write.Metadata-Write(
                         key = 'External-ID', 
                         value = '54412', )
                     ],
         )
         """
```

### Comparing `tpdk-2.0.0b2/test/test_organization_read.py` & `tpdk-2.0.7/test/test_organization_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_organization_support_read.py` & `tpdk-2.0.7/test/test_organization_support_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_organization_update.py` & `tpdk-2.0.7/test/test_organization_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -38,32 +38,33 @@
         """
         model = tpdk.models.organization_update.OrganizationUpdate()  # noqa: E501
         if include_optional :
             return OrganizationUpdate(
                 name = '', 
                 vat_number = '', 
                 commercial_registry_number = '', 
+                webhook_url = '', 
                 website_url = '', 
                 custom_base_url = '', 
                 billing_address = None, 
                 primary_color = '', 
                 secondary_color = '', 
                 accent_color = '', 
                 error_color = '', 
                 info_color = '', 
                 success_color = '', 
                 warning_color = '', 
-                end_user_notification_toggle = True, 
+                direct_notification_toggle = True, 
                 anonymity_level = 'PARTIAL_FIRST_NAME', 
                 flat_rate_enabled = True, 
                 rate_commission_safe_checkout = 1.337
             )
         else :
             return OrganizationUpdate(
-                end_user_notification_toggle = True,
+                direct_notification_toggle = True,
                 anonymity_level = 'PARTIAL_FIRST_NAME',
                 rate_commission_safe_checkout = 1.337,
         )
         """
 
     def testOrganizationUpdate(self):
         """Test OrganizationUpdate"""
```

### Comparing `tpdk-2.0.0b2/test/test_organization_update_billing_address.py` & `tpdk-2.0.7/test/test_organization_update_billing_address.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_organization_write.py` & `tpdk-2.0.7/test/test_organization_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_organization_write_billing_address.py` & `tpdk-2.0.7/test/test_organization_write_billing_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_parcel.py` & `tpdk-2.0.7/test/test_parcel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_parcel_independent_write.py` & `tpdk-2.0.7/test/test_parcel_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_parcel_read.py` & `tpdk-2.0.7/test/test_parcel_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_parcel_write.py` & `tpdk-2.0.7/test/test_parcel_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona.py` & `tpdk-2.0.7/test/test_persona.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -84,14 +84,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ], 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 offer_count = 4, 
                 purchase_count = 42, 
                 roles = [
@@ -126,14 +127,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ],
         )
         """
 
     def testPersona(self):
         """Test Persona"""
```

### Comparing `tpdk-2.0.0b2/test/test_persona_address.py` & `tpdk-2.0.7/test/test_persona_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_api.py` & `tpdk-2.0.7/test/test_persona_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_collection_read.py` & `tpdk-2.0.7/test/test_persona_collection_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_independent_write.py` & `tpdk-2.0.7/test/test_persona_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_independent_write_address.py` & `tpdk-2.0.7/test/test_persona_independent_write_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_post_auth_read.py` & `tpdk-2.0.7/test/test_persona_post_auth_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_read.py` & `tpdk-2.0.7/test/test_persona_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_read_address.py` & `tpdk-2.0.7/test/test_persona_read_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_register.py` & `tpdk-2.0.7/test/test_persona_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_token.py` & `tpdk-2.0.7/test/test_persona_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_update.py` & `tpdk-2.0.7/test/test_persona_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_update_address.py` & `tpdk-2.0.7/test/test_persona_update_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_write.py` & `tpdk-2.0.7/test/test_persona_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_persona_write_address.py` & `tpdk-2.0.7/test/test_persona_write_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_resolution_center_api.py` & `tpdk-2.0.7/test/test_resolution_center_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -56,15 +56,15 @@
         Retrieves a Dispute resource.  # noqa: E501
         """
         pass
 
     def test_api_disputes_ulid_patch(self):
         """Test case for api_disputes_ulid_patch
 
-        Updates the Dispute resource.  # noqa: E501
+        Update the Dispute  # noqa: E501
         """
         pass
 
     def test_api_disputes_ulidevaluations_post(self):
         """Test case for api_disputes_ulidevaluations_post
 
         Submit an Evaluation for the Dispute  # noqa: E501
```

### Comparing `tpdk-2.0.0b2/test/test_safe_checkout_api.py` & `tpdk-2.0.7/test/test_safe_checkout_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -109,14 +109,21 @@
     def test_api_personas_idoffers_post(self):
         """Test case for api_personas_idoffers_post
 
         Create an Offer for given Persona  # noqa: E501
         """
         pass
 
+    def test_api_transactions_get_collection(self):
+        """Test case for api_transactions_get_collection
+
+        Retrieves the collection of Transaction resources.  # noqa: E501
+        """
+        pass
+
     def test_api_transactions_uliddispute_delete(self):
         """Test case for api_transactions_uliddispute_delete
 
         Abandon claims on Dispute  # noqa: E501
         """
         pass
```

### Comparing `tpdk-2.0.0b2/test/test_transaction_collection_read.py` & `tpdk-2.0.7/test/test_transaction_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_transaction_independent_write.py` & `tpdk-2.0.7/test/test_transaction_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -47,14 +47,15 @@
                     description = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.', 
                     unit_price = 125.54, 
                     currency_code = 'EUR', 
                     item_count = 1, 
                     condition = 'USED', 
                     weight_in_gram = 56, 
                     ean_code = '4718017388450', 
+                    can_be_sold_separately = True, 
                     metadata = [
                         tpdk.models.metadata_independent_write.Metadata-IndependentWrite(
                             key = 'External-ID', 
                             value = '54412', )
                         ], ), 
                 buyer = tpdk.models.persona_independent_write.Persona-IndependentWrite(
                     first_name = 'John',
```

### Comparing `tpdk-2.0.0b2/test/test_transaction_read.py` & `tpdk-2.0.7/test/test_transaction_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_unprocessable_entity.py` & `tpdk-2.0.7/test/test_unprocessable_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_unprocessable_entity_violations_inner.py` & `tpdk-2.0.7/test/test_unprocessable_entity_violations_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user.py` & `tpdk-2.0.7/test/test_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -71,14 +71,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ], 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 consent_mail_notification = True, 
                 consent_mail_ads = True, 
                 api = None, 
@@ -98,14 +99,15 @@
                     tpdk.models.view.View(
                         id = 56, 
                         ip_address = '', 
                         offer = '', 
                         dispute = '', 
                         persona = '', 
                         user = '', 
+                        hit_count = 1, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
                     ],
                 consent_mail_notification = True,
                 consent_mail_ads = True,
         )
         """
```

### Comparing `tpdk-2.0.0b2/test/test_user_api.py` & `tpdk-2.0.7/test/test_user_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,15 +39,14 @@
         model = tpdk.models.user_api.UserApi()  # noqa: E501
         if include_optional :
             return UserApi(
                 identifier = '', 
                 owner = '', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 secret = '', 
-                monthly_quota = 56, 
                 name = '', 
                 redirect_uris = [
                     tpdk.models.redirect_uri.RedirectUri()
                     ], 
                 grants = [
                     tpdk.models.grant.Grant()
                     ],
```

### Comparing `tpdk-2.0.0b2/test/test_user_email_validation_write.py` & `tpdk-2.0.7/test/test_user_email_validation_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user_post_register_read.py` & `tpdk-2.0.7/test/test_user_post_register_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user_support_read.py` & `tpdk-2.0.7/test/test_user_support_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user_support_read_organization.py` & `tpdk-2.0.7/test/test_user_support_read_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user_write.py` & `tpdk-2.0.7/test/test_user_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_user_write_organization.py` & `tpdk-2.0.7/test/test_user_write_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_view.py` & `tpdk-2.0.7/test/test_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -41,19 +41,21 @@
             return View(
                 id = 56, 
                 ip_address = '', 
                 offer = '', 
                 dispute = '', 
                 persona = '', 
                 user = '', 
+                hit_count = 1, 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
             return View(
                 ip_address = '',
+                hit_count = 1,
         )
         """
 
     def testView(self):
         """Test View"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `tpdk-2.0.0b2/test/test_webhook.py` & `tpdk-2.0.7/test/test_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_api.py` & `tpdk-2.0.7/test/test_webhook_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -42,15 +42,15 @@
         Retrieves a WebhookHistory resource.  # noqa: E501
         """
         pass
 
     def test_api_webhook_histories_id_put(self):
         """Test case for api_webhook_histories_id_put
 
-        Replay a Webhook that ended in failure  # noqa: E501
+        Replay a Webhook that ended up in failure  # noqa: E501
         """
         pass
 
     def test_api_webhook_subscriptions_get_collection(self):
         """Test case for api_webhook_subscriptions_get_collection
 
         Retrieves the collection of WebhookSubscription resources.  # noqa: E501
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_history_collection_read.py` & `tpdk-2.0.7/test/test_webhook_history_collection_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_history_read.py` & `tpdk-2.0.7/test/test_webhook_history_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_object.py` & `tpdk-2.0.7/test/test_webhook_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_subscription_read.py` & `tpdk-2.0.7/test/test_webhook_subscription_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/test/test_webhook_subscription_write.py` & `tpdk-2.0.7/test/test_webhook_subscription_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/tpdk/__init__.py` & `tpdk-2.0.7/tpdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,49 +3,52 @@
 # flake8: noqa
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "2.0.0-b2"
+__version__ = "2.0.7"
 
 # import apis into sdk package
+from tpdk.api.ai_api import AIApi
 from tpdk.api.branding_api import BrandingApi
 from tpdk.api.notification_api import NotificationApi
 from tpdk.api.persona_api import PersonaApi
 from tpdk.api.resolution_center_api import ResolutionCenterApi
 from tpdk.api.safe_checkout_api import SafeCheckoutApi
-from tpdk.api.transaction_api import TransactionApi
 from tpdk.api.user_api import UserApi
 from tpdk.api.webhook_api import WebhookApi
 
 # import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.api_client import ApiClient
 from tpdk.configuration import Configuration
 from tpdk.exceptions import OpenApiException
 from tpdk.exceptions import ApiTypeError
 from tpdk.exceptions import ApiValueError
 from tpdk.exceptions import ApiKeyError
 from tpdk.exceptions import ApiAttributeError
 from tpdk.exceptions import ApiException
+
 # import models into sdk package
 from tpdk.models.address import Address
 from tpdk.models.address_independent_write import AddressIndependentWrite
 from tpdk.models.address_read import AddressRead
 from tpdk.models.address_update import AddressUpdate
 from tpdk.models.address_write import AddressWrite
+from tpdk.models.ai_hint import AiHint
 from tpdk.models.api_client import ApiClient
 from tpdk.models.dispute import Dispute
 from tpdk.models.dispute_collection_read import DisputeCollectionRead
 from tpdk.models.dispute_independent_write import DisputeIndependentWrite
 from tpdk.models.dispute_post_creation_read import DisputePostCreationRead
 from tpdk.models.dispute_read import DisputeRead
 from tpdk.models.dispute_update import DisputeUpdate
@@ -86,14 +89,16 @@
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 from tpdk.models.persona import Persona
 from tpdk.models.persona_address import PersonaAddress
 from tpdk.models.persona_collection_read import PersonaCollectionRead
 from tpdk.models.persona_independent_write import PersonaIndependentWrite
 from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
+from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
+from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_read_address import PersonaReadAddress
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.persona_token import PersonaToken
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_update_address import PersonaUpdateAddress
```

### Comparing `tpdk-2.0.0b2/tpdk/api/branding_api.py` & `tpdk-2.0.7/tpdk/api/branding_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
+from pydantic import Field, StrictBytes, StrictStr
 
-from typing import Optional
+from typing import Optional, Union
 
 from tpdk.models.media_read import MediaRead
 from tpdk.models.organization_read import OrganizationRead
 from tpdk.models.organization_update import OrganizationUpdate
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class BrandingApi(object):
@@ -58,32 +61,30 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param organization_update: The updated Organization resource (required)
         :type organization_update: OrganizationUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: OrganizationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_organizations_id_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_organizations_id_patch_with_http_info(id, organization_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_organizations_id_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], organization_update : Annotated[OrganizationUpdate, Field(..., description="The updated Organization resource")], **kwargs):  # noqa: E501
+    def api_organizations_id_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], organization_update : Annotated[OrganizationUpdate, Field(..., description="The updated Organization resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Update your Organization details, branding or parameters  # noqa: E501
 
         Updates the Organization resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_id_patch_with_http_info(id, organization_update, async_req=True)
@@ -91,21 +92,22 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param organization_update: The updated Organization resource (required)
         :type organization_update: OrganizationUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -158,36 +160,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['organization_update']:
+        if _params['organization_update'] is not None:
             _body_params = _params['organization_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "OrganizationRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/organizations/{id}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -214,52 +216,51 @@
         >>> thread = api.api_organizations_idicon_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_organizations_idicon_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_organizations_idicon_delete_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_organizations_idicon_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], **kwargs):  # noqa: E501
+    def api_organizations_idicon_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Unset your Organization Icon  # noqa: E501
 
         Removes the Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idicon_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -312,15 +313,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/organizations/{id}/icon', 'DELETE',
             _path_params,
             _query_params,
@@ -334,15 +335,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_organizations_idicon_post(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[StrictStr] = None, **kwargs) -> MediaRead:  # noqa: E501
+    def api_organizations_idicon_post(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> MediaRead:  # noqa: E501
         """Upload your Organization Icon  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idicon_post(id, file, async_req=True)
@@ -350,32 +351,30 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MediaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_organizations_idicon_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_organizations_idicon_post_with_http_info(id, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_organizations_idicon_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def api_organizations_idicon_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Upload your Organization Icon  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idicon_post_with_http_info(id, file, async_req=True)
@@ -383,21 +382,22 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -465,20 +465,20 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "MediaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/organizations/{id}/icon', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -505,52 +505,51 @@
         >>> thread = api.api_organizations_idlogo_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_organizations_idlogo_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_organizations_idlogo_delete_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_organizations_idlogo_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], **kwargs):  # noqa: E501
+    def api_organizations_idlogo_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Unset your Organization Logo  # noqa: E501
 
         Removes the Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idlogo_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -603,15 +602,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/organizations/{id}/logo', 'DELETE',
             _path_params,
             _query_params,
@@ -625,15 +624,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_organizations_idlogo_post(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[StrictStr] = None, **kwargs) -> MediaRead:  # noqa: E501
+    def api_organizations_idlogo_post(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> MediaRead:  # noqa: E501
         """Upload your Organization logo  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idlogo_post(id, file, async_req=True)
@@ -641,32 +640,30 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MediaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_organizations_idlogo_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_organizations_idlogo_post_with_http_info(id, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_organizations_idlogo_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def api_organizations_idlogo_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Upload your Organization logo  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_organizations_idlogo_post_with_http_info(id, file, async_req=True)
@@ -674,21 +671,22 @@
 
         :param id: Organization identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -756,20 +754,20 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "MediaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/organizations/{id}/logo', 'POST',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/notification_api.py` & `tpdk-2.0.7/tpdk/api/notification_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from tpdk.models.notification import Notification
 from tpdk.models.notification_read import NotificationRead
 from tpdk.models.notification_update import NotificationUpdate
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class NotificationApi(object):
@@ -43,69 +46,68 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
     def api_personas_idnotifications_get_collection(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> List[Notification]:  # noqa: E501
-        """Retrieves the collection of Notification resources.  # noqa: E501
+        """Retrieve pending notifications for Persona  # noqa: E501
 
         Retrieves the collection of Notification resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idnotifications_get_collection(id, page, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[Notification]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idnotifications_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idnotifications_get_collection_with_http_info(id, page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idnotifications_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
-        """Retrieves the collection of Notification resources.  # noqa: E501
+    def api_personas_idnotifications_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Retrieve pending notifications for Persona  # noqa: E501
 
         Retrieves the collection of Notification resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idnotifications_get_collection_with_http_info(id, page, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -166,15 +168,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
             '200': "List[Notification]",
         }
 
         return self.api_client.call_api(
             '/personas/{id}/notifications', 'GET',
@@ -191,15 +193,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def api_personas_persona_idnotifications_id_patch(self, persona_id : Annotated[StrictStr, Field(..., description="Persona identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification : Annotated[Notification, Field(..., description="The updated Notification resource")], **kwargs) -> Notification:  # noqa: E501
-        """Updates the Notification resource.  # noqa: E501
+        """Mark as read/unread a notification for Persona  # noqa: E501
 
         Updates the Notification resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_persona_idnotifications_id_patch(persona_id, id, notification, async_req=True)
         >>> result = thread.get()
@@ -208,33 +210,31 @@
         :type persona_id: str
         :param id: Notification identifier (required)
         :type id: str
         :param notification: The updated Notification resource (required)
         :type notification: Notification
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: Notification
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_persona_idnotifications_id_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_persona_idnotifications_id_patch_with_http_info(persona_id, id, notification, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_persona_idnotifications_id_patch_with_http_info(self, persona_id : Annotated[StrictStr, Field(..., description="Persona identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification : Annotated[Notification, Field(..., description="The updated Notification resource")], **kwargs):  # noqa: E501
-        """Updates the Notification resource.  # noqa: E501
+    def api_personas_persona_idnotifications_id_patch_with_http_info(self, persona_id : Annotated[StrictStr, Field(..., description="Persona identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification : Annotated[Notification, Field(..., description="The updated Notification resource")], **kwargs) -> ApiResponse:  # noqa: E501
+        """Mark as read/unread a notification for Persona  # noqa: E501
 
         Updates the Notification resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_persona_idnotifications_id_patch_with_http_info(persona_id, id, notification, async_req=True)
         >>> result = thread.get()
@@ -243,21 +243,22 @@
         :type persona_id: str
         :param id: Notification identifier (required)
         :type id: str
         :param notification: The updated Notification resource (required)
         :type notification: Notification
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -314,36 +315,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['notification']:
+        if _params['notification'] is not None:
             _body_params = _params['notification']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
             '200': "Notification",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/personas/{personaId}/notifications/{id}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -372,32 +373,30 @@
 
         :param id: User identifier (required)
         :type id: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[NotificationRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_users_idnotifications_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_users_idnotifications_get_collection_with_http_info(id, page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_users_idnotifications_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
+    def api_users_idnotifications_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of Notification resources.  # noqa: E501
 
         Retrieves the collection of Notification resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_idnotifications_get_collection_with_http_info(id, page, async_req=True)
@@ -405,21 +404,22 @@
 
         :param id: User identifier (required)
         :type id: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -505,15 +505,15 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def api_users_user_idnotifications_id_patch(self, user_id : Annotated[StrictStr, Field(..., description="User identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification_update : Annotated[NotificationUpdate, Field(..., description="The updated Notification resource")], **kwargs) -> NotificationRead:  # noqa: E501
-        """Updates the Notification resource.  # noqa: E501
+        """Mark as read/unread a notification for User  # noqa: E501
 
         Updates the Notification resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_user_idnotifications_id_patch(user_id, id, notification_update, async_req=True)
         >>> result = thread.get()
@@ -522,33 +522,31 @@
         :type user_id: str
         :param id: Notification identifier (required)
         :type id: str
         :param notification_update: The updated Notification resource (required)
         :type notification_update: NotificationUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: NotificationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_users_user_idnotifications_id_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_users_user_idnotifications_id_patch_with_http_info(user_id, id, notification_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_users_user_idnotifications_id_patch_with_http_info(self, user_id : Annotated[StrictStr, Field(..., description="User identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification_update : Annotated[NotificationUpdate, Field(..., description="The updated Notification resource")], **kwargs):  # noqa: E501
-        """Updates the Notification resource.  # noqa: E501
+    def api_users_user_idnotifications_id_patch_with_http_info(self, user_id : Annotated[StrictStr, Field(..., description="User identifier")], id : Annotated[StrictStr, Field(..., description="Notification identifier")], notification_update : Annotated[NotificationUpdate, Field(..., description="The updated Notification resource")], **kwargs) -> ApiResponse:  # noqa: E501
+        """Mark as read/unread a notification for User  # noqa: E501
 
         Updates the Notification resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_user_idnotifications_id_patch_with_http_info(user_id, id, notification_update, async_req=True)
         >>> result = thread.get()
@@ -557,21 +555,22 @@
         :type user_id: str
         :param id: Notification identifier (required)
         :type id: str
         :param notification_update: The updated Notification resource (required)
         :type notification_update: NotificationUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -628,36 +627,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['notification_update']:
+        if _params['notification_update'] is not None:
             _body_params = _params['notification_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {
             '200': "NotificationRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/users/{userId}/notifications/{id}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/persona_api.py` & `tpdk-2.0.7/tpdk/api/persona_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, conlist
 
 from typing import List, Optional
@@ -25,14 +27,15 @@
 from tpdk.models.persona_collection_read import PersonaCollectionRead
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_write import PersonaWrite
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class PersonaApi(object):
@@ -44,34 +47,30 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def api_personas_get_collection(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, first_name : Optional[StrictStr] = None, last_name : Optional[StrictStr] = None, date_of_birth : Optional[StrictStr] = None, date_of_birth2 : Optional[StrictStr] = None, email : Optional[StrictStr] = None, mobile_phone_number : Optional[StrictStr] = None, mobile_phone_number2 : Optional[conlist(StrictStr)] = None, gender : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of gender")] = None, order_created_at : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs) -> List[PersonaCollectionRead]:  # noqa: E501
+    def api_personas_get_collection(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, first_name : Optional[StrictStr] = None, last_name : Optional[StrictStr] = None, email : Optional[StrictStr] = None, mobile_phone_number : Optional[StrictStr] = None, mobile_phone_number2 : Optional[conlist(StrictStr)] = None, gender : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of gender")] = None, order_created_at : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, date_of_birth_before : Optional[StrictStr] = None, date_of_birth_strictly_before : Optional[StrictStr] = None, date_of_birth_after : Optional[StrictStr] = None, date_of_birth_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs) -> List[PersonaCollectionRead]:  # noqa: E501
         """Retrieves the collection of Persona resources.  # noqa: E501
 
         Retrieves the collection of Persona resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personas_get_collection(page, first_name, last_name, date_of_birth, date_of_birth2, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, async_req=True)
+        >>> thread = api.api_personas_get_collection(page, first_name, last_name, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, date_of_birth_before, date_of_birth_strictly_before, date_of_birth_after, date_of_birth_strictly_after, metadata, async_req=True)
         >>> result = thread.get()
 
         :param page: The collection page number
         :type page: int
         :param first_name: 
         :type first_name: str
         :param last_name: 
         :type last_name: str
-        :param date_of_birth: 
-        :type date_of_birth: str
-        :param date_of_birth2: 
-        :type date_of_birth2: str
         :param email: 
         :type email: str
         :param mobile_phone_number: 
         :type mobile_phone_number: str
         :param mobile_phone_number2: 
         :type mobile_phone_number2: List[str]
         :param gender: Filter on a limited subset of gender
@@ -82,55 +81,57 @@
         :type created_at_before: str
         :param created_at_strictly_before: 
         :type created_at_strictly_before: str
         :param created_at_after: 
         :type created_at_after: str
         :param created_at_strictly_after: 
         :type created_at_strictly_after: str
+        :param date_of_birth_before: 
+        :type date_of_birth_before: str
+        :param date_of_birth_strictly_before: 
+        :type date_of_birth_strictly_before: str
+        :param date_of_birth_after: 
+        :type date_of_birth_after: str
+        :param date_of_birth_strictly_after: 
+        :type date_of_birth_strictly_after: str
         :param metadata: Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type metadata: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[PersonaCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
-        return self.api_personas_get_collection_with_http_info(page, first_name, last_name, date_of_birth, date_of_birth2, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, **kwargs)  # noqa: E501
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.api_personas_get_collection_with_http_info(page, first_name, last_name, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, date_of_birth_before, date_of_birth_strictly_before, date_of_birth_after, date_of_birth_strictly_after, metadata, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, first_name : Optional[StrictStr] = None, last_name : Optional[StrictStr] = None, date_of_birth : Optional[StrictStr] = None, date_of_birth2 : Optional[StrictStr] = None, email : Optional[StrictStr] = None, mobile_phone_number : Optional[StrictStr] = None, mobile_phone_number2 : Optional[conlist(StrictStr)] = None, gender : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of gender")] = None, order_created_at : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs):  # noqa: E501
+    def api_personas_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, first_name : Optional[StrictStr] = None, last_name : Optional[StrictStr] = None, email : Optional[StrictStr] = None, mobile_phone_number : Optional[StrictStr] = None, mobile_phone_number2 : Optional[conlist(StrictStr)] = None, gender : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of gender")] = None, order_created_at : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, date_of_birth_before : Optional[StrictStr] = None, date_of_birth_strictly_before : Optional[StrictStr] = None, date_of_birth_after : Optional[StrictStr] = None, date_of_birth_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of Persona resources.  # noqa: E501
 
         Retrieves the collection of Persona resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personas_get_collection_with_http_info(page, first_name, last_name, date_of_birth, date_of_birth2, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, async_req=True)
+        >>> thread = api.api_personas_get_collection_with_http_info(page, first_name, last_name, email, mobile_phone_number, mobile_phone_number2, gender, order_created_at, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, date_of_birth_before, date_of_birth_strictly_before, date_of_birth_after, date_of_birth_strictly_after, metadata, async_req=True)
         >>> result = thread.get()
 
         :param page: The collection page number
         :type page: int
         :param first_name: 
         :type first_name: str
         :param last_name: 
         :type last_name: str
-        :param date_of_birth: 
-        :type date_of_birth: str
-        :param date_of_birth2: 
-        :type date_of_birth2: str
         :param email: 
         :type email: str
         :param mobile_phone_number: 
         :type mobile_phone_number: str
         :param mobile_phone_number2: 
         :type mobile_phone_number2: List[str]
         :param gender: Filter on a limited subset of gender
@@ -141,25 +142,34 @@
         :type created_at_before: str
         :param created_at_strictly_before: 
         :type created_at_strictly_before: str
         :param created_at_after: 
         :type created_at_after: str
         :param created_at_strictly_after: 
         :type created_at_strictly_after: str
+        :param date_of_birth_before: 
+        :type date_of_birth_before: str
+        :param date_of_birth_strictly_before: 
+        :type date_of_birth_strictly_before: str
+        :param date_of_birth_after: 
+        :type date_of_birth_after: str
+        :param date_of_birth_strictly_after: 
+        :type date_of_birth_strictly_after: str
         :param metadata: Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type metadata: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -173,25 +183,27 @@
 
         _params = locals()
 
         _all_params = [
             'page',
             'first_name',
             'last_name',
-            'date_of_birth',
-            'date_of_birth2',
             'email',
             'mobile_phone_number',
             'mobile_phone_number2',
             'gender',
             'order_created_at',
             'created_at_before',
             'created_at_strictly_before',
             'created_at_after',
             'created_at_strictly_after',
+            'date_of_birth_before',
+            'date_of_birth_strictly_before',
+            'date_of_birth_after',
+            'date_of_birth_strictly_after',
             'metadata'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -224,48 +236,54 @@
 
         if _params.get('first_name') is not None:  # noqa: E501
             _query_params.append(('firstName', _params['first_name']))
 
         if _params.get('last_name') is not None:  # noqa: E501
             _query_params.append(('lastName', _params['last_name']))
 
-        if _params.get('date_of_birth') is not None:  # noqa: E501
-            _query_params.append(('dateOfBirth', _params['date_of_birth']))
-
-        if _params.get('date_of_birth2') is not None:  # noqa: E501
-            _query_params.append(('dateOfBirth[]', _params['date_of_birth2']))
-
         if _params.get('email') is not None:  # noqa: E501
             _query_params.append(('email', _params['email']))
 
         if _params.get('mobile_phone_number') is not None:  # noqa: E501
             _query_params.append(('mobilePhoneNumber', _params['mobile_phone_number']))
 
         if _params.get('mobile_phone_number2') is not None:  # noqa: E501
             _query_params.append(('mobilePhoneNumber[]', _params['mobile_phone_number2']))
             _collection_formats['mobilePhoneNumber[]'] = 'multi'
 
         if _params.get('gender') is not None:  # noqa: E501
-            _query_params.append(('gender', _params['gender']))
+            _query_params.append(('gender', _params['gender'].value))
 
         if _params.get('order_created_at') is not None:  # noqa: E501
-            _query_params.append(('order[createdAt]', _params['order_created_at']))
+            _query_params.append(('order[createdAt]', _params['order_created_at'].value))
 
         if _params.get('created_at_before') is not None:  # noqa: E501
             _query_params.append(('createdAt[before]', _params['created_at_before']))
 
         if _params.get('created_at_strictly_before') is not None:  # noqa: E501
             _query_params.append(('createdAt[strictly_before]', _params['created_at_strictly_before']))
 
         if _params.get('created_at_after') is not None:  # noqa: E501
             _query_params.append(('createdAt[after]', _params['created_at_after']))
 
         if _params.get('created_at_strictly_after') is not None:  # noqa: E501
             _query_params.append(('createdAt[strictly_after]', _params['created_at_strictly_after']))
 
+        if _params.get('date_of_birth_before') is not None:  # noqa: E501
+            _query_params.append(('dateOfBirth[before]', _params['date_of_birth_before']))
+
+        if _params.get('date_of_birth_strictly_before') is not None:  # noqa: E501
+            _query_params.append(('dateOfBirth[strictly_before]', _params['date_of_birth_strictly_before']))
+
+        if _params.get('date_of_birth_after') is not None:  # noqa: E501
+            _query_params.append(('dateOfBirth[after]', _params['date_of_birth_after']))
+
+        if _params.get('date_of_birth_strictly_after') is not None:  # noqa: E501
+            _query_params.append(('dateOfBirth[strictly_after]', _params['date_of_birth_strictly_after']))
+
         if _params.get('metadata') is not None:  # noqa: E501
             _query_params.append(('metadata[]', _params['metadata']))
             _collection_formats['metadata[]'] = 'csv'
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -274,15 +292,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[PersonaCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/personas', 'GET',
@@ -312,52 +330,51 @@
         >>> thread = api.api_personas_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_id_delete_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_id_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs):  # noqa: E501
+    def api_personas_id_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Unregister a Persona (Your customer)  # noqa: E501
 
         You **MAY** unregister (or free the email/phone number) your Persona entry using that endpoint. *Please note that* this operation will fail if that Persona have any ongoing operations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -410,15 +427,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/personas/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -446,52 +463,51 @@
         >>> thread = api.api_personas_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_id_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs):  # noqa: E501
+    def api_personas_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves a Persona resource.  # noqa: E501
 
         Retrieves a Persona resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -548,15 +564,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "PersonaRead",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -589,32 +605,30 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param persona_update: The updated Persona resource (required)
         :type persona_update: PersonaUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_id_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_id_patch_with_http_info(id, persona_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_id_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_update : Annotated[PersonaUpdate, Field(..., description="The updated Persona resource")], **kwargs):  # noqa: E501
+    def api_personas_id_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_update : Annotated[PersonaUpdate, Field(..., description="The updated Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Updates the Persona resource.  # noqa: E501
 
         Update your Persona (eg. your customer/user entry) through that API call. _Beware that updating_ **email** and/or the **mobile phone number** must be done using non reserved values. Otherwise this operation will be rejected.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_id_patch_with_http_info(id, persona_update, async_req=True)
@@ -622,21 +636,22 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param persona_update: The updated Persona resource (required)
         :type persona_update: PersonaUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -689,36 +704,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_update']:
+        if _params['persona_update'] is not None:
             _body_params = _params['persona_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "PersonaRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/personas/{id}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -747,32 +762,30 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param persona_write: The new Persona resource (required)
         :type persona_write: PersonaWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaPostAuthRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idtoken_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idtoken_post_with_http_info(id, persona_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idtoken_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs):  # noqa: E501
+    def api_personas_idtoken_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Issue authenticated URL for single end-user  # noqa: E501
 
         Without this, your users may be required to pass a MFA challenge even if they are already logged-in from your website. Pass the URL you wish your user access, either a Dispute or Safe-checkout resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idtoken_post_with_http_info(id, persona_write, async_req=True)
@@ -780,21 +793,22 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param persona_write: The new Persona resource (required)
         :type persona_write: PersonaWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -847,15 +861,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_write']:
+        if _params['persona_write'] is not None:
             _body_params = _params['persona_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -865,17 +879,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "PersonaPostAuthRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/personas/{id}/token', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -902,52 +916,51 @@
         >>> thread = api.api_personas_post(persona_write, async_req=True)
         >>> result = thread.get()
 
         :param persona_write: The new Persona resource (required)
         :type persona_write: PersonaWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_post_with_http_info(persona_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_post_with_http_info(self, persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs):  # noqa: E501
+    def api_personas_post_with_http_info(self, persona_write : Annotated[PersonaWrite, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Register a Persona (Your customer)  # noqa: E501
 
         You should not register your whole database of users, only those who are concerned by a Safe-checkout or Dispute operation. One Persona entry for your organization can be assigned as a seller or buyer.  **Notes:**   - (i) There is a unique constraint for the mobile phone numbers and email.   - (ii) You will have to issue a DELETE operation on a Persona that withhold a specific phone number or email.   - (iii) You are NOT REQUIRED to provide email OR a mobile phone number but it is highly recommended, if none provided the email will be generated as '{ulid}@your-domain.tld'. In that case, please specify at least one metadata in order to find your entry with ease.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_post_with_http_info(persona_write, async_req=True)
         >>> result = thread.get()
 
         :param persona_write: The new Persona resource (required)
         :type persona_write: PersonaWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -996,15 +1009,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_write']:
+        if _params['persona_write'] is not None:
             _body_params = _params['persona_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -1014,17 +1027,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "PersonaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/personas', 'POST',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/resolution_center_api.py` & `tpdk-2.0.7/tpdk/api/resolution_center_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictInt, StrictStr, conlist
+from pydantic import Field, StrictBool, StrictBytes, StrictInt, StrictStr, conlist
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from tpdk.models.dispute_collection_read import DisputeCollectionRead
 from tpdk.models.dispute_independent_write import DisputeIndependentWrite
 from tpdk.models.dispute_post_creation_read import DisputePostCreationRead
 from tpdk.models.dispute_read import DisputeRead
 from tpdk.models.dispute_update import DisputeUpdate
 from tpdk.models.evaluation_read import EvaluationRead
@@ -32,14 +34,15 @@
 from tpdk.models.evidence_read import EvidenceRead
 from tpdk.models.evidence_write import EvidenceWrite
 from tpdk.models.media_read import MediaRead
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class ResolutionCenterApi(object):
@@ -99,32 +102,30 @@
         :type metadata: List[str]
         :param transaction_metadata: Flattened OrderedMap for transaction.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type transaction_metadata: List[str]
         :param transaction_offer_metadata: Flattened OrderedMap for transaction.offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type transaction_offer_metadata: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DisputeCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_get_collection_with_http_info(page, order_created_at, order_status, order_updated_at, transaction_offer_title, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, status, transaction_status, exists_recommended_solution, exists_chosen_solution, exists_counter_solution, exists_platform_solution, metadata, transaction_metadata, transaction_offer_metadata, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_created_at : Optional[StrictStr] = None, order_status : Optional[StrictStr] = None, order_updated_at : Optional[StrictStr] = None, transaction_offer_title : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, transaction_status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of transaction.status")] = None, exists_recommended_solution : Optional[StrictBool] = None, exists_chosen_solution : Optional[StrictBool] = None, exists_counter_solution : Optional[StrictBool] = None, exists_platform_solution : Optional[StrictBool] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, transaction_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for transaction.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, transaction_offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for transaction.offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs):  # noqa: E501
+    def api_disputes_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_created_at : Optional[StrictStr] = None, order_status : Optional[StrictStr] = None, order_updated_at : Optional[StrictStr] = None, transaction_offer_title : Optional[StrictStr] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, transaction_status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of transaction.status")] = None, exists_recommended_solution : Optional[StrictBool] = None, exists_chosen_solution : Optional[StrictBool] = None, exists_counter_solution : Optional[StrictBool] = None, exists_platform_solution : Optional[StrictBool] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, transaction_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for transaction.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, transaction_offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for transaction.offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of Dispute resources.  # noqa: E501
 
         Retrieves the collection of Dispute resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_get_collection_with_http_info(page, order_created_at, order_status, order_updated_at, transaction_offer_title, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, status, transaction_status, exists_recommended_solution, exists_chosen_solution, exists_counter_solution, exists_platform_solution, metadata, transaction_metadata, transaction_offer_metadata, async_req=True)
@@ -164,21 +165,22 @@
         :type metadata: List[str]
         :param transaction_metadata: Flattened OrderedMap for transaction.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type transaction_metadata: List[str]
         :param transaction_offer_metadata: Flattened OrderedMap for transaction.offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
         :type transaction_offer_metadata: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -241,21 +243,21 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('order_created_at') is not None:  # noqa: E501
-            _query_params.append(('order[createdAt]', _params['order_created_at']))
+            _query_params.append(('order[createdAt]', _params['order_created_at'].value))
 
         if _params.get('order_status') is not None:  # noqa: E501
-            _query_params.append(('order[status]', _params['order_status']))
+            _query_params.append(('order[status]', _params['order_status'].value))
 
         if _params.get('order_updated_at') is not None:  # noqa: E501
-            _query_params.append(('order[updatedAt]', _params['order_updated_at']))
+            _query_params.append(('order[updatedAt]', _params['order_updated_at'].value))
 
         if _params.get('transaction_offer_title') is not None:  # noqa: E501
             _query_params.append(('transaction.offer.title', _params['transaction_offer_title']))
 
         if _params.get('created_at_before') is not None:  # noqa: E501
             _query_params.append(('createdAt[before]', _params['created_at_before']))
 
@@ -265,18 +267,18 @@
         if _params.get('created_at_after') is not None:  # noqa: E501
             _query_params.append(('createdAt[after]', _params['created_at_after']))
 
         if _params.get('created_at_strictly_after') is not None:  # noqa: E501
             _query_params.append(('createdAt[strictly_after]', _params['created_at_strictly_after']))
 
         if _params.get('status') is not None:  # noqa: E501
-            _query_params.append(('status', _params['status']))
+            _query_params.append(('status', _params['status'].value))
 
         if _params.get('transaction_status') is not None:  # noqa: E501
-            _query_params.append(('transaction.status', _params['transaction_status']))
+            _query_params.append(('transaction.status', _params['transaction_status'].value))
 
         if _params.get('exists_recommended_solution') is not None:  # noqa: E501
             _query_params.append(('exists[recommendedSolution]', _params['exists_recommended_solution']))
 
         if _params.get('exists_chosen_solution') is not None:  # noqa: E501
             _query_params.append(('exists[chosenSolution]', _params['exists_chosen_solution']))
 
@@ -306,15 +308,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[DisputeCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/disputes', 'GET',
@@ -344,52 +346,51 @@
         >>> thread = api.api_disputes_post(dispute_independent_write, async_req=True)
         >>> result = thread.get()
 
         :param dispute_independent_write: The new Dispute resource (required)
         :type dispute_independent_write: DisputeIndependentWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputePostCreationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_post_with_http_info(dispute_independent_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_post_with_http_info(self, dispute_independent_write : Annotated[DisputeIndependentWrite, Field(..., description="The new Dispute resource")], **kwargs):  # noqa: E501
+    def api_disputes_post_with_http_info(self, dispute_independent_write : Annotated[DisputeIndependentWrite, Field(..., description="The new Dispute resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Draft a standalone Dispute  # noqa: E501
 
         Create a draft dispute to be filled by an alleged aggrieved customer. Do not use that endpoint if the transaction took place using our safe-checkout tunnel. This endpoint return a unique URL that can be accessed by both the complainant and seller (if individual).  **Note:** You can generate at your own discretion tokens for both parties, thus avoiding the secondary authentication.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_post_with_http_info(dispute_independent_write, async_req=True)
         >>> result = thread.get()
 
         :param dispute_independent_write: The new Dispute resource (required)
         :type dispute_independent_write: DisputeIndependentWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -438,15 +439,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['dispute_independent_write']:
+        if _params['dispute_independent_write'] is not None:
             _body_params = _params['dispute_independent_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -456,17 +457,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "DisputePostCreationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/disputes', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -493,52 +494,51 @@
         >>> thread = api.api_disputes_ulid_delete(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulid_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulid_delete_with_http_info(ulid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulid_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], **kwargs):  # noqa: E501
+    def api_disputes_ulid_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Abandon claims on Dispute  # noqa: E501
 
         **Only the buyer/complainant** can dismiss the case immediately. Otherwise, the support can but in a limited ranges of Dispute status.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulid_delete_with_http_info(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -591,15 +591,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/disputes/{ulid}', 'DELETE',
             _path_params,
             _query_params,
@@ -627,52 +627,51 @@
         >>> thread = api.api_disputes_ulid_get(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputeRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulid_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulid_get_with_http_info(ulid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulid_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], **kwargs):  # noqa: E501
+    def api_disputes_ulid_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves a Dispute resource.  # noqa: E501
 
         Retrieves a Dispute resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulid_get_with_http_info(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -729,15 +728,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "DisputeRead",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -755,69 +754,68 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def api_disputes_ulid_patch(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], dispute_update : Annotated[DisputeUpdate, Field(..., description="The updated Dispute resource")], **kwargs) -> DisputeRead:  # noqa: E501
-        """Updates the Dispute resource.  # noqa: E501
+        """Update the Dispute  # noqa: E501
 
         Updates the Dispute resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulid_patch(ulid, dispute_update, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param dispute_update: The updated Dispute resource (required)
         :type dispute_update: DisputeUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputeRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulid_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulid_patch_with_http_info(ulid, dispute_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulid_patch_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], dispute_update : Annotated[DisputeUpdate, Field(..., description="The updated Dispute resource")], **kwargs):  # noqa: E501
-        """Updates the Dispute resource.  # noqa: E501
+    def api_disputes_ulid_patch_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], dispute_update : Annotated[DisputeUpdate, Field(..., description="The updated Dispute resource")], **kwargs) -> ApiResponse:  # noqa: E501
+        """Update the Dispute  # noqa: E501
 
         Updates the Dispute resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulid_patch_with_http_info(ulid, dispute_update, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param dispute_update: The updated Dispute resource (required)
         :type dispute_update: DisputeUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -870,15 +868,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['dispute_update']:
+        if _params['dispute_update'] is not None:
             _body_params = _params['dispute_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -890,16 +888,16 @@
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "DisputeRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/disputes/{ulid}', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -928,32 +926,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param evaluation_write: The new Evaluation resource (required)
         :type evaluation_write: EvaluationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EvaluationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidevaluations_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidevaluations_post_with_http_info(ulid, evaluation_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidevaluations_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], evaluation_write : Annotated[EvaluationWrite, Field(..., description="The new Evaluation resource")], **kwargs):  # noqa: E501
+    def api_disputes_ulidevaluations_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], evaluation_write : Annotated[EvaluationWrite, Field(..., description="The new Evaluation resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Submit an Evaluation for the Dispute  # noqa: E501
 
         **Only authenticated** complainant and seller **CAN** issue an evaluation **WHEN** the dispute reached a final state.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevaluations_post_with_http_info(ulid, evaluation_write, async_req=True)
@@ -961,21 +957,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param evaluation_write: The new Evaluation resource (required)
         :type evaluation_write: EvaluationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1028,35 +1025,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['evaluation_write']:
+        if _params['evaluation_write'] is not None:
             _body_params = _params['evaluation_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "EvaluationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/disputes/{ulid}/evaluations', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -1085,32 +1082,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[EvidenceRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidevidences_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidevidences_get_collection_with_http_info(ulid, page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidevidences_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
+    def api_disputes_ulidevidences_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieve all Evidences in Dispute  # noqa: E501
 
         Retrieves the collection of Evidence resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevidences_get_collection_with_http_info(ulid, page, async_req=True)
@@ -1118,21 +1113,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1193,15 +1189,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey']  # noqa: E501
 
         _response_types_map = {
             '200': "List[EvidenceRead]",
         }
 
         return self.api_client.call_api(
             '/disputes/{ulid}/evidences', 'GET',
@@ -1233,32 +1229,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param id: Evidence identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidevidences_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidevidences_id_delete_with_http_info(ulid, id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidevidences_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], **kwargs):  # noqa: E501
+    def api_disputes_ulidevidences_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Withdraw an Evidence from a Dispute  # noqa: E501
 
         Removes the Evidence resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevidences_id_delete_with_http_info(ulid, id, async_req=True)
@@ -1266,21 +1260,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param id: Evidence identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1337,15 +1332,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/disputes/{ulid}/evidences/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -1359,15 +1354,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_disputes_ulidevidences_idmedia_post(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], file : Optional[StrictStr] = None, **kwargs) -> MediaRead:  # noqa: E501
+    def api_disputes_ulidevidences_idmedia_post(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> MediaRead:  # noqa: E501
         """Upload attachment in regard of described Evidence  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevidences_idmedia_post(ulid, id, file, async_req=True)
@@ -1377,32 +1372,30 @@
         :type ulid: str
         :param id: Evidence identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MediaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidevidences_idmedia_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidevidences_idmedia_post_with_http_info(ulid, id, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidevidences_idmedia_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], file : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def api_disputes_ulidevidences_idmedia_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Evidence identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Upload attachment in regard of described Evidence  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevidences_idmedia_post_with_http_info(ulid, id, file, async_req=True)
@@ -1412,21 +1405,22 @@
         :type ulid: str
         :param id: Evidence identifier (required)
         :type id: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1498,20 +1492,20 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "MediaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/disputes/{ulid}/evidences/{id}/media', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -1540,32 +1534,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param evidence_write: The new Evidence resource (required)
         :type evidence_write: EvidenceWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EvidenceRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidevidences_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidevidences_post_with_http_info(ulid, evidence_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidevidences_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], evidence_write : Annotated[EvidenceWrite, Field(..., description="The new Evidence resource")], **kwargs):  # noqa: E501
+    def api_disputes_ulidevidences_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], evidence_write : Annotated[EvidenceWrite, Field(..., description="The new Evidence resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Submit an Evidence to the Dispute case  # noqa: E501
 
         This action does not held the actual upload, you will have to do the upload in a dedicated request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidevidences_post_with_http_info(ulid, evidence_write, async_req=True)
@@ -1573,21 +1565,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param evidence_write: The new Evidence resource (required)
         :type evidence_write: EvidenceWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1640,35 +1633,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['evidence_write']:
+        if _params['evidence_write'] is not None:
             _body_params = _params['evidence_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "EvidenceRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/disputes/{ulid}/evidences', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -1697,32 +1690,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[object]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidparcels_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidparcels_get_collection_with_http_info(ulid, page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidparcels_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
+    def api_disputes_ulidparcels_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of Parcel resources.  # noqa: E501
 
         Retrieves the collection of Parcel resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidparcels_get_collection_with_http_info(ulid, page, async_req=True)
@@ -1730,21 +1721,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1845,32 +1837,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param id: Parcel identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidparcels_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidparcels_id_delete_with_http_info(ulid, id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidparcels_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Parcel identifier")], **kwargs):  # noqa: E501
+    def api_disputes_ulidparcels_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Parcel identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Removes the Parcel resource.  # noqa: E501
 
         Removes the Parcel resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidparcels_id_delete_with_http_info(ulid, id, async_req=True)
@@ -1878,21 +1868,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param id: Parcel identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1949,15 +1940,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/disputes/{ulid}/parcels/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -1987,32 +1978,30 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param parcel_write: The new Parcel resource (required)
         :type parcel_write: ParcelWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ParcelRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_disputes_ulidparcels_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_disputes_ulidparcels_post_with_http_info(ulid, parcel_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_disputes_ulidparcels_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], parcel_write : Annotated[ParcelWrite, Field(..., description="The new Parcel resource")], **kwargs):  # noqa: E501
+    def api_disputes_ulidparcels_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], parcel_write : Annotated[ParcelWrite, Field(..., description="The new Parcel resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Creates a Parcel resource.  # noqa: E501
 
         Creates a Parcel resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_disputes_ulidparcels_post_with_http_info(ulid, parcel_write, async_req=True)
@@ -2020,21 +2009,22 @@
 
         :param ulid: Dispute identifier (required)
         :type ulid: str
         :param parcel_write: The new Parcel resource (required)
         :type parcel_write: ParcelWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2087,15 +2077,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['parcel_write']:
+        if _params['parcel_write'] is not None:
             _body_params = _params['parcel_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -2128,15 +2118,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_offers_ulidmedias_post(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[StrictStr] = None, **kwargs) -> MediaRead:  # noqa: E501
+    def api_offers_ulidmedias_post(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> MediaRead:  # noqa: E501
         """Upload a picture for a given Offer  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidmedias_post(ulid, file, async_req=True)
@@ -2144,32 +2134,30 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MediaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidmedias_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidmedias_post_with_http_info(ulid, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidmedias_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def api_offers_ulidmedias_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Upload a picture for a given Offer  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidmedias_post_with_http_info(ulid, file, async_req=True)
@@ -2177,21 +2165,22 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2259,20 +2248,20 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "MediaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/offers/{ulid}/medias', 'POST',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/safe_checkout_api.py` & `tpdk-2.0.7/tpdk/api/safe_checkout_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist
+from pydantic import Field, StrictBool, StrictBytes, StrictFloat, StrictInt, StrictStr, conlist
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from tpdk.models.dispute_post_creation_read import DisputePostCreationRead
 from tpdk.models.dispute_read import DisputeRead
 from tpdk.models.dispute_update import DisputeUpdate
 from tpdk.models.dispute_write import DisputeWrite
 from tpdk.models.evaluation_read import EvaluationRead
 from tpdk.models.evaluation_write import EvaluationWrite
@@ -37,14 +39,15 @@
 from tpdk.models.offer_write import OfferWrite
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 from tpdk.models.transaction_collection_read import TransactionCollectionRead
 from tpdk.models.transaction_read import TransactionRead
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class SafeCheckoutApi(object):
@@ -56,15 +59,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def api_offers_get_collection(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[StrictFloat] = None, unit_price2 : Optional[conlist(StrictFloat)] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> List[OfferCollectionRead]:  # noqa: E501
+    def api_offers_get_collection(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[Union[StrictFloat, StrictInt]] = None, unit_price2 : Optional[conlist(Union[StrictFloat, StrictInt])] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> List[OfferCollectionRead]:  # noqa: E501
         """Read issued Offers  # noqa: E501
 
         Retrieves the collection of Offer resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_get_collection(page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, async_req=True)
@@ -102,32 +105,30 @@
         :type nature: str
         :param condition: Filter on a limited subset of condition
         :type condition: str
         :param shipping_allowed: 
         :type shipping_allowed: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[OfferCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_get_collection_with_http_info(page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[StrictFloat] = None, unit_price2 : Optional[conlist(StrictFloat)] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def api_offers_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[Union[StrictFloat, StrictInt]] = None, unit_price2 : Optional[conlist(Union[StrictFloat, StrictInt])] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Read issued Offers  # noqa: E501
 
         Retrieves the collection of Offer resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_get_collection_with_http_info(page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, async_req=True)
@@ -165,21 +166,22 @@
         :type nature: str
         :param condition: Filter on a limited subset of condition
         :type condition: str
         :param shipping_allowed: 
         :type shipping_allowed: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -285,18 +287,18 @@
             _collection_formats['metadata[]'] = 'csv'
 
         if _params.get('offer_metadata') is not None:  # noqa: E501
             _query_params.append(('offer.metadata[]', _params['offer_metadata']))
             _collection_formats['offer.metadata[]'] = 'csv'
 
         if _params.get('nature') is not None:  # noqa: E501
-            _query_params.append(('nature', _params['nature']))
+            _query_params.append(('nature', _params['nature'].value))
 
         if _params.get('condition') is not None:  # noqa: E501
-            _query_params.append(('condition', _params['condition']))
+            _query_params.append(('condition', _params['condition'].value))
 
         if _params.get('shipping_allowed') is not None:  # noqa: E501
             _query_params.append(('shippingAllowed', _params['shipping_allowed']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -305,15 +307,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[OfferCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/offers', 'GET',
@@ -343,52 +345,51 @@
         >>> thread = api.api_offers_post(offer_independent_write, async_req=True)
         >>> result = thread.get()
 
         :param offer_independent_write: The new Offer resource (required)
         :type offer_independent_write: OfferIndependentWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: OfferPostCreationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_post_with_http_info(offer_independent_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_post_with_http_info(self, offer_independent_write : Annotated[OfferIndependentWrite, Field(..., description="The new Offer resource")], **kwargs):  # noqa: E501
+    def api_offers_post_with_http_info(self, offer_independent_write : Annotated[OfferIndependentWrite, Field(..., description="The new Offer resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Create an Offer and retrieve url  # noqa: E501
 
         Publish an offer so that you can safely retrieve a safe-checkout unique link from us  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_post_with_http_info(offer_independent_write, async_req=True)
         >>> result = thread.get()
 
         :param offer_independent_write: The new Offer resource (required)
         :type offer_independent_write: OfferIndependentWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -437,35 +438,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['offer_independent_write']:
+        if _params['offer_independent_write'] is not None:
             _body_params = _params['offer_independent_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "OfferPostCreationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/offers', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -492,52 +493,51 @@
         >>> thread = api.api_offers_ulid_get(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: OfferRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulid_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulid_get_with_http_info(ulid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulid_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], **kwargs):  # noqa: E501
+    def api_offers_ulid_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Read an Offer  # noqa: E501
 
         Retrieves a Offer resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulid_get_with_http_info(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -594,15 +594,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "OfferRead",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -635,32 +635,30 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param id: Media identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidmedias_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidmedias_id_delete_with_http_info(ulid, id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidmedias_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], id : Annotated[StrictStr, Field(..., description="Media identifier")], **kwargs):  # noqa: E501
+    def api_offers_ulidmedias_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], id : Annotated[StrictStr, Field(..., description="Media identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Removes the Media resource.  # noqa: E501
 
         Removes the Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidmedias_id_delete_with_http_info(ulid, id, async_req=True)
@@ -668,21 +666,22 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param id: Media identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -739,15 +738,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/offers/{ulid}/medias/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -761,15 +760,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_offers_ulidmedias_post(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[StrictStr] = None, **kwargs) -> MediaRead:  # noqa: E501
+    def api_offers_ulidmedias_post(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> MediaRead:  # noqa: E501
         """Upload a picture for a given Offer  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidmedias_post(ulid, file, async_req=True)
@@ -777,32 +776,30 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MediaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidmedias_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidmedias_post_with_http_info(ulid, file, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidmedias_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def api_offers_ulidmedias_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], file : Optional[Union[StrictBytes, StrictStr]] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Upload a picture for a given Offer  # noqa: E501
 
         Creates a Media resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidmedias_post_with_http_info(ulid, file, async_req=True)
@@ -810,21 +807,22 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param file:
         :type file: bytearray
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -892,20 +890,20 @@
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "MediaRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/offers/{ulid}/medias', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -942,32 +940,30 @@
         :type metadata: List[str]
         :param status: Filter on a limited subset of status
         :type status: str
         :param exists_dispute: 
         :type exists_dispute: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[TransactionCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidtransactions_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidtransactions_get_collection_with_http_info(ulid, page, order_status, metadata, status, exists_dispute, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidtransactions_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_status : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, exists_dispute : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def api_offers_ulidtransactions_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_status : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, exists_dispute : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieve Payment Intents for Offer  # noqa: E501
 
         Retrieves the collection of Transaction resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidtransactions_get_collection_with_http_info(ulid, page, order_status, metadata, status, exists_dispute, async_req=True)
@@ -983,21 +979,22 @@
         :type metadata: List[str]
         :param status: Filter on a limited subset of status
         :type status: str
         :param exists_dispute: 
         :type exists_dispute: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1051,22 +1048,22 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('order_status') is not None:  # noqa: E501
-            _query_params.append(('order[status]', _params['order_status']))
+            _query_params.append(('order[status]', _params['order_status'].value))
 
         if _params.get('metadata') is not None:  # noqa: E501
             _query_params.append(('metadata[]', _params['metadata']))
             _collection_formats['metadata[]'] = 'csv'
 
         if _params.get('status') is not None:  # noqa: E501
-            _query_params.append(('status', _params['status']))
+            _query_params.append(('status', _params['status'].value))
 
         if _params.get('exists_dispute') is not None:  # noqa: E501
             _query_params.append(('exists[dispute]', _params['exists_dispute']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -1075,15 +1072,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[TransactionCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/offers/{ulid}/transactions', 'GET',
@@ -1117,32 +1114,30 @@
         :type ulid: str
         :param id: Transaction identifier (required)
         :type id: str
         :param evaluation_write: The new Evaluation resource (required)
         :type evaluation_write: EvaluationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EvaluationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidtransactions_idevaluations_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidtransactions_idevaluations_post_with_http_info(ulid, id, evaluation_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidtransactions_idevaluations_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Transaction identifier")], evaluation_write : Annotated[EvaluationWrite, Field(..., description="The new Evaluation resource")], **kwargs):  # noqa: E501
+    def api_offers_ulidtransactions_idevaluations_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Dispute identifier")], id : Annotated[StrictStr, Field(..., description="Transaction identifier")], evaluation_write : Annotated[EvaluationWrite, Field(..., description="The new Evaluation resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Submit an Evaluation for the Offer  # noqa: E501
 
         **Only authenticated** buyer and seller **CAN** issue an evaluation **WHEN** the transaction reached a final state.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidtransactions_idevaluations_post_with_http_info(ulid, id, evaluation_write, async_req=True)
@@ -1152,21 +1147,22 @@
         :type ulid: str
         :param id: Transaction identifier (required)
         :type id: str
         :param evaluation_write: The new Evaluation resource (required)
         :type evaluation_write: EvaluationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1223,35 +1219,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['evaluation_write']:
+        if _params['evaluation_write'] is not None:
             _body_params = _params['evaluation_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "EvaluationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/offers/{ulid}/transactions/{id}/evaluations', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -1280,32 +1276,30 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param body: The new Transaction resource (required)
         :type body: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: TransactionRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_offers_ulidtransactions_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_offers_ulidtransactions_post_with_http_info(ulid, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_offers_ulidtransactions_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], body : Annotated[Dict[str, Any], Field(..., description="The new Transaction resource")], **kwargs):  # noqa: E501
+    def api_offers_ulidtransactions_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Offer identifier")], body : Annotated[Dict[str, Any], Field(..., description="The new Transaction resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Create a Payment Intent for Offer  # noqa: E501
 
         Cannot be used outside of a Persona (buyer)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_offers_ulidtransactions_post_with_http_info(ulid, body, async_req=True)
@@ -1313,21 +1307,22 @@
 
         :param ulid: Offer identifier (required)
         :type ulid: str
         :param body: The new Transaction resource (required)
         :type body: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1380,35 +1375,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['body']:
+        if _params['body'] is not None:
             _body_params = _params['body']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['personaAuthKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "TransactionRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/offers/{ulid}/transactions', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -1435,52 +1430,51 @@
         >>> thread = api.api_personas_idoffers_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idoffers_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idoffers_delete_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idoffers_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs):  # noqa: E501
+    def api_personas_idoffers_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Revoke an Offer for given Persona  # noqa: E501
 
         That goes without says, if that **Offer** have a _Transaction_ **that is ongoing**, you **MAY NOT** revoke the **Offer**.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idoffers_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: Persona identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1533,15 +1527,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/personas/{id}/offers', 'DELETE',
             _path_params,
             _query_params,
@@ -1555,15 +1549,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def api_personas_idoffers_get_collection(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[StrictFloat] = None, unit_price2 : Optional[conlist(StrictFloat)] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> List[OfferCollectionRead]:  # noqa: E501
+    def api_personas_idoffers_get_collection(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[Union[StrictFloat, StrictInt]] = None, unit_price2 : Optional[conlist(Union[StrictFloat, StrictInt])] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> List[OfferCollectionRead]:  # noqa: E501
         """List or Search Offers for given Persona  # noqa: E501
 
         Retrieves the collection of Offer resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idoffers_get_collection(id, page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, async_req=True)
@@ -1603,32 +1597,30 @@
         :type nature: str
         :param condition: Filter on a limited subset of condition
         :type condition: str
         :param shipping_allowed: 
         :type shipping_allowed: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[OfferCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idoffers_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idoffers_get_collection_with_http_info(id, page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idoffers_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[StrictFloat] = None, unit_price2 : Optional[conlist(StrictFloat)] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def api_personas_idoffers_get_collection_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, title : Optional[StrictStr] = None, public_url : Optional[StrictStr] = None, public_url2 : Optional[conlist(StrictStr)] = None, unit_price : Optional[Union[StrictFloat, StrictInt]] = None, unit_price2 : Optional[conlist(Union[StrictFloat, StrictInt])] = None, item_count : Optional[StrictInt] = None, item_count2 : Optional[conlist(StrictInt)] = None, created_at_before : Optional[StrictStr] = None, created_at_strictly_before : Optional[StrictStr] = None, created_at_after : Optional[StrictStr] = None, created_at_strictly_after : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, offer_metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for offer.metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, nature : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of nature")] = None, condition : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of condition")] = None, shipping_allowed : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """List or Search Offers for given Persona  # noqa: E501
 
         Retrieves the collection of Offer resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idoffers_get_collection_with_http_info(id, page, title, public_url, public_url2, unit_price, unit_price2, item_count, item_count2, created_at_before, created_at_strictly_before, created_at_after, created_at_strictly_after, metadata, offer_metadata, nature, condition, shipping_allowed, async_req=True)
@@ -1668,21 +1660,22 @@
         :type nature: str
         :param condition: Filter on a limited subset of condition
         :type condition: str
         :param shipping_allowed: 
         :type shipping_allowed: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1792,18 +1785,18 @@
             _collection_formats['metadata[]'] = 'csv'
 
         if _params.get('offer_metadata') is not None:  # noqa: E501
             _query_params.append(('offer.metadata[]', _params['offer_metadata']))
             _collection_formats['offer.metadata[]'] = 'csv'
 
         if _params.get('nature') is not None:  # noqa: E501
-            _query_params.append(('nature', _params['nature']))
+            _query_params.append(('nature', _params['nature'].value))
 
         if _params.get('condition') is not None:  # noqa: E501
-            _query_params.append(('condition', _params['condition']))
+            _query_params.append(('condition', _params['condition'].value))
 
         if _params.get('shipping_allowed') is not None:  # noqa: E501
             _query_params.append(('shippingAllowed', _params['shipping_allowed']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -1812,15 +1805,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[OfferCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/personas/{id}/offers', 'GET',
@@ -1852,32 +1845,30 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param offer_update: The updated Offer resource (required)
         :type offer_update: OfferUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: OfferRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idoffers_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idoffers_patch_with_http_info(id, offer_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idoffers_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], offer_update : Annotated[OfferUpdate, Field(..., description="The updated Offer resource")], **kwargs):  # noqa: E501
+    def api_personas_idoffers_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], offer_update : Annotated[OfferUpdate, Field(..., description="The updated Offer resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Update an Offer for given Persona  # noqa: E501
 
         Updates the Offer resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idoffers_patch_with_http_info(id, offer_update, async_req=True)
@@ -1885,21 +1876,22 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param offer_update: The updated Offer resource (required)
         :type offer_update: OfferUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1952,36 +1944,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['offer_update']:
+        if _params['offer_update'] is not None:
             _body_params = _params['offer_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "OfferRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/personas/{id}/offers', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -2010,32 +2002,30 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param offer_write: The new Offer resource (required)
         :type offer_write: OfferWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: OfferPostCreationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personas_idoffers_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personas_idoffers_post_with_http_info(id, offer_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personas_idoffers_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], offer_write : Annotated[OfferWrite, Field(..., description="The new Offer resource")], **kwargs):  # noqa: E501
+    def api_personas_idoffers_post_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Persona identifier")], offer_write : Annotated[OfferWrite, Field(..., description="The new Offer resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Create an Offer for given Persona  # noqa: E501
 
         Creates a Offer resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personas_idoffers_post_with_http_info(id, offer_write, async_req=True)
@@ -2043,21 +2033,22 @@
 
         :param id: Persona identifier (required)
         :type id: str
         :param offer_write: The new Offer resource (required)
         :type offer_write: OfferWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2110,35 +2101,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['offer_write']:
+        if _params['offer_write'] is not None:
             _body_params = _params['offer_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "OfferPostCreationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/personas/{id}/offers', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -2151,66 +2142,237 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def api_transactions_get_collection(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_status : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, exists_dispute : Optional[StrictBool] = None, **kwargs) -> List[TransactionCollectionRead]:  # noqa: E501
+        """Retrieves the collection of Transaction resources.  # noqa: E501
+
+        Retrieves the collection of Transaction resources.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_transactions_get_collection(page, order_status, metadata, status, exists_dispute, async_req=True)
+        >>> result = thread.get()
+
+        :param page: The collection page number
+        :type page: int
+        :param order_status: 
+        :type order_status: str
+        :param metadata: Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
+        :type metadata: List[str]
+        :param status: Filter on a limited subset of status
+        :type status: str
+        :param exists_dispute: 
+        :type exists_dispute: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: List[TransactionCollectionRead]
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.api_transactions_get_collection_with_http_info(page, order_status, metadata, status, exists_dispute, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def api_transactions_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, order_status : Optional[StrictStr] = None, metadata : Annotated[Optional[conlist(conlist(StrictStr))], Field(description="Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.")] = None, status : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of status")] = None, exists_dispute : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """Retrieves the collection of Transaction resources.  # noqa: E501
+
+        Retrieves the collection of Transaction resources.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_transactions_get_collection_with_http_info(page, order_status, metadata, status, exists_dispute, async_req=True)
+        >>> result = thread.get()
+
+        :param page: The collection page number
+        :type page: int
+        :param order_status: 
+        :type order_status: str
+        :param metadata: Flattened OrderedMap for metadata. Must be a multiple of two items count. Explicitly set \"null\" for desired value.
+        :type metadata: List[str]
+        :param status: Filter on a limited subset of status
+        :type status: str
+        :param exists_dispute: 
+        :type exists_dispute: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(List[TransactionCollectionRead], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'page',
+            'order_status',
+            'metadata',
+            'status',
+            'exists_dispute'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method api_transactions_get_collection" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('order_status') is not None:  # noqa: E501
+            _query_params.append(('order[status]', _params['order_status'].value))
+
+        if _params.get('metadata') is not None:  # noqa: E501
+            _query_params.append(('metadata[]', _params['metadata']))
+            _collection_formats['metadata[]'] = 'csv'
+
+        if _params.get('status') is not None:  # noqa: E501
+            _query_params.append(('status', _params['status'].value))
+
+        if _params.get('exists_dispute') is not None:  # noqa: E501
+            _query_params.append(('exists[dispute]', _params['exists_dispute']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "List[TransactionCollectionRead]",
+        }
+
+        return self.api_client.call_api(
+            '/transactions', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def api_transactions_uliddispute_delete(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], **kwargs) -> None:  # noqa: E501
         """Abandon claims on Dispute  # noqa: E501
 
         **Only the buyer/complainant** can dismiss the case immediately. Otherwise, the support can but in a limited ranges of Dispute status.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_uliddispute_delete(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_uliddispute_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_uliddispute_delete_with_http_info(ulid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_uliddispute_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], **kwargs):  # noqa: E501
+    def api_transactions_uliddispute_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Abandon claims on Dispute  # noqa: E501
 
         **Only the buyer/complainant** can dismiss the case immediately. Otherwise, the support can but in a limited ranges of Dispute status.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_uliddispute_delete_with_http_info(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2263,15 +2425,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/transactions/{ulid}/dispute', 'DELETE',
             _path_params,
             _query_params,
@@ -2299,52 +2461,51 @@
         >>> thread = api.api_transactions_uliddispute_get(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputeRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_uliddispute_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_uliddispute_get_with_http_info(ulid, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_uliddispute_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], **kwargs):  # noqa: E501
+    def api_transactions_uliddispute_get_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Read Dispute from existing Transaction  # noqa: E501
 
         Retrieves a Dispute resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_uliddispute_get_with_http_info(ulid, async_req=True)
         >>> result = thread.get()
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2401,15 +2562,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "DisputeRead",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -2442,32 +2603,30 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param dispute_update: The updated Dispute resource (required)
         :type dispute_update: DisputeUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputeRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_uliddispute_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_uliddispute_patch_with_http_info(ulid, dispute_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_uliddispute_patch_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], dispute_update : Annotated[DisputeUpdate, Field(..., description="The updated Dispute resource")], **kwargs):  # noqa: E501
+    def api_transactions_uliddispute_patch_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], dispute_update : Annotated[DisputeUpdate, Field(..., description="The updated Dispute resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Interact with a Dispute  # noqa: E501
 
         Only authenticated Persona can interact with a Dispute object. Usually through our web application.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_uliddispute_patch_with_http_info(ulid, dispute_update, async_req=True)
@@ -2475,21 +2634,22 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param dispute_update: The updated Dispute resource (required)
         :type dispute_update: DisputeUpdate
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2542,36 +2702,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['dispute_update']:
+        if _params['dispute_update'] is not None:
             _body_params = _params['dispute_update']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['personaAuthKey']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey']  # noqa: E501
 
         _response_types_map = {
             '200': "DisputeRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/transactions/{ulid}/dispute', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
@@ -2600,32 +2760,30 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param dispute_write: The new Dispute resource (required)
         :type dispute_write: DisputeWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DisputePostCreationRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_uliddispute_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_uliddispute_post_with_http_info(ulid, dispute_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_uliddispute_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], dispute_write : Annotated[DisputeWrite, Field(..., description="The new Dispute resource")], **kwargs):  # noqa: E501
+    def api_transactions_uliddispute_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], dispute_write : Annotated[DisputeWrite, Field(..., description="The new Dispute resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Open a Dispute related to existing Transaction  # noqa: E501
 
         Creates a Dispute resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_uliddispute_post_with_http_info(ulid, dispute_write, async_req=True)
@@ -2633,21 +2791,22 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param dispute_write: The new Dispute resource (required)
         :type dispute_write: DisputeWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2700,35 +2859,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['dispute_write']:
+        if _params['dispute_write'] is not None:
             _body_params = _params['dispute_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "DisputePostCreationRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/transactions/{ulid}/dispute', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -2757,32 +2916,30 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[object]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_ulidparcels_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_ulidparcels_get_collection_with_http_info(ulid, page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_ulidparcels_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
+    def api_transactions_ulidparcels_get_collection_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Read shipments from Transaction  # noqa: E501
 
         Retrieves the collection of Parcel resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_ulidparcels_get_collection_with_http_info(ulid, page, async_req=True)
@@ -2790,21 +2947,22 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -2865,15 +3023,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'personaAuthKey']  # noqa: E501
 
         _response_types_map = {
             '200': "List[object]",
         }
 
         return self.api_client.call_api(
             '/transactions/{ulid}/parcels', 'GET',
@@ -2905,32 +3063,30 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param id: Parcel identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_ulidparcels_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_ulidparcels_id_delete_with_http_info(ulid, id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_ulidparcels_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], id : Annotated[StrictStr, Field(..., description="Parcel identifier")], **kwargs):  # noqa: E501
+    def api_transactions_ulidparcels_id_delete_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], id : Annotated[StrictStr, Field(..., description="Parcel identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Withdraw shipment from Transaction  # noqa: E501
 
         No one except the support can do that manoeuvre.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_ulidparcels_id_delete_with_http_info(ulid, id, async_req=True)
@@ -2938,21 +3094,22 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param id: Parcel identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -3009,15 +3166,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/transactions/{ulid}/parcels/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -3047,32 +3204,30 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param parcel_write: The new Parcel resource (required)
         :type parcel_write: ParcelWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ParcelRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_transactions_ulidparcels_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_transactions_ulidparcels_post_with_http_info(ulid, parcel_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_transactions_ulidparcels_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], parcel_write : Annotated[ParcelWrite, Field(..., description="The new Parcel resource")], **kwargs):  # noqa: E501
+    def api_transactions_ulidparcels_post_with_http_info(self, ulid : Annotated[StrictStr, Field(..., description="Transaction identifier")], parcel_write : Annotated[ParcelWrite, Field(..., description="The new Parcel resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Manually declare package shipped for Transaction  # noqa: E501
 
         Creates a Parcel resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_transactions_ulidparcels_post_with_http_info(ulid, parcel_write, async_req=True)
@@ -3080,21 +3235,22 @@
 
         :param ulid: Transaction identifier (required)
         :type ulid: str
         :param parcel_write: The new Parcel resource (required)
         :type parcel_write: ParcelWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -3147,15 +3303,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['parcel_write']:
+        if _params['parcel_write'] is not None:
             _body_params = _params['parcel_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -3165,17 +3321,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "ParcelRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/transactions/{ulid}/parcels', 'POST',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/user_api.py` & `tpdk-2.0.7/tpdk/api/user_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from tpdk.models.organization_read import OrganizationRead
-from tpdk.models.organization_update import OrganizationUpdate
-from tpdk.models.persona import Persona
+from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
+from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.user import User
 from tpdk.models.user_email_validation_write import UserEmailValidationWrite
 from tpdk.models.user_post_register_read import UserPostRegisterRead
 from tpdk.models.user_support_read import UserSupportRead
 from tpdk.models.user_write import UserWrite
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class UserApi(object):
@@ -49,243 +51,84 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def api_organizations_id_patch(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], organization_update : Annotated[OrganizationUpdate, Field(..., description="The updated Organization resource")], **kwargs) -> OrganizationRead:  # noqa: E501
-        """Update your Organization details, branding or parameters  # noqa: E501
-
-        Updates the Organization resource.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.api_organizations_id_patch(id, organization_update, async_req=True)
-        >>> result = thread.get()
-
-        :param id: Organization identifier (required)
-        :type id: str
-        :param organization_update: The updated Organization resource (required)
-        :type organization_update: OrganizationUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: OrganizationRead
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.api_organizations_id_patch_with_http_info(id, organization_update, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def api_organizations_id_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization identifier")], organization_update : Annotated[OrganizationUpdate, Field(..., description="The updated Organization resource")], **kwargs):  # noqa: E501
-        """Update your Organization details, branding or parameters  # noqa: E501
-
-        Updates the Organization resource.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.api_organizations_id_patch_with_http_info(id, organization_update, async_req=True)
-        >>> result = thread.get()
-
-        :param id: Organization identifier (required)
-        :type id: str
-        :param organization_update: The updated Organization resource (required)
-        :type organization_update: OrganizationUpdate
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(OrganizationRead, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'id',
-            'organization_update'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method api_organizations_id_patch" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params['organization_update']:
-            _body_params = _params['organization_update']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ['oauth']  # noqa: E501
-
-        _response_types_map = {
-            '200': "OrganizationRead",
-            '400': None,
-            '404': None,
-            '422': None,
-        }
-
-        return self.api_client.call_api(
-            '/organizations/{id}', 'PATCH',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def api_personasauthentication_post(self, persona : Annotated[Persona, Field(..., description="The new Persona resource")], **kwargs) -> Persona:  # noqa: E501
+    def api_personasauthentication_post(self, persona_persona_external_auth : Annotated[PersonaPersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> PersonaPersonaAuthReturn:  # noqa: E501
         """Persona Authentication  # noqa: E501
 
         Main route for Persona (Organization customers) to authenticate themselves. Public access, captcha protected and MFA mandatory.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personasauthentication_post(persona, async_req=True)
+        >>> thread = api.api_personasauthentication_post(persona_persona_external_auth, async_req=True)
         >>> result = thread.get()
 
-        :param persona: The new Persona resource (required)
-        :type persona: Persona
+        :param persona_persona_external_auth: The new Persona resource (required)
+        :type persona_persona_external_auth: PersonaPersonaExternalAuth
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Persona
+        :rtype: PersonaPersonaAuthReturn
         """
         kwargs['_return_http_data_only'] = True
-        return self.api_personasauthentication_post_with_http_info(persona, **kwargs)  # noqa: E501
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personasauthentication_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.api_personasauthentication_post_with_http_info(persona_persona_external_auth, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personasauthentication_post_with_http_info(self, persona : Annotated[Persona, Field(..., description="The new Persona resource")], **kwargs):  # noqa: E501
+    def api_personasauthentication_post_with_http_info(self, persona_persona_external_auth : Annotated[PersonaPersonaExternalAuth, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Persona Authentication  # noqa: E501
 
         Main route for Persona (Organization customers) to authenticate themselves. Public access, captcha protected and MFA mandatory.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_personasauthentication_post_with_http_info(persona, async_req=True)
+        >>> thread = api.api_personasauthentication_post_with_http_info(persona_persona_external_auth, async_req=True)
         >>> result = thread.get()
 
-        :param persona: The new Persona resource (required)
-        :type persona: Persona
+        :param persona_persona_external_auth: The new Persona resource (required)
+        :type persona_persona_external_auth: PersonaPersonaExternalAuth
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Persona, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PersonaPersonaAuthReturn, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'persona'
+            'persona_persona_external_auth'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -315,16 +158,16 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona']:
-            _body_params = _params['persona']
+        if _params['persona_persona_external_auth'] is not None:
+            _body_params = _params['persona_persona_external_auth']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -333,15 +176,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
-            '201': "Persona",
+            '201': "PersonaPersonaAuthReturn",
             '400': None,
             '422': None,
         }
 
         return self.api_client.call_api(
             '/personas/authentication', 'POST',
             _path_params,
@@ -370,52 +213,51 @@
         >>> thread = api.api_personasregister_post(persona_register, async_req=True)
         >>> result = thread.get()
 
         :param persona_register: The new Persona resource (required)
         :type persona_register: PersonaRegister
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: PersonaRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_personasregister_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_personasregister_post_with_http_info(persona_register, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_personasregister_post_with_http_info(self, persona_register : Annotated[PersonaRegister, Field(..., description="The new Persona resource")], **kwargs):  # noqa: E501
+    def api_personasregister_post_with_http_info(self, persona_register : Annotated[PersonaRegister, Field(..., description="The new Persona resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Persona external registration  # noqa: E501
 
         Creates a Persona resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_personasregister_post_with_http_info(persona_register, async_req=True)
         >>> result = thread.get()
 
         :param persona_register: The new Persona resource (required)
         :type persona_register: PersonaRegister
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -464,15 +306,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['persona_register']:
+        if _params['persona_register'] is not None:
             _body_params = _params['persona_register']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -519,52 +361,51 @@
         >>> thread = api.api_register_post(user_write, async_req=True)
         >>> result = thread.get()
 
         :param user_write: The new User resource (required)
         :type user_write: UserWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: UserPostRegisterRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_register_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_register_post_with_http_info(user_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_register_post_with_http_info(self, user_write : Annotated[UserWrite, Field(..., description="The new User resource")], **kwargs):  # noqa: E501
+    def api_register_post_with_http_info(self, user_write : Annotated[UserWrite, Field(..., description="The new User resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Organization onboarding  # noqa: E501
 
         Internal-use only, protected by a captcha. Organization first-enrollment  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_register_post_with_http_info(user_write, async_req=True)
         >>> result = thread.get()
 
         :param user_write: The new User resource (required)
         :type user_write: UserWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -613,15 +454,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['user_write']:
+        if _params['user_write'] is not None:
             _body_params = _params['user_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -631,17 +472,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "UserPostRegisterRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/register', 'POST',
             _path_params,
             _query_params,
             _header_params,
@@ -668,52 +509,51 @@
         >>> thread = api.api_users_get_collection(page, async_req=True)
         >>> result = thread.get()
 
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[UserSupportRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_users_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_users_get_collection_with_http_info(page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_users_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs):  # noqa: E501
+    def api_users_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of User resources.  # noqa: E501
 
         Retrieves the collection of User resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_get_collection_with_http_info(page, async_req=True)
         >>> result = thread.get()
 
         :param page: The collection page number
         :type page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -770,15 +610,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {
             '200': "List[UserSupportRead]",
         }
 
         return self.api_client.call_api(
             '/users', 'GET',
@@ -808,52 +648,51 @@
         >>> thread = api.api_users_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: User identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: User
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_users_id_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_users_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_users_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], **kwargs):  # noqa: E501
+    def api_users_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves a User resource.  # noqa: E501
 
         Retrieves a User resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: User identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -910,15 +749,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {
             '200': "User",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -951,32 +790,30 @@
 
         :param id: User identifier (required)
         :type id: str
         :param user_email_validation_write: The updated User resource (required)
         :type user_email_validation_write: UserEmailValidationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: UserPostRegisterRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_users_idemail_validation_patch_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_users_idemail_validation_patch_with_http_info(id, user_email_validation_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_users_idemail_validation_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], user_email_validation_write : Annotated[UserEmailValidationWrite, Field(..., description="The updated User resource")], **kwargs):  # noqa: E501
+    def api_users_idemail_validation_patch_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User identifier")], user_email_validation_write : Annotated[UserEmailValidationWrite, Field(..., description="The updated User resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Validate email ownership  # noqa: E501
 
         Updates the User resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_users_idemail_validation_patch_with_http_info(id, user_email_validation_write, async_req=True)
@@ -984,21 +821,22 @@
 
         :param id: User identifier (required)
         :type id: str
         :param user_email_validation_write: The updated User resource (required)
         :type user_email_validation_write: UserEmailValidationWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -1051,15 +889,15 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['user_email_validation_write']:
+        if _params['user_email_validation_write'] is not None:
             _body_params = _params['user_email_validation_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
@@ -1071,16 +909,16 @@
 
         # authentication setting
         _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "UserPostRegisterRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/users/{id}/email-validation', 'PATCH',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api/webhook_api.py` & `tpdk-2.0.7/tpdk/api/webhook_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
+import io
+import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, conlist
 
 from typing import Any, Dict, List, Optional
 
 from tpdk.models.webhook_history_collection_read import WebhookHistoryCollectionRead
 from tpdk.models.webhook_history_read import WebhookHistoryRead
 from tpdk.models.webhook_subscription_read import WebhookSubscriptionRead
 from tpdk.models.webhook_subscription_write import WebhookSubscriptionWrite
 
 from tpdk.api_client import ApiClient
+from tpdk.api_response import ApiResponse
 from tpdk.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class WebhookApi(object):
@@ -61,32 +64,30 @@
         :type page: int
         :param event: 
         :type event: str
         :param event2: 
         :type event2: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[WebhookHistoryCollectionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_histories_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_histories_get_collection_with_http_info(page, event, event2, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_histories_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, event : Optional[StrictStr] = None, event2 : Optional[conlist(StrictStr)] = None, **kwargs):  # noqa: E501
+    def api_webhook_histories_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, event : Optional[StrictStr] = None, event2 : Optional[conlist(StrictStr)] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of WebhookHistory resources.  # noqa: E501
 
         Retrieves the collection of WebhookHistory resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_histories_get_collection_with_http_info(page, event, event2, async_req=True)
@@ -96,21 +97,22 @@
         :type page: int
         :param event: 
         :type event: str
         :param event2: 
         :type event2: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -176,15 +178,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[WebhookHistoryCollectionRead]",
         }
 
         return self.api_client.call_api(
             '/webhook-histories', 'GET',
@@ -214,52 +216,51 @@
         >>> thread = api.api_webhook_histories_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookHistory identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: WebhookHistoryRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_histories_id_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_histories_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_histories_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookHistory identifier")], **kwargs):  # noqa: E501
+    def api_webhook_histories_id_get_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookHistory identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves a WebhookHistory resource.  # noqa: E501
 
         Retrieves a WebhookHistory resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_histories_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookHistory identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -316,15 +317,15 @@
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "WebhookHistoryRead",
             '404': None,
         }
 
         return self.api_client.call_api(
@@ -342,69 +343,68 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def api_webhook_histories_id_put(self, id : Annotated[StrictStr, Field(..., description="WebhookHistory identifier")], body : Annotated[Dict[str, Any], Field(..., description="The updated WebhookHistory resource")], **kwargs) -> WebhookHistoryRead:  # noqa: E501
-        """Replay a Webhook that ended in failure  # noqa: E501
+        """Replay a Webhook that ended up in failure  # noqa: E501
 
         Replaces the WebhookHistory resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_histories_id_put(id, body, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookHistory identifier (required)
         :type id: str
         :param body: The updated WebhookHistory resource (required)
         :type body: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: WebhookHistoryRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_histories_id_put_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_histories_id_put_with_http_info(id, body, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_histories_id_put_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookHistory identifier")], body : Annotated[Dict[str, Any], Field(..., description="The updated WebhookHistory resource")], **kwargs):  # noqa: E501
-        """Replay a Webhook that ended in failure  # noqa: E501
+    def api_webhook_histories_id_put_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookHistory identifier")], body : Annotated[Dict[str, Any], Field(..., description="The updated WebhookHistory resource")], **kwargs) -> ApiResponse:  # noqa: E501
+        """Replay a Webhook that ended up in failure  # noqa: E501
 
         Replaces the WebhookHistory resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_histories_id_put_with_http_info(id, body, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookHistory identifier (required)
         :type id: str
         :param body: The updated WebhookHistory resource (required)
         :type body: object
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -457,36 +457,36 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['body']:
+        if _params['body'] is not None:
             _body_params = _params['body']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {
             '200': "WebhookHistoryRead",
             '400': None,
-            '404': None,
             '422': None,
+            '404': None,
         }
 
         return self.api_client.call_api(
             '/webhook-histories/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
@@ -515,32 +515,30 @@
 
         :param page: The collection page number
         :type page: int
         :param event: Filter on a limited subset of event
         :type event: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[WebhookSubscriptionRead]
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_subscriptions_get_collection_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_subscriptions_get_collection_with_http_info(page, event, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_subscriptions_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, event : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of event")] = None, **kwargs):  # noqa: E501
+    def api_webhook_subscriptions_get_collection_with_http_info(self, page : Annotated[Optional[StrictInt], Field(description="The collection page number")] = None, event : Annotated[Optional[StrictStr], Field(description="Filter on a limited subset of event")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Retrieves the collection of WebhookSubscription resources.  # noqa: E501
 
         Retrieves the collection of WebhookSubscription resources.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_subscriptions_get_collection_with_http_info(page, event, async_req=True)
@@ -548,21 +546,22 @@
 
         :param page: The collection page number
         :type page: int
         :param event: Filter on a limited subset of event
         :type event: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -609,29 +608,29 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('event') is not None:  # noqa: E501
-            _query_params.append(('event', _params['event']))
+            _query_params.append(('event', _params['event'].value))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey', 'oauth']  # noqa: E501
 
         _response_types_map = {
             '200': "List[WebhookSubscriptionRead]",
         }
 
         return self.api_client.call_api(
             '/webhook-subscriptions', 'GET',
@@ -661,52 +660,51 @@
         >>> thread = api.api_webhook_subscriptions_id_delete(id, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookSubscription identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_subscriptions_id_delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_subscriptions_id_delete_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_subscriptions_id_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookSubscription identifier")], **kwargs):  # noqa: E501
+    def api_webhook_subscriptions_id_delete_with_http_info(self, id : Annotated[StrictStr, Field(..., description="WebhookSubscription identifier")], **kwargs) -> ApiResponse:  # noqa: E501
         """Removes the WebhookSubscription resource.  # noqa: E501
 
         Removes the WebhookSubscription resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_subscriptions_id_delete_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: WebhookSubscription identifier (required)
         :type id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -759,15 +757,15 @@
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
             '/webhook-subscriptions/{id}', 'DELETE',
             _path_params,
             _query_params,
@@ -795,52 +793,51 @@
         >>> thread = api.api_webhook_subscriptions_post(webhook_subscription_write, async_req=True)
         >>> result = thread.get()
 
         :param webhook_subscription_write: The new WebhookSubscription resource (required)
         :type webhook_subscription_write: WebhookSubscriptionWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: WebhookSubscriptionRead
         """
         kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the api_webhook_subscriptions_post_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.api_webhook_subscriptions_post_with_http_info(webhook_subscription_write, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def api_webhook_subscriptions_post_with_http_info(self, webhook_subscription_write : Annotated[WebhookSubscriptionWrite, Field(..., description="The new WebhookSubscription resource")], **kwargs):  # noqa: E501
+    def api_webhook_subscriptions_post_with_http_info(self, webhook_subscription_write : Annotated[WebhookSubscriptionWrite, Field(..., description="The new WebhookSubscription resource")], **kwargs) -> ApiResponse:  # noqa: E501
         """Subscribe to Event(s)  # noqa: E501
 
         Creates a WebhookSubscription resource.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.api_webhook_subscriptions_post_with_http_info(webhook_subscription_write, async_req=True)
         >>> result = thread.get()
 
         :param webhook_subscription_write: The new WebhookSubscription resource (required)
         :type webhook_subscription_write: WebhookSubscriptionWrite
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
@@ -889,35 +886,35 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['webhook_subscription_write']:
+        if _params['webhook_subscription_write'] is not None:
             _body_params = _params['webhook_subscription_write']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
-        _auth_settings = ['jwtPersonalKey', 'personaAuthKey', 'oauth']  # noqa: E501
+        _auth_settings = ['jwtPersonalKey']  # noqa: E501
 
         _response_types_map = {
+            '422': "UnprocessableEntity",
             '201': "WebhookSubscriptionRead",
             '400': None,
-            '422': "UnprocessableEntity",
         }
 
         return self.api_client.call_api(
             '/webhook-subscriptions', 'POST',
             _path_params,
             _query_params,
             _header_params,
```

### Comparing `tpdk-2.0.0b2/tpdk/api_client.py` & `tpdk-2.0.7/tpdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -22,14 +22,15 @@
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
 from tpdk.configuration import Configuration
+from tpdk.api_response import ApiResponse
 import tpdk.models
 from tpdk import rest
 from tpdk.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
@@ -72,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0-b2/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -218,44 +219,44 @@
         except ApiException as e:
             if e.body:
                 e.body = e.body.decode('utf-8')
             raise e
 
         self.last_response = response_data
 
-        return_data = response_data
-
-        if not _preload_content:
-            return return_data
-
-        response_type = response_types_map.get(str(response_data.status), None)
-
-        if response_type == "bytearray":
-            response_data.data = response_data.data
-        else:
-            match = None
-            content_type = response_data.getheader('content-type')
-            if content_type is not None:
-                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
-            encoding = match.group(1) if match else "utf-8"
-            response_data.data = response_data.data.decode(encoding)
-
-        # deserialize response data
-        if response_type == "bytearray":
-            return_data = response_data.data
-        elif response_type:
-            return_data = self.deserialize(response_data, response_type)
-        else:
-            return_data = None
+        return_data = None # assuming derialization is not needed
+        # data needs deserialization or returns HTTP data (deserialized) only
+        if _preload_content or _return_http_data_only:
+          response_type = response_types_map.get(str(response_data.status), None)
+
+          if response_type == "bytearray":
+              response_data.data = response_data.data
+          else:
+              match = None
+              content_type = response_data.getheader('content-type')
+              if content_type is not None:
+                  match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
+              encoding = match.group(1) if match else "utf-8"
+              response_data.data = response_data.data.decode(encoding)
+
+          # deserialize response data
+          if response_type == "bytearray":
+              return_data = response_data.data
+          elif response_type:
+              return_data = self.deserialize(response_data, response_type)
+          else:
+              return_data = None
 
         if _return_http_data_only:
-            return (return_data)
+            return return_data
         else:
-            return (return_data, response_data.status,
-                    response_data.getheaders())
+            return ApiResponse(status_code = response_data.status,
+                           data = return_data,
+                           headers = response_data.getheaders(),
+                           raw_data = response_data.data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
@@ -355,16 +356,16 @@
             return self.__deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
                  response_types_map=None, auth_settings=None,
                  async_req=None, _return_http_data_only=None,
-                 collection_formats=None,_preload_content=True,
-                  _request_timeout=None, _host=None, _request_auth=None):
+                 collection_formats=None, _preload_content=True,
+                 _request_timeout=None, _host=None, _request_auth=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -375,21 +376,22 @@
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
         :param response: Response data type.
         :param files dict: key -> filename, value -> filepath,
             for `multipart/form-data`.
         :param async_req bool: execute request asynchronously
-        :param _return_http_data_only: response data without head status code
-                                       and headers
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
```

### Comparing `tpdk-2.0.0b2/tpdk/configuration.py` & `tpdk-2.0.7/tpdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -162,14 +162,18 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
@@ -393,31 +397,31 @@
                     'jwtPersonalKey',
                 ),
             }
         if 'personaAuthKey' in self.api_key:
             auth['personaAuthKey'] = {
                 'type': 'api_key',
                 'in': 'header',
-                'key': 'X-Persona-Auth',
+                'key': 'X-Persona-Authorization',
                 'value': self.get_api_key_with_prefix(
                     'personaAuthKey',
                 ),
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.0-b2\n"\
-               "SDK Package Version: 2.0.0-b2".\
+               "Version of the API: 2.0.7\n"\
+               "SDK Package Version: 2.0.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tpdk-2.0.0b2/tpdk/exceptions.py` & `tpdk-2.0.7/tpdk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `tpdk-2.0.0b2/tpdk/models/__init__.py` & `tpdk-2.0.7/tpdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 # flake8: noqa
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
 from tpdk.models.address import Address
 from tpdk.models.address_independent_write import AddressIndependentWrite
 from tpdk.models.address_read import AddressRead
 from tpdk.models.address_update import AddressUpdate
 from tpdk.models.address_write import AddressWrite
+from tpdk.models.ai_hint import AiHint
 from tpdk.models.api_client import ApiClient
 from tpdk.models.dispute import Dispute
 from tpdk.models.dispute_collection_read import DisputeCollectionRead
 from tpdk.models.dispute_independent_write import DisputeIndependentWrite
 from tpdk.models.dispute_post_creation_read import DisputePostCreationRead
 from tpdk.models.dispute_read import DisputeRead
 from tpdk.models.dispute_update import DisputeUpdate
@@ -64,14 +65,16 @@
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.parcel_write import ParcelWrite
 from tpdk.models.persona import Persona
 from tpdk.models.persona_address import PersonaAddress
 from tpdk.models.persona_collection_read import PersonaCollectionRead
 from tpdk.models.persona_independent_write import PersonaIndependentWrite
 from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
+from tpdk.models.persona_persona_auth_return import PersonaPersonaAuthReturn
+from tpdk.models.persona_persona_external_auth import PersonaPersonaExternalAuth
 from tpdk.models.persona_post_auth_read import PersonaPostAuthRead
 from tpdk.models.persona_read import PersonaRead
 from tpdk.models.persona_read_address import PersonaReadAddress
 from tpdk.models.persona_register import PersonaRegister
 from tpdk.models.persona_token import PersonaToken
 from tpdk.models.persona_update import PersonaUpdate
 from tpdk.models.persona_update_address import PersonaUpdateAddress
```

### Comparing `tpdk-2.0.0b2/tpdk/models/address.py` & `tpdk-2.0.7/tpdk/models/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
@@ -38,14 +37,15 @@
     building_floor: Optional[StrictStr] = Field(None, alias="buildingFloor")
     gate_or_portal_or_inbox_code: Optional[StrictStr] = Field(None, alias="gateOrPortalOrInboxCode")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["id", "companyName", "countryCode", "zipCode", "cityName", "firstLine", "secondLine", "buildingName", "buildingFloor", "gateOrPortalOrInboxCode", "createdAt", "updatedAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -106,15 +106,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Address:
         """Create an instance of Address from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Address.parse_obj(obj)
 
         _obj = Address.parse_obj({
             "id": obj.get("id"),
             "company_name": obj.get("companyName"),
             "country_code": obj.get("countryCode"),
             "zip_code": obj.get("zipCode"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/address_independent_write.py` & `tpdk-2.0.7/tpdk/models/address_independent_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -35,14 +34,15 @@
     second_line: Optional[StrictStr] = Field(None, alias="secondLine")
     building_name: Optional[StrictStr] = Field(None, alias="buildingName")
     building_floor: Optional[StrictStr] = Field(None, alias="buildingFloor")
     gate_or_portal_or_inbox_code: Optional[StrictStr] = Field(None, alias="gateOrPortalOrInboxCode")
     __properties = ["companyName", "countryCode", "zipCode", "cityName", "firstLine", "secondLine", "buildingName", "buildingFloor", "gateOrPortalOrInboxCode"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -95,15 +95,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> AddressIndependentWrite:
         """Create an instance of AddressIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return AddressIndependentWrite.parse_obj(obj)
 
         _obj = AddressIndependentWrite.parse_obj({
             "company_name": obj.get("companyName"),
             "country_code": obj.get("countryCode"),
             "zip_code": obj.get("zipCode"),
             "city_name": obj.get("cityName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/address_read.py` & `tpdk-2.0.7/tpdk/models/address_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -37,14 +36,15 @@
     building_floor: Optional[StrictStr] = Field(None, alias="buildingFloor")
     gate_or_portal_or_inbox_code: Optional[StrictStr] = Field(None, alias="gateOrPortalOrInboxCode")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["companyName", "countryCode", "zipCode", "cityName", "firstLine", "secondLine", "buildingName", "buildingFloor", "gateOrPortalOrInboxCode", "createdAt", "updatedAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -104,15 +104,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> AddressRead:
         """Create an instance of AddressRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return AddressRead.parse_obj(obj)
 
         _obj = AddressRead.parse_obj({
             "company_name": obj.get("companyName"),
             "country_code": obj.get("countryCode"),
             "zip_code": obj.get("zipCode"),
             "city_name": obj.get("cityName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/address_update.py` & `tpdk-2.0.7/tpdk/models/address_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -35,14 +34,15 @@
     second_line: Optional[StrictStr] = Field(None, alias="secondLine")
     building_name: Optional[StrictStr] = Field(None, alias="buildingName")
     building_floor: Optional[StrictStr] = Field(None, alias="buildingFloor")
     gate_or_portal_or_inbox_code: Optional[StrictStr] = Field(None, alias="gateOrPortalOrInboxCode")
     __properties = ["companyName", "countryCode", "zipCode", "cityName", "firstLine", "secondLine", "buildingName", "buildingFloor", "gateOrPortalOrInboxCode"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -95,15 +95,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> AddressUpdate:
         """Create an instance of AddressUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return AddressUpdate.parse_obj(obj)
 
         _obj = AddressUpdate.parse_obj({
             "company_name": obj.get("companyName"),
             "country_code": obj.get("countryCode"),
             "zip_code": obj.get("zipCode"),
             "city_name": obj.get("cityName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/address_write.py` & `tpdk-2.0.7/tpdk/models/address_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -35,14 +34,15 @@
     second_line: Optional[StrictStr] = Field(None, alias="secondLine")
     building_name: Optional[StrictStr] = Field(None, alias="buildingName")
     building_floor: Optional[StrictStr] = Field(None, alias="buildingFloor")
     gate_or_portal_or_inbox_code: Optional[StrictStr] = Field(None, alias="gateOrPortalOrInboxCode")
     __properties = ["companyName", "countryCode", "zipCode", "cityName", "firstLine", "secondLine", "buildingName", "buildingFloor", "gateOrPortalOrInboxCode"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -95,15 +95,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> AddressWrite:
         """Create an instance of AddressWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return AddressWrite.parse_obj(obj)
 
         _obj = AddressWrite.parse_obj({
             "company_name": obj.get("companyName"),
             "country_code": obj.get("countryCode"),
             "zip_code": obj.get("zipCode"),
             "city_name": obj.get("cityName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/api_client.py` & `tpdk-2.0.7/tpdk/models/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist, constr
+from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 
 class ApiClient(BaseModel):
     """
     
     """
-    identifier: constr(strict=True, max_length=32) = ...
+    identifier: constr(strict=True, max_length=32) = Field(...)
     owner: Optional[StrictStr] = None
     created_at: datetime = Field(..., alias="createdAt")
     secret: Optional[StrictStr] = None
-    monthly_quota: Optional[StrictInt] = Field(None, alias="monthlyQuota")
     name: Optional[StrictStr] = None
     redirect_uris: Optional[conlist(Dict[str, Any])] = Field(None, alias="redirectUris")
     grants: Optional[conlist(Dict[str, Any])] = None
     scopes: Optional[conlist(Dict[str, Any])] = None
     active: Optional[StrictBool] = None
     allow_plain_text_pkce: Optional[StrictBool] = Field(None, alias="allowPlainTextPkce")
     confidential: Optional[StrictBool] = None
     plain_text_pkce_allowed: Optional[StrictBool] = Field(None, alias="plainTextPkceAllowed")
-    __properties = ["identifier", "owner", "createdAt", "secret", "monthlyQuota", "name", "redirectUris", "grants", "scopes", "active", "allowPlainTextPkce", "confidential", "plainTextPkceAllowed"]
+    __properties = ["identifier", "owner", "createdAt", "secret", "name", "redirectUris", "grants", "scopes", "active", "allowPlainTextPkce", "confidential", "plainTextPkceAllowed"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -73,36 +72,30 @@
             _dict['owner'] = None
 
         # set to None if secret (nullable) is None
         # and __fields_set__ contains the field
         if self.secret is None and "secret" in self.__fields_set__:
             _dict['secret'] = None
 
-        # set to None if monthly_quota (nullable) is None
-        # and __fields_set__ contains the field
-        if self.monthly_quota is None and "monthly_quota" in self.__fields_set__:
-            _dict['monthlyQuota'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ApiClient:
         """Create an instance of ApiClient from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return ApiClient.parse_obj(obj)
 
         _obj = ApiClient.parse_obj({
             "identifier": obj.get("identifier"),
             "owner": obj.get("owner"),
             "created_at": obj.get("createdAt"),
             "secret": obj.get("secret"),
-            "monthly_quota": obj.get("monthlyQuota"),
             "name": obj.get("name"),
             "redirect_uris": obj.get("redirectUris"),
             "grants": obj.get("grants"),
             "scopes": obj.get("scopes"),
             "active": obj.get("active"),
             "allow_plain_text_pkce": obj.get("allowPlainTextPkce"),
             "confidential": obj.get("confidential"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute.py` & `tpdk-2.0.7/tpdk/models/dispute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conint, conlist, validator
@@ -27,20 +26,20 @@
 from tpdk.models.view import View
 
 class Dispute(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
     id: Optional[StrictInt] = None
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     url: Optional[StrictStr] = None
     transaction: Optional[StrictStr] = None
-    status: StrictStr = ...
+    status: StrictStr = Field(...)
     redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
-    item_count: Optional[conint(strict=True, gt=0)] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
+    item_count: Optional[StrictInt] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
     issue_type: StrictStr = Field(..., alias="issueType")
     issue_in_description_type: Optional[StrictStr] = Field(None, alias="issueInDescriptionType", description="To be set only in conjunction of issueType = NOT_AS_DESCRIBED.")
     issue_details: Optional[StrictStr] = Field(None, alias="issueDetails")
     complainant_truthfulness_score: StrictInt = Field(..., alias="complainantTruthfulnessScore")
     seller_truthfulness_score: StrictInt = Field(..., alias="sellerTruthfulnessScore")
     complainant_stake: StrictStr = Field(..., alias="complainantStake")
     inferred_stake: Optional[StrictStr] = Field(None, alias="inferredStake")
@@ -52,91 +51,107 @@
     counter_partial_refund_amount: Optional[StrictInt] = Field(None, alias="counterPartialRefundAmount")
     complainant_approval: Optional[StrictBool] = Field(None, alias="complainantApproval")
     seller_approval: Optional[StrictBool] = Field(..., alias="sellerApproval")
     platform_solution: Optional[StrictStr] = Field(None, alias="platformSolution")
     platform_partial_refund_amount: Optional[conint(strict=True, gt=0)] = Field(None, alias="platformPartialRefundAmount")
     platform_approval: Optional[StrictBool] = Field(None, alias="platformApproval")
     arbitration_by: Optional[StrictStr] = Field(None, alias="arbitrationBy")
-    parcels: conlist(StrictStr) = ...
-    messages: conlist(Message) = ...
-    views: conlist(View) = ...
-    metadata: conlist(Metadata) = ...
+    parcels: conlist(StrictStr) = Field(...)
+    messages: conlist(Message) = Field(...)
+    views: conlist(View) = Field(...)
+    metadata: conlist(Metadata) = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     iri: Optional[StrictStr] = None
     message_count: Optional[StrictInt] = Field(None, alias="messageCount")
     __properties = ["id", "ulid", "url", "transaction", "status", "redirectUrl", "itemCount", "issueType", "issueInDescriptionType", "issueDetails", "complainantTruthfulnessScore", "sellerTruthfulnessScore", "complainantStake", "inferredStake", "recommendedSolution", "recommendedPartialRefundAmount", "chosenSolution", "chosenPartialRefundAmount", "counterSolution", "counterPartialRefundAmount", "complainantApproval", "sellerApproval", "platformSolution", "platformPartialRefundAmount", "platformApproval", "arbitrationBy", "parcels", "messages", "views", "metadata", "createdAt", "updatedAt", "iri", "messageCount"]
 
     @validator('status')
-    def status_validate_enum(cls, v):
-        if v not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
             raise ValueError("must be one of enum values ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED')")
-        return v
+        return value
 
     @validator('issue_type')
-    def issue_type_validate_enum(cls, v):
-        if v not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
+    def issue_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
             raise ValueError("must be one of enum values ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD')")
-        return v
+        return value
 
     @validator('issue_in_description_type')
-    def issue_in_description_type_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
+    def issue_in_description_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
             raise ValueError("must be one of enum values ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null')")
-        return v
+        return value
 
     @validator('complainant_stake')
-    def complainant_stake_validate_enum(cls, v):
-        if v not in ('LOW', 'MEDIUM', 'HIGH'):
+    def complainant_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('LOW', 'MEDIUM', 'HIGH'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH')")
-        return v
+        return value
 
     @validator('inferred_stake')
-    def inferred_stake_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
+    def inferred_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     @validator('recommended_solution')
-    def recommended_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def recommended_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('chosen_solution')
-    def chosen_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def chosen_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('counter_solution')
-    def counter_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def counter_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('platform_solution')
-    def platform_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def platform_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -275,15 +290,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Dispute:
         """Create an instance of Dispute from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Dispute.parse_obj(obj)
 
         _obj = Dispute.parse_obj({
             "id": obj.get("id"),
             "ulid": obj.get("ulid"),
             "url": obj.get("url"),
             "transaction": obj.get("transaction"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_collection_read.py` & `tpdk-2.0.7/tpdk/models/dispute_collection_read.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,93 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conint, validator
+from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
 from tpdk.models.transaction_collection_read import TransactionCollectionRead
 
 class DisputeCollectionRead(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     transaction: Optional[TransactionCollectionRead] = None
-    status: StrictStr = ...
-    item_count: Optional[conint(strict=True, gt=0)] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
+    status: StrictStr = Field(...)
+    item_count: Optional[StrictInt] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
     issue_type: StrictStr = Field(..., alias="issueType")
     issue_in_description_type: Optional[StrictStr] = Field(None, alias="issueInDescriptionType", description="To be set only in conjunction of issueType = NOT_AS_DESCRIBED.")
     complainant_stake: StrictStr = Field(..., alias="complainantStake")
     inferred_stake: Optional[StrictStr] = Field(None, alias="inferredStake")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     iri: Optional[StrictStr] = None
     message_count: Optional[StrictInt] = Field(None, alias="messageCount")
     __properties = ["ulid", "transaction", "status", "itemCount", "issueType", "issueInDescriptionType", "complainantStake", "inferredStake", "createdAt", "updatedAt", "iri", "messageCount"]
 
     @validator('status')
-    def status_validate_enum(cls, v):
-        if v not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
             raise ValueError("must be one of enum values ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED')")
-        return v
+        return value
 
     @validator('issue_type')
-    def issue_type_validate_enum(cls, v):
-        if v not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
+    def issue_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
             raise ValueError("must be one of enum values ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD')")
-        return v
+        return value
 
     @validator('issue_in_description_type')
-    def issue_in_description_type_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
+    def issue_in_description_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
             raise ValueError("must be one of enum values ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null')")
-        return v
+        return value
 
     @validator('complainant_stake')
-    def complainant_stake_validate_enum(cls, v):
-        if v not in ('LOW', 'MEDIUM', 'HIGH'):
+    def complainant_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('LOW', 'MEDIUM', 'HIGH'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH')")
-        return v
+        return value
 
     @validator('inferred_stake')
-    def inferred_stake_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
+    def inferred_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -130,15 +137,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> DisputeCollectionRead:
         """Create an instance of DisputeCollectionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return DisputeCollectionRead.parse_obj(obj)
 
         _obj = DisputeCollectionRead.parse_obj({
             "ulid": obj.get("ulid"),
             "transaction": TransactionCollectionRead.from_dict(obj.get("transaction")) if obj.get("transaction") is not None else None,
             "status": obj.get("status") if obj.get("status") is not None else 'CREATED',
             "item_count": obj.get("itemCount"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_independent_write.py` & `tpdk-2.0.7/tpdk/models/dispute_independent_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
@@ -27,18 +26,19 @@
 
 class DisputeIndependentWrite(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
     transaction: Optional[TransactionIndependentWrite] = None
     redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
-    metadata: conlist(MetadataIndependentWrite) = ...
+    metadata: conlist(MetadataIndependentWrite) = Field(...)
     __properties = ["transaction", "redirectUrl", "metadata"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -76,15 +76,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> DisputeIndependentWrite:
         """Create an instance of DisputeIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return DisputeIndependentWrite.parse_obj(obj)
 
         _obj = DisputeIndependentWrite.parse_obj({
             "transaction": TransactionIndependentWrite.from_dict(obj.get("transaction")) if obj.get("transaction") is not None else None,
             "redirect_url": obj.get("redirectUrl"),
             "metadata": [MetadataIndependentWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_post_creation_read.py` & `tpdk-2.0.7/tpdk/models/dispute_post_creation_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
 class DisputePostCreationRead(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     url: Optional[StrictStr] = None
     __properties = ["ulid", "url"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -63,15 +63,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> DisputePostCreationRead:
         """Create an instance of DisputePostCreationRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return DisputePostCreationRead.parse_obj(obj)
 
         _obj = DisputePostCreationRead.parse_obj({
             "ulid": obj.get("ulid"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_read.py` & `tpdk-2.0.7/tpdk/models/dispute_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conint, conlist, validator
 from tpdk.models.parcel_read import ParcelRead
 from tpdk.models.transaction_read import TransactionRead
 
 class DisputeRead(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     transaction: Optional[TransactionRead] = None
-    status: StrictStr = ...
-    item_count: Optional[conint(strict=True, gt=0)] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
+    status: StrictStr = Field(...)
+    item_count: Optional[StrictInt] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
     issue_type: StrictStr = Field(..., alias="issueType")
     issue_in_description_type: Optional[StrictStr] = Field(None, alias="issueInDescriptionType", description="To be set only in conjunction of issueType = NOT_AS_DESCRIBED.")
     issue_details: Optional[StrictStr] = Field(None, alias="issueDetails")
     complainant_truthfulness_score: StrictInt = Field(..., alias="complainantTruthfulnessScore")
     seller_truthfulness_score: StrictInt = Field(..., alias="sellerTruthfulnessScore")
     complainant_stake: StrictStr = Field(..., alias="complainantStake")
     inferred_stake: Optional[StrictStr] = Field(None, alias="inferredStake")
@@ -48,88 +47,104 @@
     counter_partial_refund_amount: Optional[StrictInt] = Field(None, alias="counterPartialRefundAmount")
     complainant_approval: Optional[StrictBool] = Field(None, alias="complainantApproval")
     seller_approval: Optional[StrictBool] = Field(..., alias="sellerApproval")
     platform_solution: Optional[StrictStr] = Field(None, alias="platformSolution")
     platform_partial_refund_amount: Optional[conint(strict=True, gt=0)] = Field(None, alias="platformPartialRefundAmount")
     platform_approval: Optional[StrictBool] = Field(None, alias="platformApproval")
     arbitration_by: Optional[StrictStr] = Field(None, alias="arbitrationBy")
-    parcels: conlist(ParcelRead) = ...
+    parcels: conlist(ParcelRead) = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     iri: Optional[StrictStr] = None
     message_count: Optional[StrictInt] = Field(None, alias="messageCount")
     __properties = ["ulid", "transaction", "status", "itemCount", "issueType", "issueInDescriptionType", "issueDetails", "complainantTruthfulnessScore", "sellerTruthfulnessScore", "complainantStake", "inferredStake", "recommendedSolution", "recommendedPartialRefundAmount", "chosenSolution", "chosenPartialRefundAmount", "counterSolution", "counterPartialRefundAmount", "complainantApproval", "sellerApproval", "platformSolution", "platformPartialRefundAmount", "platformApproval", "arbitrationBy", "parcels", "createdAt", "updatedAt", "iri", "messageCount"]
 
     @validator('status')
-    def status_validate_enum(cls, v):
-        if v not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED'):
             raise ValueError("must be one of enum values ('CREATED', 'SUBMITTED', 'OPENED', 'ABANDONED', 'PENDING', 'OBJECTED', 'SHIPPED', 'IN_TRANSIT', 'RETURNED', 'DISMISSED', 'RESOLVED')")
-        return v
+        return value
 
     @validator('issue_type')
-    def issue_type_validate_enum(cls, v):
-        if v not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
+    def issue_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
             raise ValueError("must be one of enum values ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD')")
-        return v
+        return value
 
     @validator('issue_in_description_type')
-    def issue_in_description_type_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
+    def issue_in_description_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
             raise ValueError("must be one of enum values ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null')")
-        return v
+        return value
 
     @validator('complainant_stake')
-    def complainant_stake_validate_enum(cls, v):
-        if v not in ('LOW', 'MEDIUM', 'HIGH'):
+    def complainant_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('LOW', 'MEDIUM', 'HIGH'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH')")
-        return v
+        return value
 
     @validator('inferred_stake')
-    def inferred_stake_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
+    def inferred_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('LOW', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     @validator('recommended_solution')
-    def recommended_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def recommended_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('chosen_solution')
-    def chosen_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def chosen_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('counter_solution')
-    def counter_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def counter_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('platform_solution')
-    def platform_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def platform_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -246,15 +261,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> DisputeRead:
         """Create an instance of DisputeRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return DisputeRead.parse_obj(obj)
 
         _obj = DisputeRead.parse_obj({
             "ulid": obj.get("ulid"),
             "transaction": TransactionRead.from_dict(obj.get("transaction")) if obj.get("transaction") is not None else None,
             "status": obj.get("status") if obj.get("status") is not None else 'CREATED',
             "item_count": obj.get("itemCount"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_update.py` & `tpdk-2.0.7/tpdk/models/dispute_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,94 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conint, validator
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
 
 class DisputeUpdate(BaseModel):
     """
     Access directly our resolution center without having used the safe-checkout feature.
     """
-    item_count: Optional[conint(strict=True, gt=0)] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
+    item_count: Optional[StrictInt] = Field(None, alias="itemCount", description="The dispute may concern only PART of the package. Specify it there.")
     issue_type: StrictStr = Field(..., alias="issueType")
     issue_in_description_type: Optional[StrictStr] = Field(None, alias="issueInDescriptionType", description="To be set only in conjunction of issueType = NOT_AS_DESCRIBED.")
     issue_details: Optional[StrictStr] = Field(None, alias="issueDetails")
     complainant_stake: StrictStr = Field(..., alias="complainantStake")
     chosen_solution: Optional[StrictStr] = Field(None, alias="chosenSolution")
     chosen_partial_refund_amount: Optional[StrictInt] = Field(None, alias="chosenPartialRefundAmount")
     counter_solution: Optional[StrictStr] = Field(None, alias="counterSolution")
     counter_partial_refund_amount: Optional[StrictInt] = Field(None, alias="counterPartialRefundAmount")
     complainant_approval: Optional[StrictBool] = Field(None, alias="complainantApproval")
     seller_approval: Optional[StrictBool] = Field(..., alias="sellerApproval")
     __properties = ["itemCount", "issueType", "issueInDescriptionType", "issueDetails", "complainantStake", "chosenSolution", "chosenPartialRefundAmount", "counterSolution", "counterPartialRefundAmount", "complainantApproval", "sellerApproval"]
 
     @validator('issue_type')
-    def issue_type_validate_enum(cls, v):
-        if v not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
+    def issue_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD'):
             raise ValueError("must be one of enum values ('NOT_AS_DESCRIBED', 'DOES_NOT_WORK', 'IS_INCOMPLETE', 'DELIVERY_ISSUE', 'ALLEGED_FRAUD')")
-        return v
+        return value
 
     @validator('issue_in_description_type')
-    def issue_in_description_type_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
+    def issue_in_description_type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null'):
             raise ValueError("must be one of enum values ('WRONG_COLOUR', 'DAMAGED_OR_USED', 'INCORRECT_FORMAT_OR_SIZE', 'DIFFERENT_MATERIAL', 'null')")
-        return v
+        return value
 
     @validator('complainant_stake')
-    def complainant_stake_validate_enum(cls, v):
-        if v not in ('LOW', 'MEDIUM', 'HIGH'):
+    def complainant_stake_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('LOW', 'MEDIUM', 'HIGH'):
             raise ValueError("must be one of enum values ('LOW', 'MEDIUM', 'HIGH')")
-        return v
+        return value
 
     @validator('chosen_solution')
-    def chosen_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def chosen_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     @validator('counter_solution')
-    def counter_solution_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
+    def counter_solution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null'):
             raise ValueError("must be one of enum values ('PARTIAL_REFUND_WITH_PARTIAL_RETURN', 'PARTIAL_REFUND_WITHOUT_RETURN', 'COMPLETE_REFUND_WITH_RETURN', 'COMPLETE_REFUND_WITHOUT_RETURN', 'ABANDON_CLAIM', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -143,15 +151,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> DisputeUpdate:
         """Create an instance of DisputeUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return DisputeUpdate.parse_obj(obj)
 
         _obj = DisputeUpdate.parse_obj({
             "item_count": obj.get("itemCount"),
             "issue_type": obj.get("issueType"),
             "issue_in_description_type": obj.get("issueInDescriptionType"),
             "issue_details": obj.get("issueDetails"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/dispute_write.py` & `tpdk-2.0.7/tpdk/models/metadata_independent_write.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class DisputeWrite(BaseModel):
+class MetadataIndependentWrite(BaseModel):
     """
     
     """
-    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
-    __properties = ["redirectUrl"]
+    key: StrictStr = Field(...)
+    value: Optional[StrictStr] = None
+    __properties = ["key", "value"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DisputeWrite:
-        """Create an instance of DisputeWrite from a JSON string"""
+    def from_json(cls, json_str: str) -> MetadataIndependentWrite:
+        """Create an instance of MetadataIndependentWrite from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if redirect_url (nullable) is None
+        # set to None if value (nullable) is None
         # and __fields_set__ contains the field
-        if self.redirect_url is None and "redirect_url" in self.__fields_set__:
-            _dict['redirectUrl'] = None
+        if self.value is None and "value" in self.__fields_set__:
+            _dict['value'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DisputeWrite:
-        """Create an instance of DisputeWrite from a dict"""
+    def from_dict(cls, obj: dict) -> MetadataIndependentWrite:
+        """Create an instance of MetadataIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return DisputeWrite.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return MetadataIndependentWrite.parse_obj(obj)
 
-        _obj = DisputeWrite.parse_obj({
-            "redirect_url": obj.get("redirectUrl")
+        _obj = MetadataIndependentWrite.parse_obj({
+            "key": obj.get("key"),
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evaluation_read.py` & `tpdk-2.0.7/tpdk/models/evaluation_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
@@ -29,14 +28,15 @@
     """
     rating: Optional[StrictInt] = None
     comment: Optional[StrictStr] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     __properties = ["rating", "comment", "createdAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -65,15 +65,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> EvaluationRead:
         """Create an instance of EvaluationRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return EvaluationRead.parse_obj(obj)
 
         _obj = EvaluationRead.parse_obj({
             "rating": obj.get("rating"),
             "comment": obj.get("comment"),
             "created_at": obj.get("createdAt")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evaluation_write.py` & `tpdk-2.0.7/tpdk/models/evaluation_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictInt, StrictStr
@@ -28,14 +27,15 @@
     
     """
     rating: Optional[StrictInt] = None
     comment: Optional[StrictStr] = None
     __properties = ["rating", "comment"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -63,15 +63,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> EvaluationWrite:
         """Create an instance of EvaluationWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return EvaluationWrite.parse_obj(obj)
 
         _obj = EvaluationWrite.parse_obj({
             "rating": obj.get("rating"),
             "comment": obj.get("comment")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evidence.py` & `tpdk-2.0.7/tpdk/models/evidence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
@@ -26,28 +25,30 @@
 class Evidence(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
     dispute: Optional[StrictStr] = None
     owner: Optional[StrictStr] = None
-    status: StrictStr = ...
+    status: StrictStr = Field(...)
     media: Optional[StrictStr] = None
     additional_information: Optional[StrictStr] = Field(None, alias="additionalInformation", description="Description of what the evidence actually is.")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["id", "dispute", "owner", "status", "media", "additionalInformation", "createdAt", "updatedAt"]
 
     @validator('status')
-    def status_validate_enum(cls, v):
-        if v not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
             raise ValueError("must be one of enum values ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -93,15 +94,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Evidence:
         """Create an instance of Evidence from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Evidence.parse_obj(obj)
 
         _obj = Evidence.parse_obj({
             "id": obj.get("id"),
             "dispute": obj.get("dispute"),
             "owner": obj.get("owner"),
             "status": obj.get("status") if obj.get("status") is not None else 'SUBMITTED',
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evidence_read.py` & `tpdk-2.0.7/tpdk/models/evidence_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
 from tpdk.models.evidence_read_media import EvidenceReadMedia
 
 class EvidenceRead(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    status: StrictStr = ...
+    status: StrictStr = Field(...)
     media: Optional[EvidenceReadMedia] = None
     additional_information: Optional[StrictStr] = Field(None, alias="additionalInformation", description="Description of what the evidence actually is.")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["id", "status", "media", "additionalInformation", "createdAt", "updatedAt"]
 
     @validator('status')
-    def status_validate_enum(cls, v):
-        if v not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
+    def status_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
             raise ValueError("must be one of enum values ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -85,15 +86,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> EvidenceRead:
         """Create an instance of EvidenceRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return EvidenceRead.parse_obj(obj)
 
         _obj = EvidenceRead.parse_obj({
             "id": obj.get("id"),
             "status": obj.get("status") if obj.get("status") is not None else 'SUBMITTED',
             "media": EvidenceReadMedia.from_dict(obj.get("media")) if obj.get("media") is not None else None,
             "additional_information": obj.get("additionalInformation"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evidence_read_media.py` & `tpdk-2.0.7/tpdk/models/evidence_read_media.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[MediaRead] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(EVIDENCEREADMEDIA_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = EvidenceReadMedia.construct()
         error_messages = []
         # validate data type: MediaRead
-        if type(v) is not MediaRead:
+        if not isinstance(v, MediaRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `MediaRead`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into EvidenceReadMedia with anyOf schemas: MediaRead. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in EvidenceReadMedia with anyOf schemas: MediaRead. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> EvidenceReadMedia:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> EvidenceReadMedia:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = EvidenceReadMedia.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[MediaRead] = None
         try:
             instance.actual_instance = MediaRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into EvidenceReadMedia with anyOf schemas: MediaRead. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/evidence_write.py` & `tpdk-2.0.7/tpdk/models/evidence_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -27,14 +26,15 @@
     """
     
     """
     additional_information: Optional[StrictStr] = Field(None, alias="additionalInformation", description="Description of what the evidence actually is.")
     __properties = ["additionalInformation"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -57,15 +57,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> EvidenceWrite:
         """Create an instance of EvidenceWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return EvidenceWrite.parse_obj(obj)
 
         _obj = EvidenceWrite.parse_obj({
             "additional_information": obj.get("additionalInformation")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/media.py` & `tpdk-2.0.7/tpdk/models/media.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictBytes, StrictInt, StrictStr
 
 class Media(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    extension: StrictStr = ...
-    filename: StrictStr = ...
+    extension: StrictStr = Field(...)
+    filename: StrictStr = Field(...)
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl")
-    file: Optional[StrictBytes] = None
+    file: Optional[Union[StrictBytes, StrictStr]] = None
     b64_encoded_tmp_file: Optional[StrictStr] = Field(None, alias="b64EncodedTmpFile")
     thumbnail: Optional[StrictStr] = Field(None, description="Associated 374x374 pixels small thumbnail")
     original: Optional[StrictStr] = None
     owner: Optional[StrictStr] = None
     thumbnail_url: Optional[StrictStr] = Field(None, alias="thumbnailUrl")
     __properties = ["id", "extension", "filename", "publicUrl", "file", "b64EncodedTmpFile", "thumbnail", "original", "owner", "thumbnailUrl"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -60,17 +60,14 @@
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                             "id",
                             "thumbnail_url",
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of file
-        if self.file:
-            _dict['file'] = self.file.to_dict()
         # set to None if public_url (nullable) is None
         # and __fields_set__ contains the field
         if self.public_url is None and "public_url" in self.__fields_set__:
             _dict['publicUrl'] = None
 
         # set to None if file (nullable) is None
         # and __fields_set__ contains the field
@@ -106,23 +103,23 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Media:
         """Create an instance of Media from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Media.parse_obj(obj)
 
         _obj = Media.parse_obj({
             "id": obj.get("id"),
             "extension": obj.get("extension"),
             "filename": obj.get("filename"),
             "public_url": obj.get("publicUrl"),
-            "file": bytearray.from_dict(obj.get("file")) if obj.get("file") is not None else None,
+            "file": obj.get("file"),
             "b64_encoded_tmp_file": obj.get("b64EncodedTmpFile"),
             "thumbnail": obj.get("thumbnail"),
             "original": obj.get("original"),
             "owner": obj.get("owner"),
             "thumbnail_url": obj.get("thumbnailUrl")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/media_read.py` & `tpdk-2.0.7/tpdk/models/media_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -27,14 +26,15 @@
     """
     
     """
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl")
     __properties = ["publicUrl"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -62,15 +62,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> MediaRead:
         """Create an instance of MediaRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return MediaRead.parse_obj(obj)
 
         _obj = MediaRead.parse_obj({
             "public_url": obj.get("publicUrl")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/message.py` & `tpdk-2.0.7/tpdk/models/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
@@ -27,19 +26,20 @@
     """
     
     """
     id: Optional[StrictInt] = None
     agent: Optional[StrictStr] = None
     var_from: Optional[StrictStr] = Field(None, alias="from")
     to: Optional[StrictStr] = None
-    body: StrictStr = ...
+    body: StrictStr = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     __properties = ["id", "agent", "from", "to", "body", "createdAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -79,15 +79,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Message:
         """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Message.parse_obj(obj)
 
         _obj = Message.parse_obj({
             "id": obj.get("id"),
             "agent": obj.get("agent"),
             "var_from": obj.get("from"),
             "to": obj.get("to"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/metadata.py` & `tpdk-2.0.7/tpdk/models/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class Metadata(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    key: StrictStr = ...
+    key: StrictStr = Field(...)
     value: Optional[StrictStr] = None
     __properties = ["id", "key", "value"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -65,15 +65,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Metadata:
         """Create an instance of Metadata from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Metadata.parse_obj(obj)
 
         _obj = Metadata.parse_obj({
             "id": obj.get("id"),
             "key": obj.get("key"),
             "value": obj.get("value")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/metadata_independent_write.py` & `tpdk-2.0.7/tpdk/models/metadata_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class MetadataIndependentWrite(BaseModel):
+class MetadataUpdate(BaseModel):
     """
     
     """
-    key: StrictStr = ...
+    key: StrictStr = Field(...)
     value: Optional[StrictStr] = None
     __properties = ["key", "value"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> MetadataIndependentWrite:
-        """Create an instance of MetadataIndependentWrite from a JSON string"""
+    def from_json(cls, json_str: str) -> MetadataUpdate:
+        """Create an instance of MetadataUpdate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -58,21 +58,21 @@
         # and __fields_set__ contains the field
         if self.value is None and "value" in self.__fields_set__:
             _dict['value'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> MetadataIndependentWrite:
-        """Create an instance of MetadataIndependentWrite from a dict"""
+    def from_dict(cls, obj: dict) -> MetadataUpdate:
+        """Create an instance of MetadataUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return MetadataIndependentWrite.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return MetadataUpdate.parse_obj(obj)
 
-        _obj = MetadataIndependentWrite.parse_obj({
+        _obj = MetadataUpdate.parse_obj({
             "key": obj.get("key"),
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/metadata_read.py` & `tpdk-2.0.7/tpdk/models/metadata_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
 class MetadataRead(BaseModel):
     """
     
     """
-    key: StrictStr = ...
+    key: StrictStr = Field(...)
     value: Optional[StrictStr] = None
     __properties = ["key", "value"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -63,15 +63,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> MetadataRead:
         """Create an instance of MetadataRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return MetadataRead.parse_obj(obj)
 
         _obj = MetadataRead.parse_obj({
             "key": obj.get("key"),
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/metadata_update.py` & `tpdk-2.0.7/tpdk/models/dispute_write.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,76 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class MetadataUpdate(BaseModel):
+class DisputeWrite(BaseModel):
     """
     
     """
-    key: StrictStr = ...
-    value: Optional[StrictStr] = None
-    __properties = ["key", "value"]
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
+    __properties = ["redirectUrl"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> MetadataUpdate:
-        """Create an instance of MetadataUpdate from a JSON string"""
+    def from_json(cls, json_str: str) -> DisputeWrite:
+        """Create an instance of DisputeWrite from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if value (nullable) is None
+        # set to None if redirect_url (nullable) is None
         # and __fields_set__ contains the field
-        if self.value is None and "value" in self.__fields_set__:
-            _dict['value'] = None
+        if self.redirect_url is None and "redirect_url" in self.__fields_set__:
+            _dict['redirectUrl'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> MetadataUpdate:
-        """Create an instance of MetadataUpdate from a dict"""
+    def from_dict(cls, obj: dict) -> DisputeWrite:
+        """Create an instance of DisputeWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return MetadataUpdate.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return DisputeWrite.parse_obj(obj)
 
-        _obj = MetadataUpdate.parse_obj({
-            "key": obj.get("key"),
-            "value": obj.get("value")
+        _obj = DisputeWrite.parse_obj({
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/metadata_write.py` & `tpdk-2.0.7/tpdk/models/metadata_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
 class MetadataWrite(BaseModel):
     """
     
     """
-    key: StrictStr = ...
+    key: StrictStr = Field(...)
     value: Optional[StrictStr] = None
     __properties = ["key", "value"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -63,15 +63,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> MetadataWrite:
         """Create an instance of MetadataWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return MetadataWrite.parse_obj(obj)
 
         _obj = MetadataWrite.parse_obj({
             "key": obj.get("key"),
             "value": obj.get("value")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/notification.py` & `tpdk-2.0.7/tpdk/models/notification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
 
 class Notification(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    type: StrictStr = ...
+    type: StrictStr = Field(...)
     seen: Optional[StrictBool] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     __properties = ["id", "type", "seen", "createdAt"]
 
     @validator('type')
-    def type_validate_enum(cls, v):
-        if v not in ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED'):
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED'):
             raise ValueError("must be one of enum values ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -68,15 +69,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Notification:
         """Create an instance of Notification from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Notification.parse_obj(obj)
 
         _obj = Notification.parse_obj({
             "id": obj.get("id"),
             "type": obj.get("type"),
             "seen": obj.get("seen"),
             "created_at": obj.get("createdAt")
```

### Comparing `tpdk-2.0.0b2/tpdk/models/notification_read.py` & `tpdk-2.0.7/tpdk/models/notification_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 
 class NotificationRead(BaseModel):
     """
     
     """
-    type: StrictStr = ...
+    type: StrictStr = Field(...)
     seen: Optional[StrictBool] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     __properties = ["type", "seen", "createdAt"]
 
     @validator('type')
-    def type_validate_enum(cls, v):
-        if v not in ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED'):
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED'):
             raise ValueError("must be one of enum values ('DISPUTE_STATE_UPDATE', 'MESSAGE_SENT', 'DISPUTE_SETTLEMENT', 'DISPUTE_ARBITRATION_REQUIRED', 'DISPUTE_RESOLVED')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -66,15 +67,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> NotificationRead:
         """Create an instance of NotificationRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return NotificationRead.parse_obj(obj)
 
         _obj = NotificationRead.parse_obj({
             "type": obj.get("type"),
             "seen": obj.get("seen"),
             "created_at": obj.get("createdAt")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/notification_update.py` & `tpdk-2.0.7/tpdk/models/notification_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictBool
@@ -27,14 +26,15 @@
     """
     
     """
     seen: Optional[StrictBool] = None
     __properties = ["seen"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -57,15 +57,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> NotificationUpdate:
         """Create an instance of NotificationUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return NotificationUpdate.parse_obj(obj)
 
         _obj = NotificationUpdate.parse_obj({
             "seen": obj.get("seen")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer.py` & `tpdk-2.0.7/tpdk/models/offer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,87 +1,91 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
 from tpdk.models.metadata import Metadata
 from tpdk.models.view import View
 
 class Offer(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
     enforce_persona_auth: StrictBool = Field(..., alias="enforcePersonaAuth", description="Mean that the generated url cannot be accessed without a generated token for a Persona. Disallow external registration.")
-    override_rate_commission_safe_checkout: StrictFloat = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
+    override_rate_commission_safe_checkout: Union[StrictFloat, StrictInt] = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
     redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
-    url: Optional[StrictStr] = ...
+    url: Optional[StrictStr] = Field(...)
     organization: Optional[StrictStr] = None
     seller: Optional[StrictStr] = Field(None, description="If the seller is actually YOUR organization, set it to NULL.")
     nature: StrictStr = Field(..., description="This WILL affect the assigned workflow. Choosing service will disable delivery for example. Refer to our technical hub for more information.")
     title: Optional[StrictStr] = None
     description: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
+    unit_price: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="unitPrice")
     currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
     item_count: StrictInt = Field(..., alias="itemCount")
-    condition: StrictStr = ...
+    condition: StrictStr = Field(...)
     weight_in_gram: Optional[StrictInt] = Field(None, alias="weightInGram")
     shipping_allowed: StrictBool = Field(..., alias="shippingAllowed", description="That toggle allows the seller to propose shipping for its item. If set in conjunction of shippingCarrier, the label will be automatically generated. Also, it will restrict the carrier to the limited subset defined.")
     hand_delivery_allowed: StrictBool = Field(..., alias="handDeliveryAllowed", description="Enable both parties to finalize the transaction in person rather than using delivery. A QR Code must be scanned by the seller once the buyer claims the product.")
     shipping_carriers: conlist(StrictStr) = Field(..., alias="shippingCarriers", description="If you wish to enable automated shipping label generation through a specific provider, specify it there.")
     ean_code: Optional[StrictStr] = Field(None, alias="eanCode")
-    metadata: conlist(Metadata) = ...
-    medias: conlist(StrictStr) = ...
-    views: conlist(View) = ...
+    can_be_sold_separately: StrictBool = Field(..., alias="canBeSoldSeparately", description="Set this flag to false to forbid a potential buyer to acquire this item separately.          This is only useful in a BulkOffer context.")
+    metadata: conlist(Metadata) = Field(...)
+    medias: conlist(StrictStr) = Field(...)
+    views: conlist(View) = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     iri: Optional[StrictStr] = None
-    __properties = ["id", "ulid", "publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "url", "organization", "seller", "nature", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "metadata", "medias", "views", "createdAt", "updatedAt", "iri"]
+    __properties = ["id", "ulid", "publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "url", "organization", "seller", "nature", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "canBeSoldSeparately", "metadata", "medias", "views", "createdAt", "updatedAt", "iri"]
 
     @validator('nature')
-    def nature_validate_enum(cls, v):
-        if v not in ('service', 'physical_item', 'dematerialized_item', 'rent_item'):
+    def nature_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('service', 'physical_item', 'dematerialized_item', 'rent_item'):
             raise ValueError("must be one of enum values ('service', 'physical_item', 'dematerialized_item', 'rent_item')")
-        return v
+        return value
 
     @validator('condition')
-    def condition_validate_enum(cls, v):
-        if v not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
+    def condition_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
             raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
-        return v
+        return value
 
     @validator('shipping_carriers')
-    def shipping_carriers_validate_enum(cls, v):
-        for i in v:
+    def shipping_carriers_validate_enum(cls, value):
+        """Validates the enum"""
+        for i in value:
             if i not in ('SwissPost', 'Colissimo', 'MondialRelay'):
                 raise ValueError("each list item must be one of ('SwissPost', 'Colissimo', 'MondialRelay')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -178,22 +182,22 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Offer:
         """Create an instance of Offer from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Offer.parse_obj(obj)
 
         _obj = Offer.parse_obj({
             "id": obj.get("id"),
             "ulid": obj.get("ulid"),
             "public_url": obj.get("publicUrl"),
-            "enforce_persona_auth": obj.get("enforcePersonaAuth"),
+            "enforce_persona_auth": obj.get("enforcePersonaAuth") if obj.get("enforcePersonaAuth") is not None else True,
             "override_rate_commission_safe_checkout": obj.get("overrideRateCommissionSafeCheckout"),
             "redirect_url": obj.get("redirectUrl"),
             "url": obj.get("url"),
             "organization": obj.get("organization"),
             "seller": obj.get("seller"),
             "nature": obj.get("nature") if obj.get("nature") is not None else 'physical_item',
             "title": obj.get("title"),
@@ -203,14 +207,15 @@
             "item_count": obj.get("itemCount") if obj.get("itemCount") is not None else 1,
             "condition": obj.get("condition") if obj.get("condition") is not None else 'USED',
             "weight_in_gram": obj.get("weightInGram"),
             "shipping_allowed": obj.get("shippingAllowed"),
             "hand_delivery_allowed": obj.get("handDeliveryAllowed") if obj.get("handDeliveryAllowed") is not None else True,
             "shipping_carriers": obj.get("shippingCarriers"),
             "ean_code": obj.get("eanCode"),
+            "can_be_sold_separately": obj.get("canBeSoldSeparately") if obj.get("canBeSoldSeparately") is not None else True,
             "metadata": [Metadata.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None,
             "medias": obj.get("medias"),
             "views": [View.from_dict(_item) for _item in obj.get("views")] if obj.get("views") is not None else None,
             "created_at": obj.get("createdAt"),
             "updated_at": obj.get("updatedAt"),
             "iri": obj.get("iri")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_collection_read.py` & `tpdk-2.0.7/tpdk/models/offer_collection_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, validator
 
 class OfferCollectionRead(BaseModel):
     """
     An Offer object represent a public listening
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
     title: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
+    unit_price: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="unitPrice")
     currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
     item_count: StrictInt = Field(..., alias="itemCount")
-    condition: StrictStr = ...
+    condition: StrictStr = Field(...)
     __properties = ["ulid", "publicUrl", "title", "unitPrice", "currencyCode", "itemCount", "condition"]
 
     @validator('condition')
-    def condition_validate_enum(cls, v):
-        if v not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
+    def condition_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
             raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -84,15 +85,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> OfferCollectionRead:
         """Create an instance of OfferCollectionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return OfferCollectionRead.parse_obj(obj)
 
         _obj = OfferCollectionRead.parse_obj({
             "ulid": obj.get("ulid"),
             "public_url": obj.get("publicUrl"),
             "title": obj.get("title"),
             "unit_price": obj.get("unitPrice"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_independent_write.py` & `tpdk-2.0.7/tpdk/models/persona_independent_write.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,152 +1,138 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import date
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, validator
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, validator
 from tpdk.models.metadata_independent_write import MetadataIndependentWrite
-from tpdk.models.offer_independent_write_seller import OfferIndependentWriteSeller
+from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
 
-class OfferIndependentWrite(BaseModel):
+class PersonaIndependentWrite(BaseModel):
     """
-    An Offer object represent a public listening
+    
     """
-    public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
-    seller: Optional[OfferIndependentWriteSeller] = None
-    nature: StrictStr = Field(..., description="This WILL affect the assigned workflow. Choosing service will disable delivery for example. Refer to our technical hub for more information.")
-    title: Optional[StrictStr] = None
-    description: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
-    currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
-    item_count: StrictInt = Field(..., alias="itemCount")
-    condition: StrictStr = ...
-    weight_in_gram: Optional[StrictInt] = Field(None, alias="weightInGram")
-    ean_code: Optional[StrictStr] = Field(None, alias="eanCode")
-    metadata: conlist(MetadataIndependentWrite) = ...
-    __properties = ["publicUrl", "seller", "nature", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition", "weightInGram", "eanCode", "metadata"]
-
-    @validator('nature')
-    def nature_validate_enum(cls, v):
-        if v not in ('service', 'physical_item', 'dematerialized_item', 'rent_item'):
-            raise ValueError("must be one of enum values ('service', 'physical_item', 'dematerialized_item', 'rent_item')")
-        return v
-
-    @validator('condition')
-    def condition_validate_enum(cls, v):
-        if v not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
-            raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
-        return v
+    first_name: Optional[StrictStr] = Field(None, alias="firstName")
+    last_name: Optional[StrictStr] = Field(None, alias="lastName")
+    gender: Optional[StrictStr] = 'RATHER_NOT_SAY'
+    date_of_birth: Optional[date] = Field(None, alias="dateOfBirth")
+    language: Optional[StrictStr] = Field(None, description="That data is used for rendering the frontend application with given language. If not set, will be inferred. Custom codes can be issued for specific requirements.")
+    email: Optional[StrictStr] = None
+    mobile_phone_number: Optional[StrictStr] = Field(None, alias="mobilePhoneNumber")
+    address: Optional[PersonaIndependentWriteAddress] = None
+    external_purchase_count: Optional[StrictInt] = Field(None, alias="externalPurchaseCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
+    external_sell_count: Optional[StrictInt] = Field(None, alias="externalSellCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
+    metadata: conlist(MetadataIndependentWrite) = Field(..., description="You can assign different meta to your Persona object for different purposes. eg. Ease searching.")
+    __properties = ["firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber", "address", "externalPurchaseCount", "externalSellCount", "metadata"]
+
+    @validator('gender')
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+            raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OfferIndependentWrite:
-        """Create an instance of OfferIndependentWrite from a JSON string"""
+    def from_json(cls, json_str: str) -> PersonaIndependentWrite:
+        """Create an instance of PersonaIndependentWrite from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of seller
-        if self.seller:
-            _dict['seller'] = self.seller.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of address
+        if self.address:
+            _dict['address'] = self.address.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in metadata (list)
         _items = []
         if self.metadata:
             for _item in self.metadata:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['metadata'] = _items
-        # set to None if public_url (nullable) is None
-        # and __fields_set__ contains the field
-        if self.public_url is None and "public_url" in self.__fields_set__:
-            _dict['publicUrl'] = None
-
-        # set to None if seller (nullable) is None
-        # and __fields_set__ contains the field
-        if self.seller is None and "seller" in self.__fields_set__:
-            _dict['seller'] = None
-
-        # set to None if description (nullable) is None
+        # set to None if date_of_birth (nullable) is None
         # and __fields_set__ contains the field
-        if self.description is None and "description" in self.__fields_set__:
-            _dict['description'] = None
+        if self.date_of_birth is None and "date_of_birth" in self.__fields_set__:
+            _dict['dateOfBirth'] = None
 
-        # set to None if unit_price (nullable) is None
+        # set to None if language (nullable) is None
         # and __fields_set__ contains the field
-        if self.unit_price is None and "unit_price" in self.__fields_set__:
-            _dict['unitPrice'] = None
+        if self.language is None and "language" in self.__fields_set__:
+            _dict['language'] = None
 
-        # set to None if currency_code (nullable) is None
+        # set to None if email (nullable) is None
         # and __fields_set__ contains the field
-        if self.currency_code is None and "currency_code" in self.__fields_set__:
-            _dict['currencyCode'] = None
+        if self.email is None and "email" in self.__fields_set__:
+            _dict['email'] = None
 
-        # set to None if weight_in_gram (nullable) is None
+        # set to None if mobile_phone_number (nullable) is None
         # and __fields_set__ contains the field
-        if self.weight_in_gram is None and "weight_in_gram" in self.__fields_set__:
-            _dict['weightInGram'] = None
+        if self.mobile_phone_number is None and "mobile_phone_number" in self.__fields_set__:
+            _dict['mobilePhoneNumber'] = None
 
-        # set to None if ean_code (nullable) is None
+        # set to None if address (nullable) is None
         # and __fields_set__ contains the field
-        if self.ean_code is None and "ean_code" in self.__fields_set__:
-            _dict['eanCode'] = None
+        if self.address is None and "address" in self.__fields_set__:
+            _dict['address'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OfferIndependentWrite:
-        """Create an instance of OfferIndependentWrite from a dict"""
+    def from_dict(cls, obj: dict) -> PersonaIndependentWrite:
+        """Create an instance of PersonaIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OfferIndependentWrite.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return PersonaIndependentWrite.parse_obj(obj)
 
-        _obj = OfferIndependentWrite.parse_obj({
-            "public_url": obj.get("publicUrl"),
-            "seller": OfferIndependentWriteSeller.from_dict(obj.get("seller")) if obj.get("seller") is not None else None,
-            "nature": obj.get("nature") if obj.get("nature") is not None else 'physical_item',
-            "title": obj.get("title"),
-            "description": obj.get("description"),
-            "unit_price": obj.get("unitPrice"),
-            "currency_code": obj.get("currencyCode") if obj.get("currencyCode") is not None else 'EUR',
-            "item_count": obj.get("itemCount") if obj.get("itemCount") is not None else 1,
-            "condition": obj.get("condition") if obj.get("condition") is not None else 'USED',
-            "weight_in_gram": obj.get("weightInGram"),
-            "ean_code": obj.get("eanCode"),
+        _obj = PersonaIndependentWrite.parse_obj({
+            "first_name": obj.get("firstName"),
+            "last_name": obj.get("lastName"),
+            "gender": obj.get("gender") if obj.get("gender") is not None else 'RATHER_NOT_SAY',
+            "date_of_birth": obj.get("dateOfBirth"),
+            "language": obj.get("language"),
+            "email": obj.get("email"),
+            "mobile_phone_number": obj.get("mobilePhoneNumber"),
+            "address": PersonaIndependentWriteAddress.from_dict(obj.get("address")) if obj.get("address") is not None else None,
+            "external_purchase_count": obj.get("externalPurchaseCount"),
+            "external_sell_count": obj.get("externalSellCount"),
             "metadata": [MetadataIndependentWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_independent_write_seller.py` & `tpdk-2.0.7/tpdk/models/offer_independent_write_seller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[PersonaIndependentWrite] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(OFFERINDEPENDENTWRITESELLER_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = OfferIndependentWriteSeller.construct()
         error_messages = []
         # validate data type: PersonaIndependentWrite
-        if type(v) is not PersonaIndependentWrite:
+        if not isinstance(v, PersonaIndependentWrite):
             error_messages.append(f"Error! Input type `{type(v)}` is not `PersonaIndependentWrite`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into OfferIndependentWriteSeller with anyOf schemas: PersonaIndependentWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in OfferIndependentWriteSeller with anyOf schemas: PersonaIndependentWrite. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> OfferIndependentWriteSeller:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> OfferIndependentWriteSeller:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = OfferIndependentWriteSeller.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[PersonaIndependentWrite] = None
         try:
             instance.actual_instance = PersonaIndependentWrite.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into OfferIndependentWriteSeller with anyOf schemas: PersonaIndependentWrite. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_post_creation_read.py` & `tpdk-2.0.7/tpdk/models/offer_post_creation_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
 class OfferPostCreationRead(BaseModel):
     """
     An Offer object represent a public listening
     """
-    url: Optional[StrictStr] = ...
+    url: Optional[StrictStr] = Field(...)
     __properties = ["url"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -63,15 +63,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> OfferPostCreationRead:
         """Create an instance of OfferPostCreationRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return OfferPostCreationRead.parse_obj(obj)
 
         _obj = OfferPostCreationRead.parse_obj({
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_read.py` & `tpdk-2.0.7/tpdk/models/offer_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, validator
 
 class OfferRead(BaseModel):
     """
     An Offer object represent a public listening
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
     nature: StrictStr = Field(..., description="This WILL affect the assigned workflow. Choosing service will disable delivery for example. Refer to our technical hub for more information.")
     title: Optional[StrictStr] = None
     description: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
+    unit_price: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="unitPrice")
     currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
     item_count: StrictInt = Field(..., alias="itemCount")
-    condition: StrictStr = ...
+    condition: StrictStr = Field(...)
     __properties = ["ulid", "publicUrl", "nature", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition"]
 
     @validator('nature')
-    def nature_validate_enum(cls, v):
-        if v not in ('service', 'physical_item', 'dematerialized_item', 'rent_item'):
+    def nature_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('service', 'physical_item', 'dematerialized_item', 'rent_item'):
             raise ValueError("must be one of enum values ('service', 'physical_item', 'dematerialized_item', 'rent_item')")
-        return v
+        return value
 
     @validator('condition')
-    def condition_validate_enum(cls, v):
-        if v not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
+    def condition_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
             raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -97,15 +99,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> OfferRead:
         """Create an instance of OfferRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return OfferRead.parse_obj(obj)
 
         _obj = OfferRead.parse_obj({
             "ulid": obj.get("ulid"),
             "public_url": obj.get("publicUrl"),
             "nature": obj.get("nature") if obj.get("nature") is not None else 'physical_item',
             "title": obj.get("title"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_update.py` & `tpdk-2.0.7/tpdk/models/offer_write.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from tpdk.models.metadata_update import MetadataUpdate
+from tpdk.models.metadata_write import MetadataWrite
 
-class OfferUpdate(BaseModel):
+class OfferWrite(BaseModel):
     """
     
     """
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
     enforce_persona_auth: StrictBool = Field(..., alias="enforcePersonaAuth", description="Mean that the generated url cannot be accessed without a generated token for a Persona. Disallow external registration.")
-    override_rate_commission_safe_checkout: StrictFloat = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
+    override_rate_commission_safe_checkout: Union[StrictFloat, StrictInt] = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
     redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
     title: Optional[StrictStr] = None
     description: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
+    unit_price: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="unitPrice")
     currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
     item_count: StrictInt = Field(..., alias="itemCount")
+    condition: StrictStr = Field(...)
     weight_in_gram: Optional[StrictInt] = Field(None, alias="weightInGram")
     shipping_allowed: StrictBool = Field(..., alias="shippingAllowed", description="That toggle allows the seller to propose shipping for its item. If set in conjunction of shippingCarrier, the label will be automatically generated. Also, it will restrict the carrier to the limited subset defined.")
     hand_delivery_allowed: StrictBool = Field(..., alias="handDeliveryAllowed", description="Enable both parties to finalize the transaction in person rather than using delivery. A QR Code must be scanned by the seller once the buyer claims the product.")
     shipping_carriers: conlist(StrictStr) = Field(..., alias="shippingCarriers", description="If you wish to enable automated shipping label generation through a specific provider, specify it there.")
     ean_code: Optional[StrictStr] = Field(None, alias="eanCode")
-    metadata: conlist(MetadataUpdate) = ...
-    __properties = ["publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "title", "description", "unitPrice", "currencyCode", "itemCount", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "metadata"]
+    can_be_sold_separately: StrictBool = Field(..., alias="canBeSoldSeparately", description="Set this flag to false to forbid a potential buyer to acquire this item separately.          This is only useful in a BulkOffer context.")
+    metadata: conlist(MetadataWrite) = Field(...)
+    __properties = ["publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "canBeSoldSeparately", "metadata"]
+
+    @validator('condition')
+    def condition_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
+            raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
+        return value
 
     @validator('shipping_carriers')
-    def shipping_carriers_validate_enum(cls, v):
-        for i in v:
+    def shipping_carriers_validate_enum(cls, value):
+        """Validates the enum"""
+        for i in value:
             if i not in ('SwissPost', 'Colissimo', 'MondialRelay'):
                 raise ValueError("each list item must be one of ('SwissPost', 'Colissimo', 'MondialRelay')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OfferUpdate:
-        """Create an instance of OfferUpdate from a JSON string"""
+    def from_json(cls, json_str: str) -> OfferWrite:
+        """Create an instance of OfferWrite from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -116,34 +126,36 @@
         # and __fields_set__ contains the field
         if self.ean_code is None and "ean_code" in self.__fields_set__:
             _dict['eanCode'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OfferUpdate:
-        """Create an instance of OfferUpdate from a dict"""
+    def from_dict(cls, obj: dict) -> OfferWrite:
+        """Create an instance of OfferWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OfferUpdate.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return OfferWrite.parse_obj(obj)
 
-        _obj = OfferUpdate.parse_obj({
+        _obj = OfferWrite.parse_obj({
             "public_url": obj.get("publicUrl"),
-            "enforce_persona_auth": obj.get("enforcePersonaAuth"),
+            "enforce_persona_auth": obj.get("enforcePersonaAuth") if obj.get("enforcePersonaAuth") is not None else True,
             "override_rate_commission_safe_checkout": obj.get("overrideRateCommissionSafeCheckout"),
             "redirect_url": obj.get("redirectUrl"),
             "title": obj.get("title"),
             "description": obj.get("description"),
             "unit_price": obj.get("unitPrice"),
             "currency_code": obj.get("currencyCode") if obj.get("currencyCode") is not None else 'EUR',
             "item_count": obj.get("itemCount") if obj.get("itemCount") is not None else 1,
+            "condition": obj.get("condition") if obj.get("condition") is not None else 'USED',
             "weight_in_gram": obj.get("weightInGram"),
             "shipping_allowed": obj.get("shippingAllowed"),
             "hand_delivery_allowed": obj.get("handDeliveryAllowed") if obj.get("handDeliveryAllowed") is not None else True,
             "shipping_carriers": obj.get("shippingCarriers"),
             "ean_code": obj.get("eanCode"),
-            "metadata": [MetadataUpdate.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
+            "can_be_sold_separately": obj.get("canBeSoldSeparately") if obj.get("canBeSoldSeparately") is not None else True,
+            "metadata": [MetadataWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/offer_write.py` & `tpdk-2.0.7/tpdk/models/offer_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from tpdk.models.metadata_write import MetadataWrite
+from tpdk.models.metadata_update import MetadataUpdate
 
-class OfferWrite(BaseModel):
+class OfferUpdate(BaseModel):
     """
     
     """
     public_url: Optional[StrictStr] = Field(None, alias="publicUrl", description="If specified, there would be not need for you to fill-in details. Must be accessible over WAN.")
     enforce_persona_auth: StrictBool = Field(..., alias="enforcePersonaAuth", description="Mean that the generated url cannot be accessed without a generated token for a Persona. Disallow external registration.")
-    override_rate_commission_safe_checkout: StrictFloat = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
+    override_rate_commission_safe_checkout: Union[StrictFloat, StrictInt] = Field(..., alias="overrideRateCommissionSafeCheckout", description="Override YOUR platform fees for that particular Offer.")
     redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="Fill-in that field IF you intend to redirect your customer instead of using a WebView.")
     title: Optional[StrictStr] = None
     description: Optional[StrictStr] = None
-    unit_price: Optional[StrictFloat] = Field(None, alias="unitPrice")
+    unit_price: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="unitPrice")
     currency_code: Optional[StrictStr] = Field('EUR', alias="currencyCode")
     item_count: StrictInt = Field(..., alias="itemCount")
-    condition: StrictStr = ...
     weight_in_gram: Optional[StrictInt] = Field(None, alias="weightInGram")
     shipping_allowed: StrictBool = Field(..., alias="shippingAllowed", description="That toggle allows the seller to propose shipping for its item. If set in conjunction of shippingCarrier, the label will be automatically generated. Also, it will restrict the carrier to the limited subset defined.")
     hand_delivery_allowed: StrictBool = Field(..., alias="handDeliveryAllowed", description="Enable both parties to finalize the transaction in person rather than using delivery. A QR Code must be scanned by the seller once the buyer claims the product.")
     shipping_carriers: conlist(StrictStr) = Field(..., alias="shippingCarriers", description="If you wish to enable automated shipping label generation through a specific provider, specify it there.")
     ean_code: Optional[StrictStr] = Field(None, alias="eanCode")
-    metadata: conlist(MetadataWrite) = ...
-    __properties = ["publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "title", "description", "unitPrice", "currencyCode", "itemCount", "condition", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "metadata"]
-
-    @validator('condition')
-    def condition_validate_enum(cls, v):
-        if v not in ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE'):
-            raise ValueError("must be one of enum values ('NEW', 'USED', 'DAMAGED', 'DETERIORATED', 'UNRECOVERABLE')")
-        return v
+    can_be_sold_separately: StrictBool = Field(..., alias="canBeSoldSeparately", description="Set this flag to false to forbid a potential buyer to acquire this item separately.          This is only useful in a BulkOffer context.")
+    metadata: conlist(MetadataUpdate) = Field(...)
+    __properties = ["publicUrl", "enforcePersonaAuth", "overrideRateCommissionSafeCheckout", "redirectUrl", "title", "description", "unitPrice", "currencyCode", "itemCount", "weightInGram", "shippingAllowed", "handDeliveryAllowed", "shippingCarriers", "eanCode", "canBeSoldSeparately", "metadata"]
 
     @validator('shipping_carriers')
-    def shipping_carriers_validate_enum(cls, v):
-        for i in v:
+    def shipping_carriers_validate_enum(cls, value):
+        """Validates the enum"""
+        for i in value:
             if i not in ('SwissPost', 'Colissimo', 'MondialRelay'):
                 raise ValueError("each list item must be one of ('SwissPost', 'Colissimo', 'MondialRelay')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OfferWrite:
-        """Create an instance of OfferWrite from a JSON string"""
+    def from_json(cls, json_str: str) -> OfferUpdate:
+        """Create an instance of OfferUpdate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -123,35 +118,35 @@
         # and __fields_set__ contains the field
         if self.ean_code is None and "ean_code" in self.__fields_set__:
             _dict['eanCode'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OfferWrite:
-        """Create an instance of OfferWrite from a dict"""
+    def from_dict(cls, obj: dict) -> OfferUpdate:
+        """Create an instance of OfferUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OfferWrite.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return OfferUpdate.parse_obj(obj)
 
-        _obj = OfferWrite.parse_obj({
+        _obj = OfferUpdate.parse_obj({
             "public_url": obj.get("publicUrl"),
-            "enforce_persona_auth": obj.get("enforcePersonaAuth"),
+            "enforce_persona_auth": obj.get("enforcePersonaAuth") if obj.get("enforcePersonaAuth") is not None else True,
             "override_rate_commission_safe_checkout": obj.get("overrideRateCommissionSafeCheckout"),
             "redirect_url": obj.get("redirectUrl"),
             "title": obj.get("title"),
             "description": obj.get("description"),
             "unit_price": obj.get("unitPrice"),
             "currency_code": obj.get("currencyCode") if obj.get("currencyCode") is not None else 'EUR',
             "item_count": obj.get("itemCount") if obj.get("itemCount") is not None else 1,
-            "condition": obj.get("condition") if obj.get("condition") is not None else 'USED',
             "weight_in_gram": obj.get("weightInGram"),
             "shipping_allowed": obj.get("shippingAllowed"),
             "hand_delivery_allowed": obj.get("handDeliveryAllowed") if obj.get("handDeliveryAllowed") is not None else True,
             "shipping_carriers": obj.get("shippingCarriers"),
             "ean_code": obj.get("eanCode"),
-            "metadata": [MetadataWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
+            "can_be_sold_separately": obj.get("canBeSoldSeparately") if obj.get("canBeSoldSeparately") is not None else True,
+            "metadata": [MetadataUpdate.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_read.py` & `tpdk-2.0.7/tpdk/models/organization_support_read.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, StrictInt, StrictStr
 
-class OrganizationRead(BaseModel):
+class OrganizationSupportRead(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
     name: Optional[StrictStr] = None
-    domain_verified: StrictBool = Field(..., alias="domainVerified")
-    __properties = ["id", "name", "domainVerified"]
+    __properties = ["id", "name"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationRead:
-        """Create an instance of OrganizationRead from a JSON string"""
+    def from_json(cls, json_str: str) -> OrganizationSupportRead:
+        """Create an instance of OrganizationSupportRead from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                             "id",
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationRead:
-        """Create an instance of OrganizationRead from a dict"""
+    def from_dict(cls, obj: dict) -> OrganizationSupportRead:
+        """Create an instance of OrganizationSupportRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OrganizationRead.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return OrganizationSupportRead.parse_obj(obj)
 
-        _obj = OrganizationRead.parse_obj({
+        _obj = OrganizationSupportRead.parse_obj({
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "domain_verified": obj.get("domainVerified")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_support_read.py` & `tpdk-2.0.7/tpdk/models/organization_read.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class OrganizationSupportRead(BaseModel):
+class OrganizationRead(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
     name: Optional[StrictStr] = None
-    __properties = ["id", "name"]
+    domain_verified: StrictBool = Field(..., alias="domainVerified")
+    __properties = ["id", "name", "domainVerified"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationSupportRead:
-        """Create an instance of OrganizationSupportRead from a JSON string"""
+    def from_json(cls, json_str: str) -> OrganizationRead:
+        """Create an instance of OrganizationRead from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                             "id",
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationSupportRead:
-        """Create an instance of OrganizationSupportRead from a dict"""
+    def from_dict(cls, obj: dict) -> OrganizationRead:
+        """Create an instance of OrganizationRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return OrganizationSupportRead.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return OrganizationRead.parse_obj(obj)
 
-        _obj = OrganizationSupportRead.parse_obj({
+        _obj = OrganizationRead.parse_obj({
             "id": obj.get("id"),
-            "name": obj.get("name")
+            "name": obj.get("name"),
+            "domain_verified": obj.get("domainVerified")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_update.py` & `tpdk-2.0.7/tpdk/models/organization_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictStr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, validator
 from tpdk.models.organization_update_billing_address import OrganizationUpdateBillingAddress
 
 class OrganizationUpdate(BaseModel):
     """
     
     """
     name: Optional[StrictStr] = None
     vat_number: Optional[StrictStr] = Field(None, alias="vatNumber")
     commercial_registry_number: Optional[StrictStr] = Field(None, alias="commercialRegistryNumber")
+    webhook_url: Optional[StrictStr] = Field(None, alias="webhookUrl")
     website_url: Optional[StrictStr] = Field(None, alias="websiteUrl")
     custom_base_url: Optional[StrictStr] = Field(None, alias="customBaseUrl")
     billing_address: Optional[OrganizationUpdateBillingAddress] = Field(None, alias="billingAddress")
     primary_color: Optional[StrictStr] = Field(None, alias="primaryColor")
     secondary_color: Optional[StrictStr] = Field(None, alias="secondaryColor")
     accent_color: Optional[StrictStr] = Field(None, alias="accentColor")
     error_color: Optional[StrictStr] = Field(None, alias="errorColor")
     info_color: Optional[StrictStr] = Field(None, alias="infoColor")
     success_color: Optional[StrictStr] = Field(None, alias="successColor")
     warning_color: Optional[StrictStr] = Field(None, alias="warningColor")
-    end_user_notification_toggle: StrictBool = Field(..., alias="endUserNotificationToggle")
+    direct_notification_toggle: StrictBool = Field(..., alias="directNotificationToggle")
     anonymity_level: StrictStr = Field(..., alias="anonymityLevel")
     flat_rate_enabled: Optional[StrictBool] = Field(None, alias="flatRateEnabled")
-    rate_commission_safe_checkout: StrictFloat = Field(..., alias="rateCommissionSafeCheckout")
-    __properties = ["name", "vatNumber", "commercialRegistryNumber", "websiteUrl", "customBaseUrl", "billingAddress", "primaryColor", "secondaryColor", "accentColor", "errorColor", "infoColor", "successColor", "warningColor", "endUserNotificationToggle", "anonymityLevel", "flatRateEnabled", "rateCommissionSafeCheckout"]
+    rate_commission_safe_checkout: Union[StrictFloat, StrictInt] = Field(..., alias="rateCommissionSafeCheckout")
+    __properties = ["name", "vatNumber", "commercialRegistryNumber", "webhookUrl", "websiteUrl", "customBaseUrl", "billingAddress", "primaryColor", "secondaryColor", "accentColor", "errorColor", "infoColor", "successColor", "warningColor", "directNotificationToggle", "anonymityLevel", "flatRateEnabled", "rateCommissionSafeCheckout"]
 
     @validator('anonymity_level')
-    def anonymity_level_validate_enum(cls, v):
-        if v not in ('COMPLETE', 'PARTIAL_FIRST_NAME', 'TRANSPARENT'):
+    def anonymity_level_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('COMPLETE', 'PARTIAL_FIRST_NAME', 'TRANSPARENT'):
             raise ValueError("must be one of enum values ('COMPLETE', 'PARTIAL_FIRST_NAME', 'TRANSPARENT')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -81,14 +83,19 @@
         if self.billing_address:
             _dict['billingAddress'] = self.billing_address.to_dict()
         # set to None if vat_number (nullable) is None
         # and __fields_set__ contains the field
         if self.vat_number is None and "vat_number" in self.__fields_set__:
             _dict['vatNumber'] = None
 
+        # set to None if webhook_url (nullable) is None
+        # and __fields_set__ contains the field
+        if self.webhook_url is None and "webhook_url" in self.__fields_set__:
+            _dict['webhookUrl'] = None
+
         # set to None if website_url (nullable) is None
         # and __fields_set__ contains the field
         if self.website_url is None and "website_url" in self.__fields_set__:
             _dict['websiteUrl'] = None
 
         # set to None if custom_base_url (nullable) is None
         # and __fields_set__ contains the field
@@ -139,31 +146,32 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> OrganizationUpdate:
         """Create an instance of OrganizationUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return OrganizationUpdate.parse_obj(obj)
 
         _obj = OrganizationUpdate.parse_obj({
             "name": obj.get("name"),
             "vat_number": obj.get("vatNumber"),
             "commercial_registry_number": obj.get("commercialRegistryNumber"),
+            "webhook_url": obj.get("webhookUrl"),
             "website_url": obj.get("websiteUrl"),
             "custom_base_url": obj.get("customBaseUrl"),
             "billing_address": OrganizationUpdateBillingAddress.from_dict(obj.get("billingAddress")) if obj.get("billingAddress") is not None else None,
             "primary_color": obj.get("primaryColor"),
             "secondary_color": obj.get("secondaryColor"),
             "accent_color": obj.get("accentColor"),
             "error_color": obj.get("errorColor"),
             "info_color": obj.get("infoColor"),
             "success_color": obj.get("successColor"),
             "warning_color": obj.get("warningColor"),
-            "end_user_notification_toggle": obj.get("endUserNotificationToggle"),
+            "direct_notification_toggle": obj.get("directNotificationToggle") if obj.get("directNotificationToggle") is not None else True,
             "anonymity_level": obj.get("anonymityLevel") if obj.get("anonymityLevel") is not None else 'PARTIAL_FIRST_NAME',
             "flat_rate_enabled": obj.get("flatRateEnabled"),
             "rate_commission_safe_checkout": obj.get("rateCommissionSafeCheckout")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_update_billing_address.py` & `tpdk-2.0.7/tpdk/models/persona_address.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -17,88 +17,106 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from tpdk.models.address_update import AddressUpdate
+from tpdk.models.address import Address
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-ORGANIZATIONUPDATEBILLINGADDRESS_ANY_OF_SCHEMAS = ["AddressUpdate"]
+PERSONAADDRESS_ANY_OF_SCHEMAS = ["Address"]
 
-class OrganizationUpdateBillingAddress(BaseModel):
+class PersonaAddress(BaseModel):
     """
-    OrganizationUpdateBillingAddress
+    Always the Shipping address. Thus enabling automated package returns.
     """
 
-    # data type: AddressUpdate
-    anyof_schema_1_validator: Optional[AddressUpdate] = None
+    # data type: Address
+    anyof_schema_1_validator: Optional[Address] = None
     actual_instance: Any
-    any_of_schemas: List[str] = Field(ORGANIZATIONUPDATEBILLINGADDRESS_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(PERSONAADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = PersonaAddress.construct()
         error_messages = []
-        # validate data type: AddressUpdate
-        if type(v) is not AddressUpdate:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AddressUpdate`")
+        # validate data type: Address
+        if not isinstance(v, Address):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `Address`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into OrganizationUpdateBillingAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in PersonaAddress with anyOf schemas: Address. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationUpdateBillingAddress:
+    def from_dict(cls, obj: dict) -> PersonaAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationUpdateBillingAddress:
+    def from_json(cls, json_str: str) -> PersonaAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = PersonaAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
-        # anyof_schema_1_validator: Optional[AddressUpdate] = None
+        # anyof_schema_1_validator: Optional[Address] = None
         try:
-            instance.actual_instance = AddressUpdate.from_json(json_str)
+            instance.actual_instance = Address.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into OrganizationUpdateBillingAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into PersonaAddress with anyOf schemas: Address. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_write.py` & `tpdk-2.0.7/tpdk/models/organization_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
@@ -33,14 +32,15 @@
     vat_number: Optional[StrictStr] = Field(None, alias="vatNumber")
     commercial_registry_number: Optional[StrictStr] = Field(None, alias="commercialRegistryNumber")
     website_url: Optional[StrictStr] = Field(None, alias="websiteUrl")
     billing_address: Optional[OrganizationWriteBillingAddress] = Field(None, alias="billingAddress")
     __properties = ["id", "name", "vatNumber", "commercialRegistryNumber", "websiteUrl", "billingAddress"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -82,15 +82,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> OrganizationWrite:
         """Create an instance of OrganizationWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return OrganizationWrite.parse_obj(obj)
 
         _obj = OrganizationWrite.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "vat_number": obj.get("vatNumber"),
             "commercial_registry_number": obj.get("commercialRegistryNumber"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/organization_write_billing_address.py` & `tpdk-2.0.7/tpdk/models/persona_write_address.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -21,84 +21,102 @@
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from tpdk.models.address_write import AddressWrite
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-ORGANIZATIONWRITEBILLINGADDRESS_ANY_OF_SCHEMAS = ["AddressWrite"]
+PERSONAWRITEADDRESS_ANY_OF_SCHEMAS = ["AddressWrite"]
 
-class OrganizationWriteBillingAddress(BaseModel):
+class PersonaWriteAddress(BaseModel):
     """
-    OrganizationWriteBillingAddress
+    Always the Shipping address. Thus enabling automated package returns.
     """
 
     # data type: AddressWrite
     anyof_schema_1_validator: Optional[AddressWrite] = None
     actual_instance: Any
-    any_of_schemas: List[str] = Field(ORGANIZATIONWRITEBILLINGADDRESS_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(PERSONAWRITEADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = PersonaWriteAddress.construct()
         error_messages = []
         # validate data type: AddressWrite
-        if type(v) is not AddressWrite:
+        if not isinstance(v, AddressWrite):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AddressWrite`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into OrganizationWriteBillingAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in PersonaWriteAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationWriteBillingAddress:
+    def from_dict(cls, obj: dict) -> PersonaWriteAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationWriteBillingAddress:
+    def from_json(cls, json_str: str) -> PersonaWriteAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = PersonaWriteAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[AddressWrite] = None
         try:
             instance.actual_instance = AddressWrite.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into OrganizationWriteBillingAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into PersonaWriteAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/parcel.py` & `tpdk-2.0.7/tpdk/models/parcel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, confloat, constr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictInt, StrictStr, confloat, conint, constr, validator
 
 class Parcel(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    carrier: StrictStr = ...
-    identifier: constr(strict=True, max_length=128, min_length=4) = ...
-    price: Optional[confloat(ge=0, strict=True)] = None
+    carrier: StrictStr = Field(...)
+    identifier: constr(strict=True, max_length=128, min_length=4) = Field(...)
+    price: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = None
     currency: Optional[StrictStr] = 'EUR'
     status: Optional[StrictStr] = None
     dispute: Optional[StrictStr] = None
     transaction: Optional[StrictStr] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["id", "carrier", "identifier", "price", "currency", "status", "dispute", "transaction", "createdAt", "updatedAt"]
 
     @validator('carrier')
-    def carrier_validate_enum(cls, v):
-        if v not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
+    def carrier_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
             raise ValueError("must be one of enum values ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -105,15 +106,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Parcel:
         """Create an instance of Parcel from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Parcel.parse_obj(obj)
 
         _obj = Parcel.parse_obj({
             "id": obj.get("id"),
             "carrier": obj.get("carrier"),
             "identifier": obj.get("identifier"),
             "price": obj.get("price"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/parcel_independent_write.py` & `tpdk-2.0.7/tpdk/models/parcel_independent_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr, confloat, constr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictStr, confloat, conint, constr, validator
 
 class ParcelIndependentWrite(BaseModel):
     """
     
     """
-    carrier: StrictStr = ...
-    identifier: constr(strict=True, max_length=128, min_length=4) = ...
-    price: Optional[confloat(ge=0, strict=True)] = None
+    carrier: StrictStr = Field(...)
+    identifier: constr(strict=True, max_length=128, min_length=4) = Field(...)
+    price: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = None
     currency: Optional[StrictStr] = 'EUR'
     __properties = ["carrier", "identifier", "price", "currency"]
 
     @validator('carrier')
-    def carrier_validate_enum(cls, v):
-        if v not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
+    def carrier_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
             raise ValueError("must be one of enum values ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -76,15 +77,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> ParcelIndependentWrite:
         """Create an instance of ParcelIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return ParcelIndependentWrite.parse_obj(obj)
 
         _obj = ParcelIndependentWrite.parse_obj({
             "carrier": obj.get("carrier"),
             "identifier": obj.get("identifier"),
             "price": obj.get("price"),
             "currency": obj.get("currency") if obj.get("currency") is not None else 'EUR'
```

### Comparing `tpdk-2.0.0b2/tpdk/models/parcel_read.py` & `tpdk-2.0.7/tpdk/models/parcel_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, confloat, constr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictStr, confloat, conint, constr, validator
 
 class ParcelRead(BaseModel):
     """
     
     """
-    carrier: StrictStr = ...
-    identifier: constr(strict=True, max_length=128, min_length=4) = ...
-    price: Optional[confloat(ge=0, strict=True)] = None
+    carrier: StrictStr = Field(...)
+    identifier: constr(strict=True, max_length=128, min_length=4) = Field(...)
+    price: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = None
     currency: Optional[StrictStr] = 'EUR'
     status: Optional[StrictStr] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     __properties = ["carrier", "identifier", "price", "currency", "status", "createdAt", "updatedAt"]
 
     @validator('carrier')
-    def carrier_validate_enum(cls, v):
-        if v not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
+    def carrier_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
             raise ValueError("must be one of enum values ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -91,15 +92,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> ParcelRead:
         """Create an instance of ParcelRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return ParcelRead.parse_obj(obj)
 
         _obj = ParcelRead.parse_obj({
             "carrier": obj.get("carrier"),
             "identifier": obj.get("identifier"),
             "price": obj.get("price"),
             "currency": obj.get("currency") if obj.get("currency") is not None else 'EUR',
```

### Comparing `tpdk-2.0.0b2/tpdk/models/parcel_write.py` & `tpdk-2.0.7/tpdk/models/parcel_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr, confloat, constr, validator
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictStr, confloat, conint, constr, validator
 
 class ParcelWrite(BaseModel):
     """
     
     """
-    carrier: StrictStr = ...
-    identifier: constr(strict=True, max_length=128, min_length=4) = ...
-    price: Optional[confloat(ge=0, strict=True)] = None
+    carrier: StrictStr = Field(...)
+    identifier: constr(strict=True, max_length=128, min_length=4) = Field(...)
+    price: Optional[Union[confloat(ge=0, strict=True), conint(ge=0, strict=True)]] = None
     currency: Optional[StrictStr] = 'EUR'
     __properties = ["carrier", "identifier", "price", "currency"]
 
     @validator('carrier')
-    def carrier_validate_enum(cls, v):
-        if v not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
+    def carrier_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis'):
             raise ValueError("must be one of enum values ('SwissPost', 'MondialRelay', 'Colissimo', 'Dhl', 'Chronopost', 'ColisPrive', 'Dpd', 'Ups', 'FedEx', 'RelaisColis')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -76,15 +77,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> ParcelWrite:
         """Create an instance of ParcelWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return ParcelWrite.parse_obj(obj)
 
         _obj = ParcelWrite.parse_obj({
             "carrier": obj.get("carrier"),
             "identifier": obj.get("identifier"),
             "price": obj.get("price"),
             "currency": obj.get("currency") if obj.get("currency") is not None else 'EUR'
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona.py` & `tpdk-2.0.7/tpdk/models/persona.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date, datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, conint, conlist, validator
@@ -48,43 +47,48 @@
     mobile_phone_number: Optional[StrictStr] = Field(None, alias="mobilePhoneNumber")
     address: Optional[PersonaAddress] = None
     risk_level: Optional[StrictStr] = Field(None, alias="riskLevel", description="We sort Persona into three distinct risks' category. This is inferred from the riskScore.")
     risk_score: Optional[conint(strict=True, le=100, ge=0)] = Field(None, alias="riskScore", description="That score is regularly updated, each action taken can potentially update that value. A value close to zero mean zero risk and close to a hundred mean risky.")
     external_purchase_count: Optional[StrictInt] = Field(None, alias="externalPurchaseCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
     external_sell_count: Optional[StrictInt] = Field(None, alias="externalSellCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
     metadata: conlist(Metadata) = Field(..., description="You can assign different meta to your Persona object for different purposes. eg. Ease searching.")
-    offers: conlist(StrictStr) = ...
-    purchases: conlist(StrictStr) = ...
-    tokens: conlist(PersonaToken) = ...
-    views: conlist(View) = ...
+    offers: conlist(StrictStr) = Field(...)
+    purchases: conlist(StrictStr) = Field(...)
+    tokens: conlist(PersonaToken) = Field(...)
+    views: conlist(View) = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     offer_count: Optional[StrictInt] = Field(None, alias="offerCount", description="Issued Offers count owned by a given Persona")
     purchase_count: Optional[StrictInt] = Field(None, alias="purchaseCount")
     roles: Optional[conlist(StrictStr)] = None
     user_identifier: Optional[StrictStr] = Field(None, alias="userIdentifier", description="Either email or the mobile phone number")
     __properties = ["id", "captcha", "organization", "targetUrl", "authUrl", "expireAt", "password", "plainPassword", "firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber", "address", "riskLevel", "riskScore", "externalPurchaseCount", "externalSellCount", "metadata", "offers", "purchases", "tokens", "views", "createdAt", "updatedAt", "offerCount", "purchaseCount", "roles", "userIdentifier"]
 
     @validator('gender')
-    def gender_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
             raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
-        return v
+        return value
 
     @validator('risk_level')
-    def risk_level_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
+    def risk_level_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('WEAK', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -213,15 +217,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Persona:
         """Create an instance of Persona from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Persona.parse_obj(obj)
 
         _obj = Persona.parse_obj({
             "id": obj.get("id"),
             "captcha": obj.get("captcha"),
             "organization": obj.get("organization"),
             "target_url": obj.get("targetUrl"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_address.py` & `tpdk-2.0.7/tpdk/models/user_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -17,88 +17,106 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from tpdk.models.address import Address
+from tpdk.models.api_client import ApiClient
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-PERSONAADDRESS_ANY_OF_SCHEMAS = ["Address"]
+USERAPI_ANY_OF_SCHEMAS = ["ApiClient"]
 
-class PersonaAddress(BaseModel):
+class UserApi(BaseModel):
     """
-    Always the Shipping address. Thus enabling automated package returns.
+    UserApi
     """
 
-    # data type: Address
-    anyof_schema_1_validator: Optional[Address] = None
+    # data type: ApiClient
+    anyof_schema_1_validator: Optional[ApiClient] = None
     actual_instance: Any
-    any_of_schemas: List[str] = Field(PERSONAADDRESS_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(USERAPI_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = UserApi.construct()
         error_messages = []
-        # validate data type: Address
-        if type(v) is not Address:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Address`")
+        # validate data type: ApiClient
+        if not isinstance(v, ApiClient):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ApiClient`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaAddress with anyOf schemas: Address. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in UserApi with anyOf schemas: ApiClient. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PersonaAddress:
+    def from_dict(cls, obj: dict) -> UserApi:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> PersonaAddress:
+    def from_json(cls, json_str: str) -> UserApi:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = UserApi.construct()
         if json_str is None:
             return instance
 
         error_messages = []
-        # anyof_schema_1_validator: Optional[Address] = None
+        # anyof_schema_1_validator: Optional[ApiClient] = None
         try:
-            instance.actual_instance = Address.from_json(json_str)
+            instance.actual_instance = ApiClient.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaAddress with anyOf schemas: Address. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into UserApi with anyOf schemas: ApiClient. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_collection_read.py` & `tpdk-2.0.7/tpdk/models/persona_collection_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
@@ -35,22 +34,25 @@
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     offer_count: Optional[StrictInt] = Field(None, alias="offerCount", description="Issued Offers count owned by a given Persona")
     purchase_count: Optional[StrictInt] = Field(None, alias="purchaseCount")
     __properties = ["id", "firstName", "lastName", "email", "riskLevel", "createdAt", "updatedAt", "offerCount", "purchaseCount"]
 
     @validator('risk_level')
-    def risk_level_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
+    def risk_level_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('WEAK', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -93,15 +95,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaCollectionRead:
         """Create an instance of PersonaCollectionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaCollectionRead.parse_obj(obj)
 
         _obj = PersonaCollectionRead.parse_obj({
             "id": obj.get("id"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "email": obj.get("email"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_independent_write.py` & `tpdk-2.0.7/tpdk/models/persona_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, validator
-from tpdk.models.metadata_independent_write import MetadataIndependentWrite
-from tpdk.models.persona_independent_write_address import PersonaIndependentWriteAddress
+from tpdk.models.metadata_update import MetadataUpdate
+from tpdk.models.persona_update_address import PersonaUpdateAddress
 
-class PersonaIndependentWrite(BaseModel):
+class PersonaUpdate(BaseModel):
     """
     
     """
     first_name: Optional[StrictStr] = Field(None, alias="firstName")
     last_name: Optional[StrictStr] = Field(None, alias="lastName")
     gender: Optional[StrictStr] = 'RATHER_NOT_SAY'
     date_of_birth: Optional[date] = Field(None, alias="dateOfBirth")
     language: Optional[StrictStr] = Field(None, description="That data is used for rendering the frontend application with given language. If not set, will be inferred. Custom codes can be issued for specific requirements.")
-    email: Optional[StrictStr] = None
-    mobile_phone_number: Optional[StrictStr] = Field(None, alias="mobilePhoneNumber")
-    address: Optional[PersonaIndependentWriteAddress] = None
+    address: Optional[PersonaUpdateAddress] = None
     external_purchase_count: Optional[StrictInt] = Field(None, alias="externalPurchaseCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
     external_sell_count: Optional[StrictInt] = Field(None, alias="externalSellCount", description="Knowing the statistics on your user is used to better know its profile when you do not use the Safe-Checkout feature. Although it is not required, we recommend that you keep us informed.")
-    metadata: conlist(MetadataIndependentWrite) = Field(..., description="You can assign different meta to your Persona object for different purposes. eg. Ease searching.")
-    __properties = ["firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber", "address", "externalPurchaseCount", "externalSellCount", "metadata"]
+    metadata: conlist(MetadataUpdate) = Field(..., description="You can assign different meta to your Persona object for different purposes. eg. Ease searching.")
+    __properties = ["firstName", "lastName", "gender", "dateOfBirth", "language", "address", "externalPurchaseCount", "externalSellCount", "metadata"]
 
     @validator('gender')
-    def gender_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
             raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PersonaIndependentWrite:
-        """Create an instance of PersonaIndependentWrite from a JSON string"""
+    def from_json(cls, json_str: str) -> PersonaUpdate:
+        """Create an instance of PersonaUpdate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -89,48 +89,36 @@
             _dict['dateOfBirth'] = None
 
         # set to None if language (nullable) is None
         # and __fields_set__ contains the field
         if self.language is None and "language" in self.__fields_set__:
             _dict['language'] = None
 
-        # set to None if email (nullable) is None
-        # and __fields_set__ contains the field
-        if self.email is None and "email" in self.__fields_set__:
-            _dict['email'] = None
-
-        # set to None if mobile_phone_number (nullable) is None
-        # and __fields_set__ contains the field
-        if self.mobile_phone_number is None and "mobile_phone_number" in self.__fields_set__:
-            _dict['mobilePhoneNumber'] = None
-
         # set to None if address (nullable) is None
         # and __fields_set__ contains the field
         if self.address is None and "address" in self.__fields_set__:
             _dict['address'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PersonaIndependentWrite:
-        """Create an instance of PersonaIndependentWrite from a dict"""
+    def from_dict(cls, obj: dict) -> PersonaUpdate:
+        """Create an instance of PersonaUpdate from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
-            return PersonaIndependentWrite.parse_obj(obj)
+        if not isinstance(obj, dict):
+            return PersonaUpdate.parse_obj(obj)
 
-        _obj = PersonaIndependentWrite.parse_obj({
+        _obj = PersonaUpdate.parse_obj({
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "gender": obj.get("gender") if obj.get("gender") is not None else 'RATHER_NOT_SAY',
             "date_of_birth": obj.get("dateOfBirth"),
             "language": obj.get("language"),
-            "email": obj.get("email"),
-            "mobile_phone_number": obj.get("mobilePhoneNumber"),
-            "address": PersonaIndependentWriteAddress.from_dict(obj.get("address")) if obj.get("address") is not None else None,
+            "address": PersonaUpdateAddress.from_dict(obj.get("address")) if obj.get("address") is not None else None,
             "external_purchase_count": obj.get("externalPurchaseCount"),
             "external_sell_count": obj.get("externalSellCount"),
-            "metadata": [MetadataIndependentWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
+            "metadata": [MetadataUpdate.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_independent_write_address.py` & `tpdk-2.0.7/tpdk/models/persona_independent_write_address.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[AddressIndependentWrite] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(PERSONAINDEPENDENTWRITEADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = PersonaIndependentWriteAddress.construct()
         error_messages = []
         # validate data type: AddressIndependentWrite
-        if type(v) is not AddressIndependentWrite:
+        if not isinstance(v, AddressIndependentWrite):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AddressIndependentWrite`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaIndependentWriteAddress with anyOf schemas: AddressIndependentWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in PersonaIndependentWriteAddress with anyOf schemas: AddressIndependentWrite. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaIndependentWriteAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> PersonaIndependentWriteAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = PersonaIndependentWriteAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[AddressIndependentWrite] = None
         try:
             instance.actual_instance = AddressIndependentWrite.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into PersonaIndependentWriteAddress with anyOf schemas: AddressIndependentWrite. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_post_auth_read.py` & `tpdk-2.0.7/tpdk/models/persona_post_auth_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -28,14 +27,15 @@
     
     """
     auth_url: Optional[StrictStr] = Field(None, alias="authUrl", description="Url that is able to bypass MFA for a single user. Please note that this should not be shared between the complainant and the seller or anyone external to them.")
     expire_at: Optional[datetime] = Field(None, alias="expireAt", description="This authenticated-URL cannot be renewed, you will have to re-create one each time. Typically valid for a single hour.")
     __properties = ["authUrl", "expireAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -68,15 +68,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaPostAuthRead:
         """Create an instance of PersonaPostAuthRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaPostAuthRead.parse_obj(obj)
 
         _obj = PersonaPostAuthRead.parse_obj({
             "auth_url": obj.get("authUrl"),
             "expire_at": obj.get("expireAt")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_read.py` & `tpdk-2.0.7/tpdk/models/persona_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date, datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, conint, conlist, validator
@@ -46,30 +45,35 @@
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     offer_count: Optional[StrictInt] = Field(None, alias="offerCount", description="Issued Offers count owned by a given Persona")
     purchase_count: Optional[StrictInt] = Field(None, alias="purchaseCount")
     __properties = ["id", "firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber", "address", "riskLevel", "riskScore", "externalPurchaseCount", "externalSellCount", "metadata", "createdAt", "updatedAt", "offerCount", "purchaseCount"]
 
     @validator('gender')
-    def gender_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
             raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
-        return v
+        return value
 
     @validator('risk_level')
-    def risk_level_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
+    def risk_level_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('WEAK', 'MEDIUM', 'HIGH', 'null'):
             raise ValueError("must be one of enum values ('WEAK', 'MEDIUM', 'HIGH', 'null')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -147,15 +151,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaRead:
         """Create an instance of PersonaRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaRead.parse_obj(obj)
 
         _obj = PersonaRead.parse_obj({
             "id": obj.get("id"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "gender": obj.get("gender") if obj.get("gender") is not None else 'RATHER_NOT_SAY',
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_read_address.py` & `tpdk-2.0.7/tpdk/models/persona_read_address.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[AddressRead] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(PERSONAREADADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = PersonaReadAddress.construct()
         error_messages = []
         # validate data type: AddressRead
-        if type(v) is not AddressRead:
+        if not isinstance(v, AddressRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AddressRead`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaReadAddress with anyOf schemas: AddressRead. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in PersonaReadAddress with anyOf schemas: AddressRead. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaReadAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> PersonaReadAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = PersonaReadAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[AddressRead] = None
         try:
             instance.actual_instance = AddressRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into PersonaReadAddress with anyOf schemas: AddressRead. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_register.py` & `tpdk-2.0.7/tpdk/models/persona_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, validator
@@ -35,22 +34,25 @@
     date_of_birth: Optional[date] = Field(None, alias="dateOfBirth")
     language: Optional[StrictStr] = Field(None, description="That data is used for rendering the frontend application with given language. If not set, will be inferred. Custom codes can be issued for specific requirements.")
     email: Optional[StrictStr] = None
     mobile_phone_number: Optional[StrictStr] = Field(None, alias="mobilePhoneNumber")
     __properties = ["captcha", "plainPassword", "firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber"]
 
     @validator('gender')
-    def gender_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
             raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -103,15 +105,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaRegister:
         """Create an instance of PersonaRegister from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaRegister.parse_obj(obj)
 
         _obj = PersonaRegister.parse_obj({
             "captcha": obj.get("captcha"),
             "plain_password": obj.get("plainPassword"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_token.py` & `tpdk-2.0.7/tpdk/models/persona_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class PersonaToken(BaseModel):
     """
     
     """
     id: Optional[StrictInt] = None
-    persona: StrictStr = ...
+    persona: StrictStr = Field(...)
     object_id: Optional[StrictStr] = Field(None, alias="objectId", description="Optional limitation on a specific object.")
-    token: StrictStr = ...
+    token: StrictStr = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     expire_at: datetime = Field(..., alias="expireAt")
     __properties = ["id", "persona", "objectId", "token", "createdAt", "expireAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -69,15 +69,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaToken:
         """Create an instance of PersonaToken from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaToken.parse_obj(obj)
 
         _obj = PersonaToken.parse_obj({
             "id": obj.get("id"),
             "persona": obj.get("persona"),
             "object_id": obj.get("objectId"),
             "token": obj.get("token"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_update_address.py` & `tpdk-2.0.7/tpdk/models/persona_update_address.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[AddressUpdate] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(PERSONAUPDATEADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = PersonaUpdateAddress.construct()
         error_messages = []
         # validate data type: AddressUpdate
-        if type(v) is not AddressUpdate:
+        if not isinstance(v, AddressUpdate):
             error_messages.append(f"Error! Input type `{type(v)}` is not `AddressUpdate`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaUpdateAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in PersonaUpdateAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaUpdateAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> PersonaUpdateAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = PersonaUpdateAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[AddressUpdate] = None
         try:
             instance.actual_instance = AddressUpdate.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into PersonaUpdateAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_write.py` & `tpdk-2.0.7/tpdk/models/persona_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import date
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist, validator
@@ -37,22 +36,25 @@
     email: Optional[StrictStr] = None
     mobile_phone_number: Optional[StrictStr] = Field(None, alias="mobilePhoneNumber")
     address: Optional[PersonaWriteAddress] = None
     metadata: conlist(MetadataWrite) = Field(..., description="You can assign different meta to your Persona object for different purposes. eg. Ease searching.")
     __properties = ["firstName", "lastName", "gender", "dateOfBirth", "language", "email", "mobilePhoneNumber", "address", "metadata"]
 
     @validator('gender')
-    def gender_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
+    def gender_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY'):
             raise ValueError("must be one of enum values ('MALE', 'FEMALE', 'OTHER', 'RATHER_NOT_SAY')")
-        return v
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -110,15 +112,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> PersonaWrite:
         """Create an instance of PersonaWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return PersonaWrite.parse_obj(obj)
 
         _obj = PersonaWrite.parse_obj({
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "gender": obj.get("gender") if obj.get("gender") is not None else 'RATHER_NOT_SAY',
             "date_of_birth": obj.get("dateOfBirth"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/persona_write_address.py` & `tpdk-2.0.7/tpdk/models/organization_update_billing_address.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -17,88 +17,106 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from tpdk.models.address_write import AddressWrite
+from tpdk.models.address_update import AddressUpdate
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-PERSONAWRITEADDRESS_ANY_OF_SCHEMAS = ["AddressWrite"]
+ORGANIZATIONUPDATEBILLINGADDRESS_ANY_OF_SCHEMAS = ["AddressUpdate"]
 
-class PersonaWriteAddress(BaseModel):
+class OrganizationUpdateBillingAddress(BaseModel):
     """
-    Always the Shipping address. Thus enabling automated package returns.
+    OrganizationUpdateBillingAddress
     """
 
-    # data type: AddressWrite
-    anyof_schema_1_validator: Optional[AddressWrite] = None
+    # data type: AddressUpdate
+    anyof_schema_1_validator: Optional[AddressUpdate] = None
     actual_instance: Any
-    any_of_schemas: List[str] = Field(PERSONAWRITEADDRESS_ANY_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(ORGANIZATIONUPDATEBILLINGADDRESS_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = OrganizationUpdateBillingAddress.construct()
         error_messages = []
-        # validate data type: AddressWrite
-        if type(v) is not AddressWrite:
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AddressWrite`")
+        # validate data type: AddressUpdate
+        if not isinstance(v, AddressUpdate):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AddressUpdate`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaWriteAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in OrganizationUpdateBillingAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PersonaWriteAddress:
+    def from_dict(cls, obj: dict) -> OrganizationUpdateBillingAddress:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
-    def from_json(cls, json_str: str) -> PersonaWriteAddress:
+    def from_json(cls, json_str: str) -> OrganizationUpdateBillingAddress:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = OrganizationUpdateBillingAddress.construct()
         if json_str is None:
             return instance
 
         error_messages = []
-        # anyof_schema_1_validator: Optional[AddressWrite] = None
+        # anyof_schema_1_validator: Optional[AddressUpdate] = None
         try:
-            instance.actual_instance = AddressWrite.from_json(json_str)
+            instance.actual_instance = AddressUpdate.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PersonaWriteAddress with anyOf schemas: AddressWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into OrganizationUpdateBillingAddress with anyOf schemas: AddressUpdate. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/transaction_collection_read.py` & `tpdk-2.0.7/tpdk/models/transaction_collection_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 from tpdk.models.offer_collection_read import OfferCollectionRead
 
 class TransactionCollectionRead(BaseModel):
     """
     
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     offer: Optional[OfferCollectionRead] = None
     __properties = ["ulid", "offer"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -62,15 +62,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> TransactionCollectionRead:
         """Create an instance of TransactionCollectionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return TransactionCollectionRead.parse_obj(obj)
 
         _obj = TransactionCollectionRead.parse_obj({
             "ulid": obj.get("ulid"),
             "offer": OfferCollectionRead.from_dict(obj.get("offer")) if obj.get("offer") is not None else None
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/transaction_independent_write.py` & `tpdk-2.0.7/tpdk/models/transaction_independent_write.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictFloat, conlist
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
 from tpdk.models.metadata_independent_write import MetadataIndependentWrite
 from tpdk.models.offer_independent_write import OfferIndependentWrite
 from tpdk.models.parcel_independent_write import ParcelIndependentWrite
 from tpdk.models.persona_independent_write import PersonaIndependentWrite
 
 class TransactionIndependentWrite(BaseModel):
     """
     
     """
     offer: Optional[OfferIndependentWrite] = None
     buyer: Optional[PersonaIndependentWrite] = None
-    fees: Optional[StrictFloat] = None
-    metadata: conlist(MetadataIndependentWrite) = ...
-    parcels: conlist(ParcelIndependentWrite) = ...
+    fees: Optional[Union[StrictFloat, StrictInt]] = None
+    metadata: conlist(MetadataIndependentWrite) = Field(...)
+    parcels: conlist(ParcelIndependentWrite) = Field(...)
     __properties = ["offer", "buyer", "fees", "metadata", "parcels"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -90,15 +90,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> TransactionIndependentWrite:
         """Create an instance of TransactionIndependentWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return TransactionIndependentWrite.parse_obj(obj)
 
         _obj = TransactionIndependentWrite.parse_obj({
             "offer": OfferIndependentWrite.from_dict(obj.get("offer")) if obj.get("offer") is not None else None,
             "buyer": PersonaIndependentWrite.from_dict(obj.get("buyer")) if obj.get("buyer") is not None else None,
             "fees": obj.get("fees"),
             "metadata": [MetadataIndependentWrite.from_dict(_item) for _item in obj.get("metadata")] if obj.get("metadata") is not None else None,
```

### Comparing `tpdk-2.0.0b2/tpdk/models/transaction_read.py` & `tpdk-2.0.7/tpdk/models/transaction_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictFloat, StrictStr, conlist
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
 from tpdk.models.metadata_read import MetadataRead
 from tpdk.models.offer_read import OfferRead
 from tpdk.models.parcel_read import ParcelRead
 
 class TransactionRead(BaseModel):
     """
     
     """
-    ulid: StrictStr = ...
+    ulid: StrictStr = Field(...)
     offer: Optional[OfferRead] = None
     buyer: Optional[StrictStr] = None
-    fees: Optional[StrictFloat] = None
-    metadata: conlist(MetadataRead) = ...
-    parcels: conlist(ParcelRead) = ...
+    fees: Optional[Union[StrictFloat, StrictInt]] = None
+    metadata: conlist(MetadataRead) = Field(...)
+    parcels: conlist(ParcelRead) = Field(...)
     __properties = ["ulid", "offer", "buyer", "fees", "metadata", "parcels"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -87,15 +87,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> TransactionRead:
         """Create an instance of TransactionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return TransactionRead.parse_obj(obj)
 
         _obj = TransactionRead.parse_obj({
             "ulid": obj.get("ulid"),
             "offer": OfferRead.from_dict(obj.get("offer")) if obj.get("offer") is not None else None,
             "buyer": obj.get("buyer"),
             "fees": obj.get("fees"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/unprocessable_entity.py` & `tpdk-2.0.7/tpdk/models/unprocessable_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, StrictStr, conlist
@@ -31,14 +30,15 @@
     type: Optional[StrictStr] = None
     title: Optional[StrictStr] = None
     detail: Optional[StrictStr] = None
     violations: Optional[conlist(UnprocessableEntityViolationsInner)] = None
     __properties = ["type", "title", "detail", "violations"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -68,15 +68,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UnprocessableEntity:
         """Create an instance of UnprocessableEntity from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UnprocessableEntity.parse_obj(obj)
 
         _obj = UnprocessableEntity.parse_obj({
             "type": obj.get("type"),
             "title": obj.get("title"),
             "detail": obj.get("detail"),
             "violations": [UnprocessableEntityViolationsInner.from_dict(_item) for _item in obj.get("violations")] if obj.get("violations") is not None else None
```

### Comparing `tpdk-2.0.0b2/tpdk/models/unprocessable_entity_violations_inner.py` & `tpdk-2.0.7/tpdk/models/unprocessable_entity_violations_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -29,14 +28,15 @@
     """
     property_path: Optional[StrictStr] = Field(None, alias="propertyPath")
     message: Optional[StrictStr] = None
     code: Optional[StrictStr] = None
     __properties = ["propertyPath", "message", "code"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -59,15 +59,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UnprocessableEntityViolationsInner:
         """Create an instance of UnprocessableEntityViolationsInner from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UnprocessableEntityViolationsInner.parse_obj(obj)
 
         _obj = UnprocessableEntityViolationsInner.parse_obj({
             "property_path": obj.get("propertyPath"),
             "message": obj.get("message"),
             "code": obj.get("code")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user.py` & `tpdk-2.0.7/tpdk/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
@@ -31,43 +30,44 @@
     """
     id: Optional[StrictStr] = None
     captcha: Optional[StrictStr] = None
     first_name: Optional[StrictStr] = Field(None, alias="firstName")
     last_name: Optional[StrictStr] = Field(None, alias="lastName")
     public_name: Optional[StrictStr] = Field(None, alias="publicName")
     role_in_company: Optional[StrictStr] = Field(None, alias="roleInCompany")
-    birthday: datetime = ...
+    birthday: datetime = Field(...)
     email: Optional[StrictStr] = None
-    roles: conlist(StrictStr) = ...
+    roles: conlist(StrictStr) = Field(...)
     password: StrictStr = Field(..., description="The hashed password")
     plain_password: Optional[StrictStr] = Field(None, alias="plainPassword")
     intl_phone_number: Optional[StrictStr] = Field(None, alias="intlPhoneNumber")
     origin_country: Optional[constr(strict=True, max_length=3)] = Field(None, alias="originCountry", description="The originating country")
     preferred_language: Optional[constr(strict=True, max_length=2)] = Field(None, alias="preferredLanguage")
     last_successful_log_in: Optional[datetime] = Field(None, alias="lastSuccessfulLogIn")
     email_verification_code: Optional[StrictStr] = Field(None, alias="emailVerificationCode")
     email_verification_input: Optional[StrictStr] = Field(None, alias="emailVerificationInput")
     phone_verification_code: Optional[StrictStr] = Field(None, alias="phoneVerificationCode")
     phone_verification_input: Optional[StrictStr] = Field(None, alias="phoneVerificationInput")
     avatar: Optional[StrictStr] = None
     notifications: Optional[conlist(StrictStr)] = None
     medias: Optional[conlist(StrictStr)] = None
-    views: conlist(View) = ...
+    views: conlist(View) = Field(...)
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     consent_mail_notification: StrictBool = Field(..., alias="consentMailNotification")
     consent_mail_ads: StrictBool = Field(..., alias="consentMailAds")
     api: Optional[UserApi] = None
     organization: Optional[StrictStr] = None
     username: Optional[StrictStr] = Field(None, description="A visual identifier that represents this user.")
     salt: Optional[StrictStr] = None
     user_identifier: Optional[StrictStr] = Field(None, alias="userIdentifier")
     __properties = ["id", "captcha", "firstName", "lastName", "publicName", "roleInCompany", "birthday", "email", "roles", "password", "plainPassword", "intlPhoneNumber", "originCountry", "preferredLanguage", "lastSuccessfulLogIn", "emailVerificationCode", "emailVerificationInput", "phoneVerificationCode", "phoneVerificationInput", "avatar", "notifications", "medias", "views", "createdAt", "updatedAt", "consentMailNotification", "consentMailAds", "api", "organization", "username", "salt", "userIdentifier"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -178,15 +178,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> User:
         """Create an instance of User from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return User.parse_obj(obj)
 
         _obj = User.parse_obj({
             "id": obj.get("id"),
             "captcha": obj.get("captcha"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_email_validation_write.py` & `tpdk-2.0.7/tpdk/models/user_email_validation_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, constr
@@ -27,14 +26,15 @@
     """
     
     """
     email_verification_input: Optional[constr(strict=True, max_length=128, min_length=128)] = Field(..., alias="emailVerificationInput")
     __properties = ["emailVerificationInput"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -62,15 +62,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserEmailValidationWrite:
         """Create an instance of UserEmailValidationWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UserEmailValidationWrite.parse_obj(obj)
 
         _obj = UserEmailValidationWrite.parse_obj({
             "email_verification_input": obj.get("emailVerificationInput")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_post_register_read.py` & `tpdk-2.0.7/tpdk/models/user_post_register_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
@@ -27,14 +26,15 @@
     """
     
     """
     id: Optional[StrictStr] = None
     __properties = ["id"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -58,15 +58,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserPostRegisterRead:
         """Create an instance of UserPostRegisterRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UserPostRegisterRead.parse_obj(obj)
 
         _obj = UserPostRegisterRead.parse_obj({
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_support_read.py` & `tpdk-2.0.7/tpdk/models/user_support_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
@@ -39,14 +38,15 @@
     avatar: Optional[StrictStr] = None
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     organization: Optional[UserSupportReadOrganization] = None
     __properties = ["id", "firstName", "lastName", "publicName", "roleInCompany", "email", "intlPhoneNumber", "lastSuccessfulLogIn", "avatar", "createdAt", "updatedAt", "organization"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -105,15 +105,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserSupportRead:
         """Create an instance of UserSupportRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UserSupportRead.parse_obj(obj)
 
         _obj = UserSupportRead.parse_obj({
             "id": obj.get("id"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "public_name": obj.get("publicName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_support_read_organization.py` & `tpdk-2.0.7/tpdk/models/user_support_read_organization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[OrganizationSupportRead] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(USERSUPPORTREADORGANIZATION_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = UserSupportReadOrganization.construct()
         error_messages = []
         # validate data type: OrganizationSupportRead
-        if type(v) is not OrganizationSupportRead:
+        if not isinstance(v, OrganizationSupportRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `OrganizationSupportRead`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into UserSupportReadOrganization with anyOf schemas: OrganizationSupportRead. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in UserSupportReadOrganization with anyOf schemas: OrganizationSupportRead. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserSupportReadOrganization:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> UserSupportReadOrganization:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = UserSupportReadOrganization.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[OrganizationSupportRead] = None
         try:
             instance.actual_instance = OrganizationSupportRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into UserSupportReadOrganization with anyOf schemas: OrganizationSupportRead. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_write.py` & `tpdk-2.0.7/tpdk/models/user_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, constr
@@ -30,25 +29,26 @@
     """
     captcha: Optional[StrictStr] = None
     first_name: constr(strict=True, max_length=64, min_length=1) = Field(..., alias="firstName")
     last_name: constr(strict=True, max_length=64, min_length=1) = Field(..., alias="lastName")
     public_name: Optional[constr(strict=True, max_length=32, min_length=2)] = Field(..., alias="publicName")
     role_in_company: Optional[constr(strict=True, max_length=32, min_length=2)] = Field(..., alias="roleInCompany")
     birthday: Optional[datetime] = None
-    email: constr(strict=True, max_length=180) = ...
+    email: constr(strict=True, max_length=180) = Field(...)
     plain_password: Optional[constr(strict=True, max_length=64, min_length=6)] = Field(..., alias="plainPassword")
     intl_phone_number: Optional[StrictStr] = Field(None, alias="intlPhoneNumber")
     origin_country: StrictStr = Field(..., alias="originCountry", description="The originating country")
     preferred_language: StrictStr = Field(..., alias="preferredLanguage")
     consent_mail_notification: Optional[StrictBool] = Field(None, alias="consentMailNotification")
     consent_mail_ads: Optional[StrictBool] = Field(None, alias="consentMailAds")
     organization: Optional[UserWriteOrganization] = None
     __properties = ["captcha", "firstName", "lastName", "publicName", "roleInCompany", "birthday", "email", "plainPassword", "intlPhoneNumber", "originCountry", "preferredLanguage", "consentMailNotification", "consentMailAds", "organization"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -104,15 +104,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserWrite:
         """Create an instance of UserWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return UserWrite.parse_obj(obj)
 
         _obj = UserWrite.parse_obj({
             "captcha": obj.get("captcha"),
             "first_name": obj.get("firstName"),
             "last_name": obj.get("lastName"),
             "public_name": obj.get("publicName"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/user_write_organization.py` & `tpdk-2.0.7/tpdk/models/user_write_organization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,69 +36,87 @@
     anyof_schema_1_validator: Optional[OrganizationWrite] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(USERWRITEORGANIZATION_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
         if v is None:
             return v
 
-        instance = cls()
+        instance = UserWriteOrganization.construct()
         error_messages = []
         # validate data type: OrganizationWrite
-        if type(v) is not OrganizationWrite:
+        if not isinstance(v, OrganizationWrite):
             error_messages.append(f"Error! Input type `{type(v)}` is not `OrganizationWrite`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into UserWriteOrganization with anyOf schemas: OrganizationWrite. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in UserWriteOrganization with anyOf schemas: OrganizationWrite. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> UserWriteOrganization:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> UserWriteOrganization:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = UserWriteOrganization.construct()
         if json_str is None:
             return instance
 
         error_messages = []
         # anyof_schema_1_validator: Optional[OrganizationWrite] = None
         try:
             instance.actual_instance = OrganizationWrite.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into UserWriteOrganization with anyOf schemas: OrganizationWrite. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/view.py` & `tpdk-2.0.7/tpdk/models/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
@@ -29,18 +28,20 @@
     """
     id: Optional[StrictInt] = None
     ip_address: StrictStr = Field(..., alias="ipAddress")
     offer: Optional[StrictStr] = None
     dispute: Optional[StrictStr] = None
     persona: Optional[StrictStr] = None
     user: Optional[StrictStr] = None
+    hit_count: StrictInt = Field(..., alias="hitCount")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
-    __properties = ["id", "ipAddress", "offer", "dispute", "persona", "user", "createdAt"]
+    __properties = ["id", "ipAddress", "offer", "dispute", "persona", "user", "hitCount", "createdAt"]
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -85,21 +86,22 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> View:
         """Create an instance of View from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return View.parse_obj(obj)
 
         _obj = View.parse_obj({
             "id": obj.get("id"),
             "ip_address": obj.get("ipAddress"),
             "offer": obj.get("offer"),
             "dispute": obj.get("dispute"),
             "persona": obj.get("persona"),
             "user": obj.get("user"),
+            "hit_count": obj.get("hitCount") if obj.get("hitCount") is not None else 1,
             "created_at": obj.get("createdAt")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook.py` & `tpdk-2.0.7/tpdk/models/webhook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
@@ -33,22 +32,25 @@
     object_id: Optional[StrictStr] = Field(None, alias="objectId")
     iri: Optional[StrictStr] = None
     occurred_at: Optional[datetime] = Field(None, alias="occurredAt")
     object: Optional[WebhookObject] = None
     __properties = ["id", "event", "objectId", "iri", "occurredAt", "object"]
 
     @validator('event')
-    def event_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
-            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
-        return v
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
+            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -74,15 +76,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> Webhook:
         """Create an instance of Webhook from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return Webhook.parse_obj(obj)
 
         _obj = Webhook.parse_obj({
             "id": obj.get("id"),
             "event": obj.get("event"),
             "object_id": obj.get("objectId"),
             "iri": obj.get("iri"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook_history_collection_read.py` & `tpdk-2.0.7/tpdk/models/webhook_history_collection_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
 
 class WebhookHistoryCollectionRead(BaseModel):
     """
     
     """
-    event: StrictStr = ...
+    event: StrictStr = Field(...)
     response_code: StrictInt = Field(..., alias="responseCode")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     attempted_at: Optional[datetime] = Field(None, alias="attemptedAt")
     retry_count: StrictInt = Field(..., alias="retryCount")
     __properties = ["event", "responseCode", "createdAt", "attemptedAt", "retryCount"]
 
     @validator('event')
-    def event_validate_enum(cls, v):
-        if v not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
-            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
-        return v
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
+            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -69,15 +70,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> WebhookHistoryCollectionRead:
         """Create an instance of WebhookHistoryCollectionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return WebhookHistoryCollectionRead.parse_obj(obj)
 
         _obj = WebhookHistoryCollectionRead.parse_obj({
             "event": obj.get("event"),
             "response_code": obj.get("responseCode"),
             "created_at": obj.get("createdAt"),
             "attempted_at": obj.get("attemptedAt"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook_history_read.py` & `tpdk-2.0.7/tpdk/models/webhook_history_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
 
 class WebhookHistoryRead(BaseModel):
     """
     
     """
-    event: StrictStr = ...
-    url: StrictStr = ...
+    event: StrictStr = Field(...)
+    url: StrictStr = Field(...)
     response_code: StrictInt = Field(..., alias="responseCode")
     response_body: StrictStr = Field(..., alias="responseBody")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     attempted_at: Optional[datetime] = Field(None, alias="attemptedAt")
     retry_count: StrictInt = Field(..., alias="retryCount")
     __properties = ["event", "url", "responseCode", "responseBody", "createdAt", "attemptedAt", "retryCount"]
 
     @validator('event')
-    def event_validate_enum(cls, v):
-        if v not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
-            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
-        return v
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
+            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -71,15 +72,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> WebhookHistoryRead:
         """Create an instance of WebhookHistoryRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return WebhookHistoryRead.parse_obj(obj)
 
         _obj = WebhookHistoryRead.parse_obj({
             "event": obj.get("event"),
             "url": obj.get("url"),
             "response_code": obj.get("responseCode"),
             "response_body": obj.get("responseBody"),
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook_object.py` & `tpdk-2.0.7/tpdk/models/webhook_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -42,87 +42,105 @@
     anyof_schema_3_validator: Optional[OfferRead] = None
     actual_instance: Any
     any_of_schemas: List[str] = Field(WEBHOOKOBJECT_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
+    def __init__(self, *args, **kwargs):
+        if args:
+            if len(args) > 1:
+                raise ValueError("If a position argument is used, only 1 is allowed to set `actual_instance`")
+            if kwargs:
+                raise ValueError("If a position argument is used, keyword arguments cannot be used.")
+            super().__init__(actual_instance=args[0])
+        else:
+            super().__init__(**kwargs)
+
     @validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = cls()
+        instance = WebhookObject.construct()
         error_messages = []
         # validate data type: DisputeRead
-        if type(v) is not DisputeRead:
+        if not isinstance(v, DisputeRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `DisputeRead`")
         else:
             return v
 
         # validate data type: PersonaRead
-        if type(v) is not PersonaRead:
+        if not isinstance(v, PersonaRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `PersonaRead`")
         else:
             return v
 
         # validate data type: OfferRead
-        if type(v) is not OfferRead:
+        if not isinstance(v, OfferRead):
             error_messages.append(f"Error! Input type `{type(v)}` is not `OfferRead`")
         else:
             return v
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into WebhookObject with anyOf schemas: DisputeRead, OfferRead, PersonaRead. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in WebhookObject with anyOf schemas: DisputeRead, OfferRead, PersonaRead. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> WebhookObject:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> WebhookObject:
         """Returns the object represented by the json string"""
-        instance = cls()
+        instance = WebhookObject.construct()
         error_messages = []
         # anyof_schema_1_validator: Optional[DisputeRead] = None
         try:
             instance.actual_instance = DisputeRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # anyof_schema_2_validator: Optional[PersonaRead] = None
         try:
             instance.actual_instance = PersonaRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # anyof_schema_3_validator: Optional[OfferRead] = None
         try:
             instance.actual_instance = OfferRead.from_json(json_str)
             return instance
-        except ValidationError as e:
+        except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
 
         if error_messages:
             # no match
             raise ValueError("No match found when deserializing the JSON string into WebhookObject with anyOf schemas: DisputeRead, OfferRead, PersonaRead. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_json()
         else:
-            return "null"
+            return json.dumps(self.actual_instance)
 
     def to_dict(self) -> dict:
         """Returns the dict representation of the actual instance"""
-        if self.actual_instance is not None:
+        if self.actual_instance is None:
+            return "null"
+
+        to_json = getattr(self.actual_instance, "to_json", None)
+        if callable(to_json):
             return self.actual_instance.to_dict()
         else:
-            return dict()
+            return json.dumps(self.actual_instance)
 
     def to_str(self) -> str:
         """Returns the string representation of the actual instance"""
         return pprint.pformat(self.dict())
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook_subscription_read.py` & `tpdk-2.0.7/tpdk/models/webhook_subscription_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, constr, validator
 
 class WebhookSubscriptionRead(BaseModel):
     """
     
     """
-    event: StrictStr = ...
+    event: StrictStr = Field(...)
     callback_url: constr(strict=True, max_length=5000, min_length=4) = Field(..., alias="callbackUrl")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     __properties = ["event", "callbackUrl", "createdAt"]
 
     @validator('event')
-    def event_validate_enum(cls, v):
-        if v not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
-            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
-        return v
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
+            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -66,15 +67,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> WebhookSubscriptionRead:
         """Create an instance of WebhookSubscriptionRead from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return WebhookSubscriptionRead.parse_obj(obj)
 
         _obj = WebhookSubscriptionRead.parse_obj({
             "event": obj.get("event"),
             "callback_url": obj.get("callbackUrl"),
             "created_at": obj.get("createdAt")
         })
```

### Comparing `tpdk-2.0.0b2/tpdk/models/webhook_subscription_write.py` & `tpdk-2.0.7/tpdk/models/webhook_subscription_write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
-from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr, constr, validator
 
 class WebhookSubscriptionWrite(BaseModel):
     """
     
     """
-    event: StrictStr = ...
+    event: StrictStr = Field(...)
     callback_url: constr(strict=True, max_length=5000, min_length=4) = Field(..., alias="callbackUrl")
     __properties = ["event", "callbackUrl"]
 
     @validator('event')
-    def event_validate_enum(cls, v):
-        if v not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
-            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
-        return v
+    def event_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added'):
+            raise ValueError("must be one of enum values ('dispute.opened', 'dispute.submitted', 'dispute.created', 'dispute.abandoned', 'dispute.settlement', 'dispute.closed', 'dispute.expired', 'dispute.manual_arbitration_required', 'dispute.updated', 'offer.created', 'offer.expired', 'offer.updated', 'offer.crawl_failure', 'offer.transaction.authorized', 'offer.transaction.reconciled', 'offer.transaction.abandoned', 'offer.closed', 'offer.transaction.refund', 'persona.added')")
+        return value
 
     class Config:
+        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
@@ -64,15 +65,15 @@
 
     @classmethod
     def from_dict(cls, obj: dict) -> WebhookSubscriptionWrite:
         """Create an instance of WebhookSubscriptionWrite from a dict"""
         if obj is None:
             return None
 
-        if type(obj) is not dict:
+        if not isinstance(obj, dict):
             return WebhookSubscriptionWrite.parse_obj(obj)
 
         _obj = WebhookSubscriptionWrite.parse_obj({
             "event": obj.get("event"),
             "callback_url": obj.get("callbackUrl")
         })
         return _obj
```

### Comparing `tpdk-2.0.0b2/tpdk/rest.py` & `tpdk-2.0.7/tpdk/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0-b2
+    The version of the OpenAPI document: 2.0.7
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -63,14 +63,18 @@
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args['server_hostname'] = configuration.tls_server_name
+
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
```

### Comparing `tpdk-2.0.0b2/tpdk.egg-info/SOURCES.txt` & `tpdk-2.0.7/tpdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 setup.cfg
 setup.py
 test/test_address.py
 test/test_address_independent_write.py
 test/test_address_read.py
 test/test_address_update.py
 test/test_address_write.py
+test/test_ai_api.py
+test/test_ai_hint.py
 test/test_api_client.py
 test/test_branding_api.py
 test/test_dispute.py
 test/test_dispute_collection_read.py
 test/test_dispute_independent_write.py
 test/test_dispute_post_creation_read.py
 test/test_dispute_read.py
@@ -54,26 +56,27 @@
 test/test_parcel_write.py
 test/test_persona.py
 test/test_persona_address.py
 test/test_persona_api.py
 test/test_persona_collection_read.py
 test/test_persona_independent_write.py
 test/test_persona_independent_write_address.py
+test/test_persona_persona_auth_return.py
+test/test_persona_persona_external_auth.py
 test/test_persona_post_auth_read.py
 test/test_persona_read.py
 test/test_persona_read_address.py
 test/test_persona_register.py
 test/test_persona_token.py
 test/test_persona_update.py
 test/test_persona_update_address.py
 test/test_persona_write.py
 test/test_persona_write_address.py
 test/test_resolution_center_api.py
 test/test_safe_checkout_api.py
-test/test_transaction_api.py
 test/test_transaction_collection_read.py
 test/test_transaction_independent_write.py
 test/test_transaction_read.py
 test/test_unprocessable_entity.py
 test/test_unprocessable_entity_violations_inner.py
 test/test_user.py
 test/test_user_api.py
@@ -89,37 +92,39 @@
 test/test_webhook_history_collection_read.py
 test/test_webhook_history_read.py
 test/test_webhook_object.py
 test/test_webhook_subscription_read.py
 test/test_webhook_subscription_write.py
 tpdk/__init__.py
 tpdk/api_client.py
+tpdk/api_response.py
 tpdk/configuration.py
 tpdk/exceptions.py
 tpdk/rest.py
 tpdk.egg-info/PKG-INFO
 tpdk.egg-info/SOURCES.txt
 tpdk.egg-info/dependency_links.txt
 tpdk.egg-info/requires.txt
 tpdk.egg-info/top_level.txt
 tpdk/api/__init__.py
+tpdk/api/ai_api.py
 tpdk/api/branding_api.py
 tpdk/api/notification_api.py
 tpdk/api/persona_api.py
 tpdk/api/resolution_center_api.py
 tpdk/api/safe_checkout_api.py
-tpdk/api/transaction_api.py
 tpdk/api/user_api.py
 tpdk/api/webhook_api.py
 tpdk/models/__init__.py
 tpdk/models/address.py
 tpdk/models/address_independent_write.py
 tpdk/models/address_read.py
 tpdk/models/address_update.py
 tpdk/models/address_write.py
+tpdk/models/ai_hint.py
 tpdk/models/api_client.py
 tpdk/models/dispute.py
 tpdk/models/dispute_collection_read.py
 tpdk/models/dispute_independent_write.py
 tpdk/models/dispute_post_creation_read.py
 tpdk/models/dispute_read.py
 tpdk/models/dispute_update.py
@@ -160,14 +165,16 @@
 tpdk/models/parcel_read.py
 tpdk/models/parcel_write.py
 tpdk/models/persona.py
 tpdk/models/persona_address.py
 tpdk/models/persona_collection_read.py
 tpdk/models/persona_independent_write.py
 tpdk/models/persona_independent_write_address.py
+tpdk/models/persona_persona_auth_return.py
+tpdk/models/persona_persona_external_auth.py
 tpdk/models/persona_post_auth_read.py
 tpdk/models/persona_read.py
 tpdk/models/persona_read_address.py
 tpdk/models/persona_register.py
 tpdk/models/persona_token.py
 tpdk/models/persona_update.py
 tpdk/models/persona_update_address.py
```

