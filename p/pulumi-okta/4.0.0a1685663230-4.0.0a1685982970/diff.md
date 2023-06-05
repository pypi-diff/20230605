# Comparing `tmp/pulumi_okta-4.0.0a1685663230.tar.gz` & `tmp/pulumi_okta-4.0.0a1685982970.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.0.0a1685663230.tar", last modified: Thu Jun  1 23:51:45 2023, max compression
+gzip compressed data, was "pulumi_okta-4.0.0a1685982970.tar", last modified: Mon Jun  5 16:40:46 2023, max compression
```

## Comparing `pulumi_okta-4.0.0a1685663230.tar` & `pulumi_okta-4.0.0a1685982970.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.043952 pulumi_okta-4.0.0a1685663230/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    29940 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)   137739 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/index/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.047952 pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24327 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31644 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95272 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:51:45.043952 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 23:51:45.000000 pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:51:45.051952 pulumi_okta-4.0.0a1685663230/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 23:51:44.000000 pulumi_okta-4.0.0a1685663230/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.892260 pulumi_okta-4.0.0a1685982970/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.892260 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137739 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/index/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.896260 pulumi_okta-4.0.0a1685982970/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24327 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:40:46.892260 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:40:46.900260 pulumi_okta-4.0.0a1685982970/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-05 16:40:46.000000 pulumi_okta-4.0.0a1685982970/setup.py
```

### Comparing `pulumi_okta-4.0.0a1685663230/PKG-INFO` & `pulumi_okta-4.0.0a1685982970/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.0.0a1685663230
+Version: 4.0.0a1685982970
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.0.0a1685663230/README.md` & `pulumi_okta-4.0.0a1685982970/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/__init__.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/_utilities.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/__init__.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_app.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_app.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetAppResult:
     """
     A collection of values returned by getApp.
     """
-    def __init__(__self__, active_only=None, groups=None, id=None, label=None, label_prefix=None, links=None, name=None, status=None, users=None):
+    def __init__(__self__, active_only=None, groups=None, id=None, label=None, label_prefix=None, links=None, name=None, skip_groups=None, skip_users=None, status=None, users=None):
         if active_only and not isinstance(active_only, bool):
             raise TypeError("Expected argument 'active_only' to be a bool")
         pulumi.set(__self__, "active_only", active_only)
         if groups and not isinstance(groups, list):
             raise TypeError("Expected argument 'groups' to be a list")
         if groups is not None:
             warnings.warn("""The `groups` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_group_assignments`""", DeprecationWarning)
@@ -43,14 +43,28 @@
         pulumi.set(__self__, "label_prefix", label_prefix)
         if links and not isinstance(links, str):
             raise TypeError("Expected argument 'links' to be a str")
         pulumi.set(__self__, "links", links)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
+        if skip_groups and not isinstance(skip_groups, bool):
+            raise TypeError("Expected argument 'skip_groups' to be a bool")
+        if skip_groups is not None:
+            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_groups", skip_groups)
+        if skip_users and not isinstance(skip_users, bool):
+            raise TypeError("Expected argument 'skip_users' to be a bool")
+        if skip_users is not None:
+            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_users", skip_users)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if users and not isinstance(users, list):
             raise TypeError("Expected argument 'users' to be a list")
         if users is not None:
             warnings.warn("""The `users` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_user_assignments`""", DeprecationWarning)
@@ -102,14 +116,24 @@
     def name(self) -> str:
         """
         Application name.
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="skipGroups")
+    def skip_groups(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_groups")
+
+    @property
+    @pulumi.getter(name="skipUsers")
+    def skip_users(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_users")
+
+    @property
     @pulumi.getter
     def status(self) -> str:
         """
         Application status.
         """
         return pulumi.get(self, "status")
 
@@ -128,22 +152,26 @@
             active_only=self.active_only,
             groups=self.groups,
             id=self.id,
             label=self.label,
             label_prefix=self.label_prefix,
             links=self.links,
             name=self.name,
+            skip_groups=self.skip_groups,
+            skip_users=self.skip_users,
             status=self.status,
             users=self.users)
 
 
 def get_app(active_only: Optional[bool] = None,
             id: Optional[str] = None,
             label: Optional[str] = None,
             label_prefix: Optional[str] = None,
+            skip_groups: Optional[bool] = None,
+            skip_users: Optional[bool] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAppResult:
     """
     Use this data source to retrieve an application from Okta.
 
     ## Example Usage
 
     ```python
@@ -165,34 +193,40 @@
            provider to do a `starts with` query as opposed to an `equals` query.
     """
     __args__ = dict()
     __args__['activeOnly'] = active_only
     __args__['id'] = id
     __args__['label'] = label
     __args__['labelPrefix'] = label_prefix
+    __args__['skipGroups'] = skip_groups
+    __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getApp:getApp', __args__, opts=opts, typ=GetAppResult).value
 
     return AwaitableGetAppResult(
         active_only=__ret__.active_only,
         groups=__ret__.groups,
         id=__ret__.id,
         label=__ret__.label,
         label_prefix=__ret__.label_prefix,
         links=__ret__.links,
         name=__ret__.name,
+        skip_groups=__ret__.skip_groups,
+        skip_users=__ret__.skip_users,
         status=__ret__.status,
         users=__ret__.users)
 
 
 @_utilities.lift_output_func(get_app)
 def get_app_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                    id: Optional[pulumi.Input[Optional[str]]] = None,
                    label: Optional[pulumi.Input[Optional[str]]] = None,
                    label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
+                   skip_groups: Optional[pulumi.Input[Optional[bool]]] = None,
+                   skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppResult]:
     """
     Use this data source to retrieve an application from Okta.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_oauth.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetOauthResult:
     """
     A collection of values returned by getOauth.
     """
-    def __init__(__self__, active_only=None, auto_submit_toolbar=None, client_id=None, client_secret=None, client_uri=None, grant_types=None, hide_ios=None, hide_web=None, id=None, label=None, label_prefix=None, links=None, login_mode=None, login_scopes=None, login_uri=None, logo_uri=None, name=None, policy_uri=None, post_logout_redirect_uris=None, redirect_uris=None, response_types=None, status=None, type=None, wildcard_redirect=None):
+    def __init__(__self__, active_only=None, auto_submit_toolbar=None, client_id=None, client_secret=None, client_uri=None, grant_types=None, hide_ios=None, hide_web=None, id=None, label=None, label_prefix=None, links=None, login_mode=None, login_scopes=None, login_uri=None, logo_uri=None, name=None, policy_uri=None, post_logout_redirect_uris=None, redirect_uris=None, response_types=None, skip_groups=None, skip_users=None, status=None, type=None, wildcard_redirect=None):
         if active_only and not isinstance(active_only, bool):
             raise TypeError("Expected argument 'active_only' to be a bool")
         pulumi.set(__self__, "active_only", active_only)
         if auto_submit_toolbar and not isinstance(auto_submit_toolbar, bool):
             raise TypeError("Expected argument 'auto_submit_toolbar' to be a bool")
         pulumi.set(__self__, "auto_submit_toolbar", auto_submit_toolbar)
         if client_id and not isinstance(client_id, str):
@@ -81,14 +81,28 @@
         pulumi.set(__self__, "post_logout_redirect_uris", post_logout_redirect_uris)
         if redirect_uris and not isinstance(redirect_uris, list):
             raise TypeError("Expected argument 'redirect_uris' to be a list")
         pulumi.set(__self__, "redirect_uris", redirect_uris)
         if response_types and not isinstance(response_types, list):
             raise TypeError("Expected argument 'response_types' to be a list")
         pulumi.set(__self__, "response_types", response_types)
+        if skip_groups and not isinstance(skip_groups, bool):
+            raise TypeError("Expected argument 'skip_groups' to be a bool")
+        if skip_groups is not None:
+            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_groups", skip_groups)
+        if skip_users and not isinstance(skip_users, bool):
+            raise TypeError("Expected argument 'skip_users' to be a bool")
+        if skip_users is not None:
+            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_users", skip_users)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if wildcard_redirect and not isinstance(wildcard_redirect, str):
@@ -254,14 +268,24 @@
     def response_types(self) -> Sequence[str]:
         """
         List of OAuth 2.0 response type strings.
         """
         return pulumi.get(self, "response_types")
 
     @property
+    @pulumi.getter(name="skipGroups")
+    def skip_groups(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_groups")
+
+    @property
+    @pulumi.getter(name="skipUsers")
+    def skip_users(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_users")
+
+    @property
     @pulumi.getter
     def status(self) -> str:
         """
         Status of application.
         """
         return pulumi.get(self, "status")
 
@@ -302,23 +326,27 @@
             login_uri=self.login_uri,
             logo_uri=self.logo_uri,
             name=self.name,
             policy_uri=self.policy_uri,
             post_logout_redirect_uris=self.post_logout_redirect_uris,
             redirect_uris=self.redirect_uris,
             response_types=self.response_types,
+            skip_groups=self.skip_groups,
+            skip_users=self.skip_users,
             status=self.status,
             type=self.type,
             wildcard_redirect=self.wildcard_redirect)
 
 
 def get_oauth(active_only: Optional[bool] = None,
               id: Optional[str] = None,
               label: Optional[str] = None,
               label_prefix: Optional[str] = None,
+              skip_groups: Optional[bool] = None,
+              skip_users: Optional[bool] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOauthResult:
     """
     Use this data source to retrieve an OIDC application from Okta.
 
     ## Example Usage
 
     ```python
@@ -342,14 +370,16 @@
            provider to do a `starts with` query as opposed to an `equals` query.
     """
     __args__ = dict()
     __args__['activeOnly'] = active_only
     __args__['id'] = id
     __args__['label'] = label
     __args__['labelPrefix'] = label_prefix
+    __args__['skipGroups'] = skip_groups
+    __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getOauth:getOauth', __args__, opts=opts, typ=GetOauthResult).value
 
     return AwaitableGetOauthResult(
         active_only=__ret__.active_only,
         auto_submit_toolbar=__ret__.auto_submit_toolbar,
         client_id=__ret__.client_id,
@@ -367,24 +397,28 @@
         login_uri=__ret__.login_uri,
         logo_uri=__ret__.logo_uri,
         name=__ret__.name,
         policy_uri=__ret__.policy_uri,
         post_logout_redirect_uris=__ret__.post_logout_redirect_uris,
         redirect_uris=__ret__.redirect_uris,
         response_types=__ret__.response_types,
+        skip_groups=__ret__.skip_groups,
+        skip_users=__ret__.skip_users,
         status=__ret__.status,
         type=__ret__.type,
         wildcard_redirect=__ret__.wildcard_redirect)
 
 
 @_utilities.lift_output_func(get_oauth)
 def get_oauth_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                      id: Optional[pulumi.Input[Optional[str]]] = None,
                      label: Optional[pulumi.Input[Optional[str]]] = None,
                      label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
+                     skip_groups: Optional[pulumi.Input[Optional[bool]]] = None,
+                     skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOauthResult]:
     """
     Use this data source to retrieve an OIDC application from Okta.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/get_saml.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetSamlResult:
     """
     A collection of values returned by getSaml.
     """
-    def __init__(__self__, accessibility_error_redirect_url=None, accessibility_login_redirect_url=None, accessibility_self_service=None, acs_endpoints=None, active_only=None, app_settings_json=None, assertion_signed=None, attribute_statements=None, audience=None, authn_context_class_ref=None, auto_submit_toolbar=None, default_relay_state=None, destination=None, digest_algorithm=None, features=None, groups=None, hide_ios=None, hide_web=None, honor_force_authn=None, id=None, idp_issuer=None, inline_hook_id=None, key_id=None, label=None, label_prefix=None, links=None, name=None, recipient=None, request_compressed=None, response_signed=None, saml_signed_request_enabled=None, signature_algorithm=None, single_logout_certificate=None, single_logout_issuer=None, single_logout_url=None, sp_issuer=None, sso_url=None, status=None, subject_name_id_format=None, subject_name_id_template=None, user_name_template=None, user_name_template_push_status=None, user_name_template_suffix=None, user_name_template_type=None, users=None):
+    def __init__(__self__, accessibility_error_redirect_url=None, accessibility_login_redirect_url=None, accessibility_self_service=None, acs_endpoints=None, active_only=None, app_settings_json=None, assertion_signed=None, attribute_statements=None, audience=None, authn_context_class_ref=None, auto_submit_toolbar=None, default_relay_state=None, destination=None, digest_algorithm=None, features=None, groups=None, hide_ios=None, hide_web=None, honor_force_authn=None, id=None, idp_issuer=None, inline_hook_id=None, key_id=None, label=None, label_prefix=None, links=None, name=None, recipient=None, request_compressed=None, response_signed=None, saml_signed_request_enabled=None, signature_algorithm=None, single_logout_certificate=None, single_logout_issuer=None, single_logout_url=None, skip_groups=None, skip_users=None, sp_issuer=None, sso_url=None, status=None, subject_name_id_format=None, subject_name_id_template=None, user_name_template=None, user_name_template_push_status=None, user_name_template_suffix=None, user_name_template_type=None, users=None):
         if accessibility_error_redirect_url and not isinstance(accessibility_error_redirect_url, str):
             raise TypeError("Expected argument 'accessibility_error_redirect_url' to be a str")
         pulumi.set(__self__, "accessibility_error_redirect_url", accessibility_error_redirect_url)
         if accessibility_login_redirect_url and not isinstance(accessibility_login_redirect_url, str):
             raise TypeError("Expected argument 'accessibility_login_redirect_url' to be a str")
         pulumi.set(__self__, "accessibility_login_redirect_url", accessibility_login_redirect_url)
         if accessibility_self_service and not isinstance(accessibility_self_service, bool):
@@ -128,14 +128,28 @@
         pulumi.set(__self__, "single_logout_certificate", single_logout_certificate)
         if single_logout_issuer and not isinstance(single_logout_issuer, str):
             raise TypeError("Expected argument 'single_logout_issuer' to be a str")
         pulumi.set(__self__, "single_logout_issuer", single_logout_issuer)
         if single_logout_url and not isinstance(single_logout_url, str):
             raise TypeError("Expected argument 'single_logout_url' to be a str")
         pulumi.set(__self__, "single_logout_url", single_logout_url)
+        if skip_groups and not isinstance(skip_groups, bool):
+            raise TypeError("Expected argument 'skip_groups' to be a bool")
+        if skip_groups is not None:
+            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_groups", skip_groups)
+        if skip_users and not isinstance(skip_users, bool):
+            raise TypeError("Expected argument 'skip_users' to be a bool")
+        if skip_users is not None:
+            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
+        pulumi.set(__self__, "skip_users", skip_users)
         if sp_issuer and not isinstance(sp_issuer, str):
             raise TypeError("Expected argument 'sp_issuer' to be a str")
         pulumi.set(__self__, "sp_issuer", sp_issuer)
         if sso_url and not isinstance(sso_url, str):
             raise TypeError("Expected argument 'sso_url' to be a str")
         pulumi.set(__self__, "sso_url", sso_url)
         if status and not isinstance(status, str):
@@ -438,14 +452,24 @@
     def single_logout_url(self) -> str:
         """
         The location where the logout response is sent.
         """
         return pulumi.get(self, "single_logout_url")
 
     @property
+    @pulumi.getter(name="skipGroups")
+    def skip_groups(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_groups")
+
+    @property
+    @pulumi.getter(name="skipUsers")
+    def skip_users(self) -> Optional[bool]:
+        return pulumi.get(self, "skip_users")
+
+    @property
     @pulumi.getter(name="spIssuer")
     def sp_issuer(self) -> str:
         """
         SAML service provider issuer.
         """
         return pulumi.get(self, "sp_issuer")
 
@@ -556,14 +580,16 @@
             request_compressed=self.request_compressed,
             response_signed=self.response_signed,
             saml_signed_request_enabled=self.saml_signed_request_enabled,
             signature_algorithm=self.signature_algorithm,
             single_logout_certificate=self.single_logout_certificate,
             single_logout_issuer=self.single_logout_issuer,
             single_logout_url=self.single_logout_url,
+            skip_groups=self.skip_groups,
+            skip_users=self.skip_users,
             sp_issuer=self.sp_issuer,
             sso_url=self.sso_url,
             status=self.status,
             subject_name_id_format=self.subject_name_id_format,
             subject_name_id_template=self.subject_name_id_template,
             user_name_template=self.user_name_template,
             user_name_template_push_status=self.user_name_template_push_status,
@@ -573,14 +599,16 @@
 
 
 def get_saml(active_only: Optional[bool] = None,
              id: Optional[str] = None,
              label: Optional[str] = None,
              label_prefix: Optional[str] = None,
              request_compressed: Optional[bool] = None,
+             skip_groups: Optional[bool] = None,
+             skip_users: Optional[bool] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSamlResult:
     """
     Use this data source to retrieve an SAML application from Okta.
 
     ## Example Usage
 
     ```python
@@ -602,14 +630,16 @@
     """
     __args__ = dict()
     __args__['activeOnly'] = active_only
     __args__['id'] = id
     __args__['label'] = label
     __args__['labelPrefix'] = label_prefix
     __args__['requestCompressed'] = request_compressed
+    __args__['skipGroups'] = skip_groups
+    __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getSaml:getSaml', __args__, opts=opts, typ=GetSamlResult).value
 
     return AwaitableGetSamlResult(
         accessibility_error_redirect_url=__ret__.accessibility_error_redirect_url,
         accessibility_login_redirect_url=__ret__.accessibility_login_redirect_url,
         accessibility_self_service=__ret__.accessibility_self_service,
@@ -641,14 +671,16 @@
         request_compressed=__ret__.request_compressed,
         response_signed=__ret__.response_signed,
         saml_signed_request_enabled=__ret__.saml_signed_request_enabled,
         signature_algorithm=__ret__.signature_algorithm,
         single_logout_certificate=__ret__.single_logout_certificate,
         single_logout_issuer=__ret__.single_logout_issuer,
         single_logout_url=__ret__.single_logout_url,
+        skip_groups=__ret__.skip_groups,
+        skip_users=__ret__.skip_users,
         sp_issuer=__ret__.sp_issuer,
         sso_url=__ret__.sso_url,
         status=__ret__.status,
         subject_name_id_format=__ret__.subject_name_id_format,
         subject_name_id_template=__ret__.subject_name_id_template,
         user_name_template=__ret__.user_name_template,
         user_name_template_push_status=__ret__.user_name_template_push_status,
@@ -659,14 +691,16 @@
 
 @_utilities.lift_output_func(get_saml)
 def get_saml_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                     id: Optional[pulumi.Input[Optional[str]]] = None,
                     label: Optional[pulumi.Input[Optional[str]]] = None,
                     label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
                     request_compressed: Optional[pulumi.Input[Optional[bool]]] = None,
+                    skip_groups: Optional[pulumi.Input[Optional[bool]]] = None,
+                    skip_users: Optional[pulumi.Input[Optional[bool]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSamlResult]:
     """
     Use this data source to retrieve an SAML application from Okta.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/swa.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/three_field.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app/user.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/authenticator.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/behaviour.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/brand.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/captcha.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/config/vars.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/domain.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/domain_verification.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/email_customization.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/email_sender.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/event_hook.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/factor/factor.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/factor_totp.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_group_assignments.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_group_assignments(id=okta_app_oauth["test"]["id"])
+    test = okta.get_app_group_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -91,14 +91,14 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_group_assignments(id=okta_app_oauth["test"]["id"])
+    test = okta.get_app_group_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_app_user_assignments.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_user_assignments(id=okta_app_oauth["test"]["id"])
+    test = okta.get_app_user_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -91,14 +91,14 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_user_assignments(id=okta_app_oauth["test"]["id"])
+    test = okta.get_app_user_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_brand.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_brands.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_groups.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_template.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_templates.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_theme.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_themes.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group/get_group.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group/group.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/signon.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,303 +5,373 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['GroupArgs', 'Group']
+__all__ = ['SignonArgs', 'Signon']
 
 @pulumi.input_type
-class GroupArgs:
+class SignonArgs:
     def __init__(__self__, *,
-                 custom_profile_attributes: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Group resource.
-        :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[str] description: The description of the Okta Group.
-        :param pulumi.Input[str] name: The name of the Okta Group.
+        The set of arguments for constructing a Signon resource.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        if custom_profile_attributes is not None:
-            pulumi.set(__self__, "custom_profile_attributes", custom_profile_attributes)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if groups_includeds is not None:
+            pulumi.set(__self__, "groups_includeds", groups_includeds)
         if name is not None:
             pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter(name="customProfileAttributes")
-    def custom_profile_attributes(self) -> Optional[pulumi.Input[str]]:
-        """
-        raw JSON containing all custom profile attributes.
-        """
-        return pulumi.get(self, "custom_profile_attributes")
-
-    @custom_profile_attributes.setter
-    def custom_profile_attributes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "custom_profile_attributes", value)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The description of the Okta Group.
+        Policy Description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of Group IDs to Include.
+        """
+        return pulumi.get(self, "groups_includeds")
+
+    @groups_includeds.setter
+    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "groups_includeds", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Okta Group.
+        Policy Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter
+    def priority(self) -> Optional[pulumi.Input[int]]:
+        """
+        Priority of the policy.
+        """
+        return pulumi.get(self, "priority")
+
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
 
 @pulumi.input_type
-class _GroupState:
+class _SignonState:
     def __init__(__self__, *,
-                 custom_profile_attributes: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None):
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Group resources.
-        :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[str] description: The description of the Okta Group.
-        :param pulumi.Input[str] name: The name of the Okta Group.
+        Input properties used for looking up and filtering Signon resources.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
-        if custom_profile_attributes is not None:
-            pulumi.set(__self__, "custom_profile_attributes", custom_profile_attributes)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if groups_includeds is not None:
+            pulumi.set(__self__, "groups_includeds", groups_includeds)
         if name is not None:
             pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter(name="customProfileAttributes")
-    def custom_profile_attributes(self) -> Optional[pulumi.Input[str]]:
-        """
-        raw JSON containing all custom profile attributes.
-        """
-        return pulumi.get(self, "custom_profile_attributes")
-
-    @custom_profile_attributes.setter
-    def custom_profile_attributes(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "custom_profile_attributes", value)
+        if priority is not None:
+            pulumi.set(__self__, "priority", priority)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The description of the Okta Group.
+        Policy Description.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of Group IDs to Include.
+        """
+        return pulumi.get(self, "groups_includeds")
+
+    @groups_includeds.setter
+    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "groups_includeds", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Okta Group.
+        Policy Name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
+    @property
+    @pulumi.getter
+    def priority(self) -> Optional[pulumi.Input[int]]:
+        """
+        Priority of the policy.
+        """
+        return pulumi.get(self, "priority")
+
+    @priority.setter
+    def priority(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "priority", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
-class Group(pulumi.CustomResource):
+
+class Signon(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 custom_profile_attributes: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates an Okta Group.
+        Creates a Sign On Policy.
 
-        This resource allows you to create and configure an Okta Group.
+        This resource allows you to create and configure a Sign On Policy.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.group.Group("example", description="My Example Group")
-        ```
-
-        Custom profile attributes
-        ```python
-        import pulumi
-        import json
-        import pulumi_okta as okta
-
-        example = okta.group.Group("example",
-            description="My Example Group",
-            custom_profile_attributes=json.dumps({
-                "example1": "testing1234",
-                "example2": True,
-                "example3": 54321,
-            }))
+        example = okta.policy.Signon("example",
+            description="Example",
+            groups_includeds=[data["okta_group"]["everyone"]["id"]],
+            status="ACTIVE")
         ```
 
         ## Import
 
-        An Okta Group can be imported via the Okta ID.
+        A Sign On Policy can be imported via the Okta ID.
 
         ```sh
-         $ pulumi import okta:group/group:Group example &#60;group id&#62;
+         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[str] description: The description of the Okta Group.
-        :param pulumi.Input[str] name: The name of the Okta Group.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[GroupArgs] = None,
+                 args: Optional[SignonArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates an Okta Group.
+        Creates a Sign On Policy.
 
-        This resource allows you to create and configure an Okta Group.
+        This resource allows you to create and configure a Sign On Policy.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.group.Group("example", description="My Example Group")
-        ```
-
-        Custom profile attributes
-        ```python
-        import pulumi
-        import json
-        import pulumi_okta as okta
-
-        example = okta.group.Group("example",
-            description="My Example Group",
-            custom_profile_attributes=json.dumps({
-                "example1": "testing1234",
-                "example2": True,
-                "example3": 54321,
-            }))
+        example = okta.policy.Signon("example",
+            description="Example",
+            groups_includeds=[data["okta_group"]["everyone"]["id"]],
+            status="ACTIVE")
         ```
 
         ## Import
 
-        An Okta Group can be imported via the Okta ID.
+        A Sign On Policy can be imported via the Okta ID.
 
         ```sh
-         $ pulumi import okta:group/group:Group example &#60;group id&#62;
+         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
         ```
 
         :param str resource_name: The name of the resource.
-        :param GroupArgs args: The arguments to use to populate this resource's properties.
+        :param SignonArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GroupArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SignonArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 custom_profile_attributes: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 priority: Optional[pulumi.Input[int]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GroupArgs.__new__(GroupArgs)
+            __props__ = SignonArgs.__new__(SignonArgs)
 
-            __props__.__dict__["custom_profile_attributes"] = custom_profile_attributes
             __props__.__dict__["description"] = description
+            __props__.__dict__["groups_includeds"] = groups_includeds
             __props__.__dict__["name"] = name
-        super(Group, __self__).__init__(
-            'okta:group/group:Group',
+            __props__.__dict__["priority"] = priority
+            __props__.__dict__["status"] = status
+        super(Signon, __self__).__init__(
+            'okta:policy/signon:Signon',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            custom_profile_attributes: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None) -> 'Group':
+            groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            priority: Optional[pulumi.Input[int]] = None,
+            status: Optional[pulumi.Input[str]] = None) -> 'Signon':
         """
-        Get an existing Group resource's state with the given name, id, and optional extra
+        Get an existing Signon resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] custom_profile_attributes: raw JSON containing all custom profile attributes.
-        :param pulumi.Input[str] description: The description of the Okta Group.
-        :param pulumi.Input[str] name: The name of the Okta Group.
+        :param pulumi.Input[str] description: Policy Description.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
+        :param pulumi.Input[str] name: Policy Name.
+        :param pulumi.Input[int] priority: Priority of the policy.
+        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GroupState.__new__(_GroupState)
+        __props__ = _SignonState.__new__(_SignonState)
 
-        __props__.__dict__["custom_profile_attributes"] = custom_profile_attributes
         __props__.__dict__["description"] = description
+        __props__.__dict__["groups_includeds"] = groups_includeds
         __props__.__dict__["name"] = name
-        return Group(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["priority"] = priority
+        __props__.__dict__["status"] = status
+        return Signon(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="customProfileAttributes")
-    def custom_profile_attributes(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        raw JSON containing all custom profile attributes.
+        Policy Description.
         """
-        return pulumi.get(self, "custom_profile_attributes")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="groupsIncludeds")
+    def groups_includeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The description of the Okta Group.
+        List of Group IDs to Include.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "groups_includeds")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the Okta Group.
+        Policy Name.
         """
         return pulumi.get(self, "name")
 
+    @property
+    @pulumi.getter
+    def priority(self) -> pulumi.Output[Optional[int]]:
+        """
+        Priority of the policy.
+        """
+        return pulumi.get(self, "priority")
+
+    @property
+    @pulumi.getter
+    def status(self) -> pulumi.Output[Optional[str]]:
+        """
+        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        """
+        return pulumi.get(self, "status")
+
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group/role.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group/rule.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group_memberships.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/saml.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/idp/social.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/index/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/hook.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/link_definition.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/link_value.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/network/zone.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/org_configuration.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/org_support.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/password.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy/signon.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user_admin_roles.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,375 +3,304 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['SignonArgs', 'Signon']
+__all__ = ['UserAdminRolesArgs', 'UserAdminRoles']
 
 @pulumi.input_type
-class SignonArgs:
+class UserAdminRolesArgs:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a Signon resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
-        """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if groups_includeds is not None:
-            pulumi.set(__self__, "groups_includeds", groups_includeds)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if priority is not None:
-            pulumi.set(__self__, "priority", priority)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+                 admin_roles: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 user_id: pulumi.Input[str],
+                 disable_notifications: Optional[pulumi.Input[bool]] = None):
         """
-        Policy Description.
+        The set of arguments for constructing a UserAdminRoles resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[str] user_id: Okta user ID.
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+        pulumi.set(__self__, "admin_roles", admin_roles)
+        pulumi.set(__self__, "user_id", user_id)
+        if disable_notifications is not None:
+            pulumi.set(__self__, "disable_notifications", disable_notifications)
 
     @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        List of Group IDs to Include.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "groups_includeds")
+        return pulumi.get(self, "admin_roles")
 
-    @groups_includeds.setter
-    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "groups_includeds", value)
+    @admin_roles.setter
+    def admin_roles(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "admin_roles", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Input[str]:
         """
-        Policy Name.
+        Okta user ID.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "user_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @user_id.setter
+    def user_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_id", value)
 
     @property
-    @pulumi.getter
-    def priority(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> Optional[pulumi.Input[bool]]:
         """
-        Priority of the policy.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "priority")
-
-    @priority.setter
-    def priority(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "priority", value)
+        return pulumi.get(self, "disable_notifications")
 
-    @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
-        """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
-        """
-        return pulumi.get(self, "status")
-
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @disable_notifications.setter
+    def disable_notifications(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_notifications", value)
 
 
 @pulumi.input_type
-class _SignonState:
+class _UserAdminRolesState:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering Signon resources.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
-        """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if groups_includeds is not None:
-            pulumi.set(__self__, "groups_includeds", groups_includeds)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if priority is not None:
-            pulumi.set(__self__, "priority", priority)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-
-    @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        Policy Description.
-        """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None):
         """
-        List of Group IDs to Include.
+        Input properties used for looking up and filtering UserAdminRoles resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
-        return pulumi.get(self, "groups_includeds")
-
-    @groups_includeds.setter
-    def groups_includeds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "groups_includeds", value)
+        if admin_roles is not None:
+            pulumi.set(__self__, "admin_roles", admin_roles)
+        if disable_notifications is not None:
+            pulumi.set(__self__, "disable_notifications", disable_notifications)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Policy Name.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "admin_roles")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @admin_roles.setter
+    def admin_roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "admin_roles", value)
 
     @property
-    @pulumi.getter
-    def priority(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> Optional[pulumi.Input[bool]]:
         """
-        Priority of the policy.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "priority")
+        return pulumi.get(self, "disable_notifications")
 
-    @priority.setter
-    def priority(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "priority", value)
+    @disable_notifications.setter
+    def disable_notifications(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_notifications", value)
 
     @property
-    @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        Okta user ID.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "user_id")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
 
 
-class Signon(pulumi.CustomResource):
+class UserAdminRoles(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates a Sign On Policy.
+        Resource to manage a set of admin roles for a specific user.
+
+        This resource allows you to manage admin roles for a single user, independent of the user schema itself.
 
-        This resource allows you to create and configure a Sign On Policy.
+        When using this with a `user.User` resource, you should add a lifecycle ignore for admin roles to avoid conflicts
+        in desired state.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.policy.Signon("example",
-            description="Example",
-            groups_includeds=[data["okta_group"]["everyone"]["id"]],
-            status="ACTIVE")
+        test_user = okta.user.User("testUser",
+            first_name="TestAcc",
+            last_name="Smith",
+            login="testAcc-replace_with_uuid@example.com",
+            email="testAcc-replace_with_uuid@example.com")
+        test_user_admin_roles = okta.UserAdminRoles("testUserAdminRoles",
+            user_id=test_user.id,
+            admin_roles=["APP_ADMIN"])
         ```
 
         ## Import
 
-        A Sign On Policy can be imported via the Okta ID.
+        Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
-         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+         $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[SignonArgs] = None,
+                 args: UserAdminRolesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a Sign On Policy.
+        Resource to manage a set of admin roles for a specific user.
 
-        This resource allows you to create and configure a Sign On Policy.
+        This resource allows you to manage admin roles for a single user, independent of the user schema itself.
+
+        When using this with a `user.User` resource, you should add a lifecycle ignore for admin roles to avoid conflicts
+        in desired state.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.policy.Signon("example",
-            description="Example",
-            groups_includeds=[data["okta_group"]["everyone"]["id"]],
-            status="ACTIVE")
+        test_user = okta.user.User("testUser",
+            first_name="TestAcc",
+            last_name="Smith",
+            login="testAcc-replace_with_uuid@example.com",
+            email="testAcc-replace_with_uuid@example.com")
+        test_user_admin_roles = okta.UserAdminRoles("testUserAdminRoles",
+            user_id=test_user.id,
+            admin_roles=["APP_ADMIN"])
         ```
 
         ## Import
 
-        A Sign On Policy can be imported via the Okta ID.
+        Existing user admin roles can be imported via the Okta User ID.
 
         ```sh
-         $ pulumi import okta:policy/signon:Signon example &#60;policy id&#62;
+         $ pulumi import okta:index/userAdminRoles:UserAdminRoles example &#60;user id&#62;
         ```
 
         :param str resource_name: The name of the resource.
-        :param SignonArgs args: The arguments to use to populate this resource's properties.
+        :param UserAdminRolesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SignonArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserAdminRolesArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 priority: Optional[pulumi.Input[int]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
+                 admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 disable_notifications: Optional[pulumi.Input[bool]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SignonArgs.__new__(SignonArgs)
+            __props__ = UserAdminRolesArgs.__new__(UserAdminRolesArgs)
 
-            __props__.__dict__["description"] = description
-            __props__.__dict__["groups_includeds"] = groups_includeds
-            __props__.__dict__["name"] = name
-            __props__.__dict__["priority"] = priority
-            __props__.__dict__["status"] = status
-        super(Signon, __self__).__init__(
-            'okta:policy/signon:Signon',
+            if admin_roles is None and not opts.urn:
+                raise TypeError("Missing required property 'admin_roles'")
+            __props__.__dict__["admin_roles"] = admin_roles
+            __props__.__dict__["disable_notifications"] = disable_notifications
+            if user_id is None and not opts.urn:
+                raise TypeError("Missing required property 'user_id'")
+            __props__.__dict__["user_id"] = user_id
+        super(UserAdminRoles, __self__).__init__(
+            'okta:index/userAdminRoles:UserAdminRoles',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            groups_includeds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            priority: Optional[pulumi.Input[int]] = None,
-            status: Optional[pulumi.Input[str]] = None) -> 'Signon':
+            admin_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            disable_notifications: Optional[pulumi.Input[bool]] = None,
+            user_id: Optional[pulumi.Input[str]] = None) -> 'UserAdminRoles':
         """
-        Get an existing Signon resource's state with the given name, id, and optional extra
+        Get an existing UserAdminRoles resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Policy Description.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] groups_includeds: List of Group IDs to Include.
-        :param pulumi.Input[str] name: Policy Name.
-        :param pulumi.Input[int] priority: Priority of the policy.
-        :param pulumi.Input[str] status: Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] admin_roles: The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
+        :param pulumi.Input[bool] disable_notifications: When this setting is enabled, the admins won't receive any of the default Okta
+               administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
+        :param pulumi.Input[str] user_id: Okta user ID.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _SignonState.__new__(_SignonState)
-
-        __props__.__dict__["description"] = description
-        __props__.__dict__["groups_includeds"] = groups_includeds
-        __props__.__dict__["name"] = name
-        __props__.__dict__["priority"] = priority
-        __props__.__dict__["status"] = status
-        return Signon(resource_name, opts=opts, __props__=__props__)
+        __props__ = _UserAdminRolesState.__new__(_UserAdminRolesState)
 
-    @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
-        """
-        Policy Description.
-        """
-        return pulumi.get(self, "description")
-
-    @property
-    @pulumi.getter(name="groupsIncludeds")
-    def groups_includeds(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List of Group IDs to Include.
-        """
-        return pulumi.get(self, "groups_includeds")
+        __props__.__dict__["admin_roles"] = admin_roles
+        __props__.__dict__["disable_notifications"] = disable_notifications
+        __props__.__dict__["user_id"] = user_id
+        return UserAdminRoles(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="adminRoles")
+    def admin_roles(self) -> pulumi.Output[Sequence[str]]:
         """
-        Policy Name.
+        The list of Okta user admin roles, e.g. `["APP_ADMIN", "USER_ADMIN"]` See [API Docs](https://developer.okta.com/docs/reference/api/roles/#role-types).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "admin_roles")
 
     @property
-    @pulumi.getter
-    def priority(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="disableNotifications")
+    def disable_notifications(self) -> pulumi.Output[Optional[bool]]:
         """
-        Priority of the policy.
+        When this setting is enabled, the admins won't receive any of the default Okta
+        administrator emails. These admins also won't have access to contact Okta Support and open support cases on behalf of your org.
         """
-        return pulumi.get(self, "priority")
+        return pulumi.get(self, "disable_notifications")
 
     @property
-    @pulumi.getter
-    def status(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
         """
-        Policy Status: `"ACTIVE"` or `"INACTIVE"`.
+        Okta user ID.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "user_id")
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,17 +328,18 @@
                  target_group_id: Optional[pulumi.Input[str]] = None,
                  ui_schema_id: Optional[pulumi.Input[str]] = None,
                  unknown_user_action: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
-        This resource allows you to create and configure a Profile Enrollment Policy Rule.
-
-        It is documented in the Okta public API's [Profile Enrollment Action object](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-action-object) section.
+        A [profile enrollment
+        policy](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-policy)
+        is limited to one default rule. This resource does not create a rule for an
+        enrollment policy, it allows the default policy rule to be updated.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
@@ -404,17 +405,18 @@
     def __init__(__self__,
                  resource_name: str,
                  args: PolicyRuleProfileEnrollmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
 
-        This resource allows you to create and configure a Profile Enrollment Policy Rule.
-
-        It is documented in the Okta public API's [Profile Enrollment Action object](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-action-object) section.
+        A [profile enrollment
+        policy](https://developer.okta.com/docs/reference/api/policy/#profile-enrollment-policy)
+        is limited to one default rule. This resource does not create a rule for an
+        enrollment policy, it allows the default policy rule to be updated.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/provider.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/resource_set.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/role_subscription.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/template_sms.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/theme.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/get_users.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/outputs.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/user.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                  postal_address: Optional[pulumi.Input[str]] = None,
                  preferred_language: Optional[pulumi.Input[str]] = None,
                  primary_phone: Optional[pulumi.Input[str]] = None,
                  profile_url: Optional[pulumi.Input[str]] = None,
                  recovery_answer: Optional[pulumi.Input[str]] = None,
                  recovery_question: Optional[pulumi.Input[str]] = None,
                  second_email: Optional[pulumi.Input[str]] = None,
+                 skip_roles: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  street_address: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None):
@@ -98,14 +99,15 @@
         :param pulumi.Input[str] profile_url: User profile property.
         :param pulumi.Input[str] recovery_answer: User password recovery answer.
                
                - `password hash` - (Optional) Specifies a hashed password to import into Okta. When updating a user with a hashed password the user must be in the `STAGED` status.
                - `algorithm"` - (Required) The algorithm used to generate the hash using the password (and salt, when applicable). Must be set to BCRYPT, SHA-512, SHA-256, SHA-1 or MD5.
         :param pulumi.Input[str] recovery_question: User password recovery question.
         :param pulumi.Input[str] second_email: User profile property.
+        :param pulumi.Input[bool] skip_roles: Do not populate user roles information (prevents additional API call)
         :param pulumi.Input[str] state: User profile property.
         :param pulumi.Input[str] status: User profile property. Valid values are "ACTIVE", "DEPROVISIONED", "STAGED", "SUSPENDED"
         :param pulumi.Input[str] street_address: User profile property.
         :param pulumi.Input[str] timezone: User profile property.
         :param pulumi.Input[str] title: User profile property.
         :param pulumi.Input[str] user_type: User profile property.
         :param pulumi.Input[str] zip_code: User profile property.
@@ -170,14 +172,19 @@
             pulumi.set(__self__, "profile_url", profile_url)
         if recovery_answer is not None:
             pulumi.set(__self__, "recovery_answer", recovery_answer)
         if recovery_question is not None:
             pulumi.set(__self__, "recovery_question", recovery_question)
         if second_email is not None:
             pulumi.set(__self__, "second_email", second_email)
+        if skip_roles is not None:
+            warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+        if skip_roles is not None:
+            pulumi.set(__self__, "skip_roles", skip_roles)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if street_address is not None:
             pulumi.set(__self__, "street_address", street_address)
         if timezone is not None:
@@ -603,14 +610,26 @@
         return pulumi.get(self, "second_email")
 
     @second_email.setter
     def second_email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "second_email", value)
 
     @property
+    @pulumi.getter(name="skipRoles")
+    def skip_roles(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Do not populate user roles information (prevents additional API call)
+        """
+        return pulumi.get(self, "skip_roles")
+
+    @skip_roles.setter
+    def skip_roles(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_roles", value)
+
+    @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
         User profile property.
         """
         return pulumi.get(self, "state")
 
@@ -725,14 +744,15 @@
                  preferred_language: Optional[pulumi.Input[str]] = None,
                  primary_phone: Optional[pulumi.Input[str]] = None,
                  profile_url: Optional[pulumi.Input[str]] = None,
                  raw_status: Optional[pulumi.Input[str]] = None,
                  recovery_answer: Optional[pulumi.Input[str]] = None,
                  recovery_question: Optional[pulumi.Input[str]] = None,
                  second_email: Optional[pulumi.Input[str]] = None,
+                 skip_roles: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  street_address: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None):
@@ -778,14 +798,15 @@
         :param pulumi.Input[str] raw_status: The raw status of the User in Okta - (status is mapped)
         :param pulumi.Input[str] recovery_answer: User password recovery answer.
                
                - `password hash` - (Optional) Specifies a hashed password to import into Okta. When updating a user with a hashed password the user must be in the `STAGED` status.
                - `algorithm"` - (Required) The algorithm used to generate the hash using the password (and salt, when applicable). Must be set to BCRYPT, SHA-512, SHA-256, SHA-1 or MD5.
         :param pulumi.Input[str] recovery_question: User password recovery question.
         :param pulumi.Input[str] second_email: User profile property.
+        :param pulumi.Input[bool] skip_roles: Do not populate user roles information (prevents additional API call)
         :param pulumi.Input[str] state: User profile property.
         :param pulumi.Input[str] status: User profile property. Valid values are "ACTIVE", "DEPROVISIONED", "STAGED", "SUSPENDED"
         :param pulumi.Input[str] street_address: User profile property.
         :param pulumi.Input[str] timezone: User profile property.
         :param pulumi.Input[str] title: User profile property.
         :param pulumi.Input[str] user_type: User profile property.
         :param pulumi.Input[str] zip_code: User profile property.
@@ -856,14 +877,19 @@
             pulumi.set(__self__, "raw_status", raw_status)
         if recovery_answer is not None:
             pulumi.set(__self__, "recovery_answer", recovery_answer)
         if recovery_question is not None:
             pulumi.set(__self__, "recovery_question", recovery_question)
         if second_email is not None:
             pulumi.set(__self__, "second_email", second_email)
+        if skip_roles is not None:
+            warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+            pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+        if skip_roles is not None:
+            pulumi.set(__self__, "skip_roles", skip_roles)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if street_address is not None:
             pulumi.set(__self__, "street_address", street_address)
         if timezone is not None:
@@ -1301,14 +1327,26 @@
         return pulumi.get(self, "second_email")
 
     @second_email.setter
     def second_email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "second_email", value)
 
     @property
+    @pulumi.getter(name="skipRoles")
+    def skip_roles(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Do not populate user roles information (prevents additional API call)
+        """
+        return pulumi.get(self, "skip_roles")
+
+    @skip_roles.setter
+    def skip_roles(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_roles", value)
+
+    @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
         User profile property.
         """
         return pulumi.get(self, "state")
 
@@ -1424,14 +1462,15 @@
                  postal_address: Optional[pulumi.Input[str]] = None,
                  preferred_language: Optional[pulumi.Input[str]] = None,
                  primary_phone: Optional[pulumi.Input[str]] = None,
                  profile_url: Optional[pulumi.Input[str]] = None,
                  recovery_answer: Optional[pulumi.Input[str]] = None,
                  recovery_question: Optional[pulumi.Input[str]] = None,
                  second_email: Optional[pulumi.Input[str]] = None,
+                 skip_roles: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  street_address: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None,
@@ -1546,14 +1585,15 @@
         :param pulumi.Input[str] profile_url: User profile property.
         :param pulumi.Input[str] recovery_answer: User password recovery answer.
                
                - `password hash` - (Optional) Specifies a hashed password to import into Okta. When updating a user with a hashed password the user must be in the `STAGED` status.
                - `algorithm"` - (Required) The algorithm used to generate the hash using the password (and salt, when applicable). Must be set to BCRYPT, SHA-512, SHA-256, SHA-1 or MD5.
         :param pulumi.Input[str] recovery_question: User password recovery question.
         :param pulumi.Input[str] second_email: User profile property.
+        :param pulumi.Input[bool] skip_roles: Do not populate user roles information (prevents additional API call)
         :param pulumi.Input[str] state: User profile property.
         :param pulumi.Input[str] status: User profile property. Valid values are "ACTIVE", "DEPROVISIONED", "STAGED", "SUSPENDED"
         :param pulumi.Input[str] street_address: User profile property.
         :param pulumi.Input[str] timezone: User profile property.
         :param pulumi.Input[str] title: User profile property.
         :param pulumi.Input[str] user_type: User profile property.
         :param pulumi.Input[str] zip_code: User profile property.
@@ -1678,14 +1718,15 @@
                  postal_address: Optional[pulumi.Input[str]] = None,
                  preferred_language: Optional[pulumi.Input[str]] = None,
                  primary_phone: Optional[pulumi.Input[str]] = None,
                  profile_url: Optional[pulumi.Input[str]] = None,
                  recovery_answer: Optional[pulumi.Input[str]] = None,
                  recovery_question: Optional[pulumi.Input[str]] = None,
                  second_email: Optional[pulumi.Input[str]] = None,
+                 skip_roles: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  street_address: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  user_type: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None,
@@ -1736,14 +1777,18 @@
             __props__.__dict__["postal_address"] = postal_address
             __props__.__dict__["preferred_language"] = preferred_language
             __props__.__dict__["primary_phone"] = primary_phone
             __props__.__dict__["profile_url"] = profile_url
             __props__.__dict__["recovery_answer"] = None if recovery_answer is None else pulumi.Output.secret(recovery_answer)
             __props__.__dict__["recovery_question"] = recovery_question
             __props__.__dict__["second_email"] = second_email
+            if skip_roles is not None and not opts.urn:
+                warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+                pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+            __props__.__dict__["skip_roles"] = skip_roles
             __props__.__dict__["state"] = state
             __props__.__dict__["status"] = status
             __props__.__dict__["street_address"] = street_address
             __props__.__dict__["timezone"] = timezone
             __props__.__dict__["title"] = title
             __props__.__dict__["user_type"] = user_type
             __props__.__dict__["zip_code"] = zip_code
@@ -1791,14 +1836,15 @@
             preferred_language: Optional[pulumi.Input[str]] = None,
             primary_phone: Optional[pulumi.Input[str]] = None,
             profile_url: Optional[pulumi.Input[str]] = None,
             raw_status: Optional[pulumi.Input[str]] = None,
             recovery_answer: Optional[pulumi.Input[str]] = None,
             recovery_question: Optional[pulumi.Input[str]] = None,
             second_email: Optional[pulumi.Input[str]] = None,
+            skip_roles: Optional[pulumi.Input[bool]] = None,
             state: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             street_address: Optional[pulumi.Input[str]] = None,
             timezone: Optional[pulumi.Input[str]] = None,
             title: Optional[pulumi.Input[str]] = None,
             user_type: Optional[pulumi.Input[str]] = None,
             zip_code: Optional[pulumi.Input[str]] = None) -> 'User':
@@ -1849,14 +1895,15 @@
         :param pulumi.Input[str] raw_status: The raw status of the User in Okta - (status is mapped)
         :param pulumi.Input[str] recovery_answer: User password recovery answer.
                
                - `password hash` - (Optional) Specifies a hashed password to import into Okta. When updating a user with a hashed password the user must be in the `STAGED` status.
                - `algorithm"` - (Required) The algorithm used to generate the hash using the password (and salt, when applicable). Must be set to BCRYPT, SHA-512, SHA-256, SHA-1 or MD5.
         :param pulumi.Input[str] recovery_question: User password recovery question.
         :param pulumi.Input[str] second_email: User profile property.
+        :param pulumi.Input[bool] skip_roles: Do not populate user roles information (prevents additional API call)
         :param pulumi.Input[str] state: User profile property.
         :param pulumi.Input[str] status: User profile property. Valid values are "ACTIVE", "DEPROVISIONED", "STAGED", "SUSPENDED"
         :param pulumi.Input[str] street_address: User profile property.
         :param pulumi.Input[str] timezone: User profile property.
         :param pulumi.Input[str] title: User profile property.
         :param pulumi.Input[str] user_type: User profile property.
         :param pulumi.Input[str] zip_code: User profile property.
@@ -1896,14 +1943,15 @@
         __props__.__dict__["preferred_language"] = preferred_language
         __props__.__dict__["primary_phone"] = primary_phone
         __props__.__dict__["profile_url"] = profile_url
         __props__.__dict__["raw_status"] = raw_status
         __props__.__dict__["recovery_answer"] = recovery_answer
         __props__.__dict__["recovery_question"] = recovery_question
         __props__.__dict__["second_email"] = second_email
+        __props__.__dict__["skip_roles"] = skip_roles
         __props__.__dict__["state"] = state
         __props__.__dict__["status"] = status
         __props__.__dict__["street_address"] = street_address
         __props__.__dict__["timezone"] = timezone
         __props__.__dict__["title"] = title
         __props__.__dict__["user_type"] = user_type
         __props__.__dict__["zip_code"] = zip_code
@@ -2195,14 +2243,22 @@
     def second_email(self) -> pulumi.Output[Optional[str]]:
         """
         User profile property.
         """
         return pulumi.get(self, "second_email")
 
     @property
+    @pulumi.getter(name="skipRoles")
+    def skip_roles(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Do not populate user roles information (prevents additional API call)
+        """
+        return pulumi.get(self, "skip_roles")
+
+    @property
     @pulumi.getter
     def state(self) -> pulumi.Output[Optional[str]]:
         """
         User profile property.
         """
         return pulumi.get(self, "state")
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user/user_type.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.0.0a1685982970/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-okta
-Version: 4.0.0a1685663230
+Version: 4.0.0a1685982970
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.0.0a1685663230/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.0.0a1685982970/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.0.0a1685663230/setup.py` & `pulumi_okta-4.0.0a1685982970/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.0.0a1685663230"
-PLUGIN_VERSION = "4.0.0-alpha.1685663230+8cbaf7e4"
+VERSION = "4.0.0a1685982970"
+PLUGIN_VERSION = "4.0.0-alpha.1685982970+0bf9727c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'okta', PLUGIN_VERSION])
         except OSError as error:
```

