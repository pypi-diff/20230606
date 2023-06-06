# Comparing `tmp/dj-accounts-3.0.9.tar.gz` & `tmp/dj-accounts-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-accounts-3.0.9.tar", last modified: Tue May  2 23:15:12 2023, max compression
+gzip compressed data, was "dj-accounts-3.1.0.tar", last modified: Tue Jun  6 18:05:56 2023, max compression
```

## Comparing `dj-accounts-3.0.9.tar` & `dj-accounts-3.1.0.tar`

### file list

```diff
@@ -1,111 +1,110 @@
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/LICENSE
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      139 2023-05-02 23:14:17.000000 dj-accounts-3.0.9/MANIFEST.in
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/README.md
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.839567 dj-accounts-3.0.9/accounts_pkg/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/api_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/asgi.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/settings-multi-auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/settings.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      378 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/wsgi.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/dj_accounts/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8485 2023-05-02 17:05:25.000000 dj-accounts-3.0.9/dj_accounts/forms.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/locale/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/locale/ar/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8091 2023-05-02 19:54:37.000000 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    12344 2023-05-02 19:54:27.000000 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.po
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4695 2023-05-02 17:11:11.000000 dj-accounts-3.0.9/dj_accounts/serializers.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/templates/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.139567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/auth_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/confirm_email_template.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      202 2023-05-02 17:52:57.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/email_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      948 2023-05-02 17:54:18.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/login.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.143567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.207567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/gender.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password1.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password2.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/username.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login-tabs.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/logo.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/social_login.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_confirm.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_done.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_subject.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/phone_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/register.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1652 2023-05-02 18:00:25.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/sidebar.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_email_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_phone_number_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_data_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_password_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/verify_phone.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.271567 dj-accounts-3.0.9/dj_accounts/tests/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/factories.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.299567 dj-accounts-3.0.9/dj_accounts/tests/migrations/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/migrations/0001_initial.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/migrations/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/mocks.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2927 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/models.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_forms.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8201 2023-05-02 19:50:05.000000 dj-accounts-3.0.9/dj_accounts/tests/test_serializers.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_tokens.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    24255 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_view_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_views.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.299567 dj-accounts-3.0.9/dj_accounts/urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/__init__.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.303567 dj-accounts-3.0.9/dj_accounts/urls/api_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1317 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_auth_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      386 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_profile_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.303567 dj-accounts-3.0.9/dj_accounts/urls/site_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_profile.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1120 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/utils.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/views.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    10759 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/views_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts.egg-info/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3804 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/SOURCES.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/dependency_links.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/top_level.txt
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.431567 dj-accounts-3.0.9/docs/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/APIAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/APIProfile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/PhoneVerificationService.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/Profile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/SessionAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/docs/index.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/pyproject.toml
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      921 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/setup.cfg
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/setup.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.682730 dj-accounts-3.1.0/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/LICENSE
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      139 2023-05-02 23:14:17.000000 dj-accounts-3.1.0/MANIFEST.in
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-06-06 18:05:56.682730 dj-accounts-3.1.0/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/README.md
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.146730 dj-accounts-3.1.0/accounts_pkg/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/accounts_pkg/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/accounts_pkg/api_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/accounts_pkg/asgi.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/accounts_pkg/settings-multi-auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/accounts_pkg/settings.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      381 2023-06-06 16:58:27.000000 dj-accounts-3.1.0/accounts_pkg/urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/accounts_pkg/wsgi.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.174729 dj-accounts-3.1.0/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.1.0/dj_accounts/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8542 2023-06-06 17:09:49.000000 dj-accounts-3.1.0/dj_accounts/forms.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.014730 dj-accounts-3.1.0/dj_accounts/locale/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.014730 dj-accounts-3.1.0/dj_accounts/locale/ar/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.190729 dj-accounts-3.1.0/dj_accounts/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8091 2023-05-02 19:54:37.000000 dj-accounts-3.1.0/dj_accounts/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    12344 2023-05-02 19:54:27.000000 dj-accounts-3.1.0/dj_accounts/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.014730 dj-accounts-3.1.0/dj_accounts/templates/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.398730 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/auth_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/confirm_email_template.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      202 2023-05-02 17:52:57.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/email_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      948 2023-05-02 17:54:18.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/login.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.418730 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.526729 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/gender.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password1.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password2.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/username.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login-tabs.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login_with_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/logo.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/social_login.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_confirm.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_done.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_subject.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/phone_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/profile.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/profile_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/register.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1652 2023-05-02 18:00:25.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/sidebar.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/update_email_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/update_phone_number_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/update_user_data_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/update_user_password_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/verify_phone.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.606730 dj-accounts-3.1.0/dj_accounts/tests/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/factories.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.606730 dj-accounts-3.1.0/dj_accounts/tests/migrations/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/migrations/0001_initial.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/migrations/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/mocks.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2936 2023-06-06 16:01:59.000000 dj-accounts-3.1.0/dj_accounts/tests/models.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      301 2023-06-06 17:22:29.000000 dj-accounts-3.1.0/dj_accounts/tests/profile_handlers.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_forms.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_tokens.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    23167 2023-06-06 18:01:54.000000 dj-accounts-3.1.0/dj_accounts/tests/test_view_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/tests/test_views.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.606730 dj-accounts-3.1.0/dj_accounts/urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/urls/__init__.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.606730 dj-accounts-3.1.0/dj_accounts/urls/api_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/urls/api_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1222 2023-06-06 18:01:54.000000 dj-accounts-3.1.0/dj_accounts/urls/api_urls/urls_auth_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      700 2023-06-06 17:58:30.000000 dj-accounts-3.1.0/dj_accounts/urls/api_urls/urls_profile_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.610730 dj-accounts-3.1.0/dj_accounts/urls/site_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/urls/site_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/urls/site_urls/urls_auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/urls/site_urls/urls_profile.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2059 2023-06-06 17:04:25.000000 dj-accounts-3.1.0/dj_accounts/utils.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/dj_accounts/views.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    12244 2023-06-06 18:01:54.000000 dj-accounts-3.1.0/dj_accounts/views_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.174729 dj-accounts-3.1.0/dj_accounts.egg-info/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-06-06 18:05:55.000000 dj-accounts-3.1.0/dj_accounts.egg-info/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3777 2023-06-06 18:05:55.000000 dj-accounts-3.1.0/dj_accounts.egg-info/SOURCES.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2023-06-06 18:05:55.000000 dj-accounts-3.1.0/dj_accounts.egg-info/dependency_links.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2023-06-06 18:05:55.000000 dj-accounts-3.1.0/dj_accounts.egg-info/top_level.txt
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-06-06 18:05:56.658730 dj-accounts-3.1.0/docs/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/docs/APIAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/docs/APIProfile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/docs/PhoneVerificationService.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/docs/Profile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/docs/SessionAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/docs/index.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2023-05-02 16:33:59.000000 dj-accounts-3.1.0/pyproject.toml
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      921 2023-06-06 18:05:56.686730 dj-accounts-3.1.0/setup.cfg
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2023-05-02 16:33:28.000000 dj-accounts-3.1.0/setup.py
```

### Comparing `dj-accounts-3.0.9/LICENSE` & `dj-accounts-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/PKG-INFO` & `dj-accounts-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.9
+Version: 3.1.0
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
 Description: ## Installation
```

### Comparing `dj-accounts-3.0.9/README.md` & `dj-accounts-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/accounts_pkg/settings-multi-auth.py` & `dj-accounts-3.1.0/accounts_pkg/settings-multi-auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/accounts_pkg/settings.py` & `dj-accounts-3.1.0/accounts_pkg/settings.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/backends.py` & `dj-accounts-3.1.0/dj_accounts/backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/forms.py` & `dj-accounts-3.1.0/dj_accounts/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 
 # profile forms
 
 
 class UserChangeForm(BaseUserChangeForm):
     class Meta(BaseUserChangeForm.Meta):
         model = UserModel
+        fields = ('username', 'first_name', 'last_name')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class UpdateUserDataForm(UserChangeForm):
     class Meta:
```

### Comparing `dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.mo` & `dj-accounts-3.1.0/dj_accounts/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.po` & `dj-accounts-3.1.0/dj_accounts/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/confirm_email_template.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/confirm_email_template.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/login.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/login.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/email.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/first_name.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/first_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/gender.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/gender.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/last_name.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/last_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password1.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password1.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password2.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/password2.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/phone.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/username.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/fields/username.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login-tabs.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login-tabs.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_email.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login_with_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_phone.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/partials/login_with_phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_confirm.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_done.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_email.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_form.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile_base.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/profile_base.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/sidebar.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/sidebar.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_password_form.html` & `dj-accounts-3.1.0/dj_accounts/templates/dj_accounts/update_user_password_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/factories.py` & `dj-accounts-3.1.0/dj_accounts/tests/factories.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/migrations/0001_initial.py` & `dj-accounts-3.1.0/dj_accounts/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/models.py` & `dj-accounts-3.1.0/dj_accounts/tests/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 class User(AbstractUser):
     objects = UserManager()
 
     USERNAME_FIELD = 'username'
     EMAIL_FIELD = 'email'
-    REQUIRED_FIELDS = ['phone']
+    REQUIRED_FIELDS = ['phone', 'email']
     AUTHENTICATION_FIELDS = ['email', 'username', 'phone', 'id']
 
     username_validator = UnicodeUsernameValidator()
     email_validator = EmailValidator()
 
     email = models.EmailField(_('email address'),
                               validators=[email_validator],
```

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_backends.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_forms.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_tokens.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_urls.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_verify_phone.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_view_api.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_view_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from rest_framework.reverse import reverse
 from rest_framework.test import APIClient
 from rest_framework.test import APITestCase
 from rest_framework.views import APIView
 from rest_framework_simplejwt.tokens import RefreshToken
 
 from .factories import UserFactory
-from ..serializers import ChangePasswordSerializer
 from ..utils import account_activation_token
 from ..views_api import UpdateProfileAPIView, ChangeEmailAPIView, ChangePhoneAPIView, \
     VerifyPhoneAPIView, VerifyEmailAPIView, ResendPhoneConfirmationAPIView, UserLogoutAPIView, ChangePasswordAPIView
 
 
 # test auth
 class LoginAPIViewTestCase(TestCase):
@@ -175,15 +174,15 @@
 
     def test_it_return_400_if_invalid_token_was_given(self):
         self.client.credentials(HTTP_AUTHORIZATION='Bearer {}'.format(self.token))
         response = self.client.post(reverse('logout_api'), {'refresh': 'abc'})
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class UserSignupAPIViewTestCase(TestCase):
+class RegisterAPIViewTestCase(TestCase):
     def setUp(self):
         self.client = APIClient()
         self.user = UserFactory()
         self.url = reverse('signup_api')
         self.data = {
             "email": "test@test.test",
             "username": "TestUser",
@@ -357,83 +356,74 @@
 class UpdateProfileDataAPIViewStructureTestCase(TestCase):
     def test_it_extends_django_LoginView(self):
         self.assertTrue(issubclass(UpdateProfileAPIView, APIView))
 
     def test_it_permission_classes_has_is_authenticated(self):
         self.assertIn(IsAuthenticated, UpdateProfileAPIView.permission_classes)
 
-    def test_view_has_method_put(self):
-        self.assertTrue(hasattr(UpdateProfileAPIView, 'put'))
+    def test_view_has_method_post(self):
+        self.assertTrue(hasattr(UpdateProfileAPIView, 'post'))
 
-    def test_view_has_method_put_is_callable(self):
-        self.assertTrue(callable(UpdateProfileAPIView.put))
+    def test_view_has_method_post_is_callable(self):
+        self.assertTrue(callable(UpdateProfileAPIView.post))
 
-    def test_put_method_signature(self):
+    def test_post_method_signature(self):
         expected_signature = ['self', 'request']
-        actual_signature = inspect.getfullargspec(UpdateProfileAPIView.put)[0]
+        actual_signature = inspect.getfullargspec(UpdateProfileAPIView.post)[0]
         self.assertEquals(actual_signature, expected_signature)
 
-    def test_it_has_get_serializer_class_method(self):
-        self.assertIn('get_serializer_class', UpdateProfileAPIView.__dict__)
-
 
 class UpdateProfileDataAPIViewTestCase(APITestCase):
     def setUp(self):
         self.client = APIClient()
         self.user = UserFactory()
         self.refresh = RefreshToken.for_user(self.user)
         self.client.credentials(HTTP_AUTHORIZATION='Bearer {}'.format(self.refresh.access_token))
         self.url = reverse('update-profile-api')
         self.data = {
+            'username': self.user.username,
             'first_name': self.user.first_name,
             'last_name': self.user.last_name,
         }
 
     def tearDown(self):
         self.client.logout()
 
     def test_it_through_exception_if_user_is_not_authenticated(self):
         self.client.logout()
-        response = self.client.put(self.url)
+        response = self.client.post(self.url)
         self.assertEquals(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
-    def test_it_returns_status_code_of_201_if_data_profile_is_updated(self):
-        response = self.client.put(self.url, self.data)
-        self.assertEquals(response.status_code, status.HTTP_201_CREATED)
+    def test_it_returns_status_code_of_200_if_data_profile_is_updated(self):
+        response = self.client.post(self.url, self.data)
+        self.assertEquals(response.status_code, status.HTTP_200_OK)
 
     def test_it_returns_user_data_after_updated(self):
-        response = self.client.put(self.url, self.data)
+        response = self.client.post(self.url, self.data)
         self.assertIsNotNone(response.data)
 
-    def test_it_returns_201_when_user_created_successfully(self):
-        response = self.client.put(self.url, data=self.data)
-        self.assertEquals(response.status_code, 201)
-
 
 class UpdateEmailAPIViewStructureTestCase(TestCase):
     def test_it_extends_django_LoginView(self):
         self.assertTrue(issubclass(ChangeEmailAPIView, APIView))
 
     def test_it_permission_classes_has_is_authenticated(self):
         self.assertIn(IsAuthenticated, ChangeEmailAPIView.permission_classes)
 
-    def test_view_has_method_put(self):
-        self.assertTrue(hasattr(ChangeEmailAPIView, 'put'))
+    def test_view_has_method_post(self):
+        self.assertTrue(hasattr(ChangeEmailAPIView, 'post'))
 
-    def test_view_has_method_put_is_callable(self):
-        self.assertTrue(callable(ChangeEmailAPIView.put))
+    def test_view_has_method_post_is_callable(self):
+        self.assertTrue(callable(ChangeEmailAPIView.post))
 
-    def test_put_method_signature(self):
+    def test_post_method_signature(self):
         expected_signature = ['self', 'request']
-        actual_signature = inspect.getfullargspec(ChangeEmailAPIView.put)[0]
+        actual_signature = inspect.getfullargspec(ChangeEmailAPIView.post)[0]
         self.assertEquals(actual_signature, expected_signature)
 
-    def test_it_has_get_serializer_class_method(self):
-        self.assertIn('get_serializer_class', ChangeEmailAPIView.__dict__)
-
 
 class UpdateEmailAPIViewTestCase(APITestCase):
     def setUp(self):
         self.client = APIClient()
         self.user = UserFactory(email='test@test.com')
         self.refresh = RefreshToken.for_user(self.user)
         self.client.credentials(HTTP_AUTHORIZATION='Bearer {}'.format(self.refresh.access_token))
@@ -444,60 +434,57 @@
         }
 
     def tearDown(self):
         self.client.logout()
 
     def test_it_through_exception_if_user_is_not_authenticated(self):
         self.client.logout()
-        response = self.client.put(self.url)
+        response = self.client.post(self.url)
         self.assertEquals(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
     def test_it_returns_422_when_data_is_invalid(self):
-        response = self.client.put(self.url, data={})
+        response = self.client.post(self.url, data={})
         self.assertEquals(response.status_code, 422)
 
     def test_it_returns_201_when_user_created_successfully(self):
-        response = self.client.put(self.url, data=self.data)
-        self.assertEquals(response.status_code, 201)
+        response = self.client.post(self.url, data=self.data)
+        self.assertEquals(response.status_code, 200)
 
     def test_it_returns_422_if_user_tried_to_enter_the_same_email(self):
         data = {
             'email': "test@test.com",
             "password": "secret",
         }
-        response = self.client.put(self.url, data=data)
+        response = self.client.post(self.url, data=data)
         self.assertEquals(response.status_code, 422)
 
     def test_it_change_email_for_user(self):
-        self.client.put(self.url, data=self.data)
+        self.client.post(self.url, data=self.data)
         self.user.refresh_from_db()
         self.assertEquals(self.user.email, self.data['new_email'])
 
 
 class UpdatePhoneAPIViewStructure(TestCase):
     def test_it_extends_django_LoginView(self):
         self.assertTrue(issubclass(ChangePhoneAPIView, APIView))
 
     def test_it_permission_classes_has_is_authenticated(self):
         self.assertIn(IsAuthenticated, ChangePhoneAPIView.permission_classes)
 
-    def test_view_has_method_put(self):
-        self.assertTrue(hasattr(ChangePhoneAPIView, 'put'))
+    def test_view_has_method_post(self):
+        self.assertTrue(hasattr(ChangePhoneAPIView, 'post'))
 
-    def test_view_has_method_put_is_callable(self):
-        self.assertTrue(callable(ChangePhoneAPIView.put))
+    def test_view_has_method_post_is_callable(self):
+        self.assertTrue(callable(ChangePhoneAPIView.post))
 
-    def test_put_method_signature(self):
+    def test_post_method_signature(self):
         expected_signature = ['self', 'request']
-        actual_signature = inspect.getfullargspec(ChangePhoneAPIView.put)[0]
+        actual_signature = inspect.getfullargspec(ChangePhoneAPIView.post)[0]
         self.assertEquals(actual_signature, expected_signature)
 
-    def test_it_has_get_serializer_class_method(self):
-        self.assertIn('get_serializer_class', ChangePhoneAPIView.__dict__)
-
 
 class UpdatePhoneAPIViewTestCase(APITestCase):
     def setUp(self):
         self.client = APIClient()
         self.user = UserFactory(phone='+201005263977')
         self.refresh = RefreshToken.for_user(self.user)
         self.client.credentials(HTTP_AUTHORIZATION='Bearer {}'.format(self.refresh.access_token))
@@ -508,78 +495,66 @@
         }
 
     def tearDown(self):
         self.client.logout()
 
     def test_it_through_exception_if_user_is_not_authenticated(self):
         self.client.logout()
-        response = self.client.put(self.url)
+        response = self.client.post(self.url)
         self.assertEquals(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
     def test_it_returns_422_when_data_is_invalid(self):
-        response = self.client.put(self.url, data={})
+        response = self.client.post(self.url, data={})
         self.assertEquals(response.status_code, 422)
 
     def test_it_returns_201_when_user_created_successfully(self):
-        response = self.client.put(self.url, data=self.data)
-        self.assertEquals(response.status_code, 201)
+        response = self.client.post(self.url, data=self.data)
+        self.assertEquals(response.status_code, 200)
 
     def test_it_returns_201_when_user_old_phone_number_is_equal_to_new_number(self):
         data = {
             'new_phone': "+201005263977",
             "password": "secret",
         }
-        response = self.client.put(self.url, data=data)
+        response = self.client.post(self.url, data=data)
         self.assertEquals(response.status_code, 422)
 
 
 class ChangePasswordAPIViewStructureAPIView(TestCase):
     def setUp(self):
         self.view = ChangePasswordAPIView
 
-    def test_it_has_serializer_class(self):
-        self.assertTrue(hasattr(self.view, 'serializer_class'))
-
-    def test_it_has_model(self):
-        self.assertTrue(hasattr(self.view, 'model'))
-
     def test_it_has_permission_class(self):
         self.assertTrue(hasattr(self.view, 'permission_classes'))
 
-    def test_it_has_update_method(self):
-        self.assertIn('update', self.view.__dict__)
+    def test_it_has_post_method(self):
+        self.assertIn('post', self.view.__dict__)
 
 
 class ChangePasswordAPIViewTestCase(TestCase):
     def setUp(self):
         self.user = UserFactory()
         self.client = APIClient()
         self.refresh = RefreshToken.for_user(self.user)
         self.client.credentials(HTTP_AUTHORIZATION='Bearer {}'.format(self.refresh.access_token))
         self.url = reverse('change_password_api')
-        self.data= {
+        self.data = {
             "new_password1": '12345678Aa',
             "new_password2": '12345678Aa',
             "old_password": 'secret'
         }
         self.password = self.user.password
 
-    def test_it_uses_change_password_serializer(self):
-        self.assertIs(ChangePasswordAPIView.serializer_class, ChangePasswordSerializer)
-
     def test_it_returns_401_when_user_is_unauthenticated(self):
         self.client.logout()
-        response = self.client.put(self.url, data={})
+        response = self.client.post(self.url, data={})
         self.assertEquals(response.status_code, status.HTTP_401_UNAUTHORIZED)
 
     def test_it_returns_422_invalid_data(self):
-        response = self.client.put(self.url, data={})
+        response = self.client.post(self.url, data={})
         self.assertEqual(response.status_code, status.HTTP_422_UNPROCESSABLE_ENTITY)
 
     def test_it_returns_200_on_update(self):
-        response = self.client.put(self.url, data=self.data)
+        response = self.client.post(self.url, data=self.data)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-    def test_it_updates_password(self):
-        self.client.put(self.url, data=self.data)
-        self.user.refresh_from_db()
-        self.assertNotEqual(self.user.password, self.password)
+
```

### Comparing `dj-accounts-3.0.9/dj_accounts/tests/test_views.py` & `dj-accounts-3.1.0/dj_accounts/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_auth_api.py` & `dj-accounts-3.1.0/dj_accounts/urls/api_urls/urls_auth_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from ...views_api import VerifyPhoneAPIView, \
-    VerifyEmailAPIView, ResendPhoneConfirmationAPIView, UserSignupAPIView, ResendEmailConfirmationLinkAPIView, \
+    VerifyEmailAPIView, ResendPhoneConfirmationAPIView, RegisterAPIView, ResendEmailConfirmationLinkAPIView, \
     UserLogoutAPIView, PasswordResetAPIView, LoginAPIView, ChangePasswordAPIView
 from django.urls import path
 from rest_framework_simplejwt.views import TokenRefreshView
 
 urlpatterns = [
 
     # simple jwt
     path('login/', LoginAPIView.as_view(), name='login_api'),
     path('token/refresh/', TokenRefreshView.as_view(), name='token_refresh'),
     path('logout/', UserLogoutAPIView.as_view(), name='logout_api'),
-    path('signup/', UserSignupAPIView.as_view(), name='signup_api'),
+    path('signup/', RegisterAPIView.as_view(), name='signup_api'),
 
     # password
-    path('change_password/', ChangePasswordAPIView.as_view(), name='change_password_api'),
     path('password_reset/', PasswordResetAPIView.as_view(), name='password_reset_api'),
 
     # email verification
     path('verify/email/<str:uidb64>/<str:token>/', VerifyEmailAPIView.as_view(), name='verify_email_api'),
     path('resend_email_activation/', ResendEmailConfirmationLinkAPIView.as_view(), name='resend_email_activation_api'),
 
     # phone verification
```

### Comparing `dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_auth.py` & `dj-accounts-3.1.0/dj_accounts/urls/site_urls/urls_auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/verify_phone.py` & `dj-accounts-3.1.0/dj_accounts/verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/views.py` & `dj-accounts-3.1.0/dj_accounts/views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/dj_accounts/views_api.py` & `dj-accounts-3.1.0/dj_accounts/views_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import importlib
 import sys
 import traceback
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.contrib.auth.forms import PasswordResetForm, PasswordChangeForm
 from django.contrib.auth.tokens import default_token_generator
 from django.utils.encoding import force_text
 from django.utils.http import urlsafe_base64_decode
 from django.utils.timezone import now
 from django.utils.translation import gettext as _
 from django.utils.translation import gettext_lazy as _
 from rest_framework import status
-from rest_framework.generics import UpdateAPIView
+from rest_framework.exceptions import ValidationError
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
+from rest_framework_simplejwt.exceptions import TokenError
 from rest_framework_simplejwt.tokens import RefreshToken
 
-from .forms import UpdateEmailForm, UpdatePhoneNumberForm
+from .forms import UpdateEmailForm, UpdatePhoneNumberForm, MultipleLoginForm
 from .forms import VerifyPhoneForm
-from .serializers import LogoutSerializer, PasswordResetSerializer, RegisterSerializer, \
-    LoginSerializer, ChangePasswordSerializer
-from .utils import account_activation_token, send_mail_confirmation
+from .utils import account_activation_token, send_mail_confirmation, get_user_tokens, get_errors, get_settings_value, \
+    get_class_from_settings
 from .verify_phone import VerifyPhone
 
 UserModel = get_user_model()
 
 
-class UserSignupAPIView(APIView):
+class RegisterAPIView(APIView):
     access_token = None
     refresh_token = None
     token = None
     user = None
     authentication_classes = []
     permission_classes = []
 
@@ -75,82 +76,83 @@
         return Response(errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
 
 class LoginAPIView(APIView):
     authentication_classes = []
     permission_classes = []
 
+    def get_form_class(self):
+        """
+        if MULTIPLE_AUTHENTICATION_ACTIVE is True
+        - returns MultipleLoginForm
+        else
+        - returns the regular AuthenticationForm if LOGIN_FORM setting is not defined
+        - returns the provided LOGIN_FORM if set
+        """
+        if get_settings_value('MULTIPLE_AUTHENTICATION_ACTIVE', False):
+            return MultipleLoginForm
+        return get_class_from_settings('LOGIN_FORM', 'django.contrib.auth.forms.AuthenticationForm')
+
     def post(self, request, *args, **kwargs):
-        serializer = LoginSerializer(data=request.data)
-        if serializer.is_valid():
-            user = serializer.cache_user
-            tokens = RefreshToken.for_user(user)
-            return Response({
-                "access_token": str(tokens.access_token),
-                "refresh_token": str(tokens)
-            }, status=status.HTTP_200_OK)
-        return Response(serializer.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+        form = self.get_form_class()(data=request.data)
+        if form.is_valid():
+            user = form.user_cache
+            tokens = get_user_tokens(user)
+            return Response(tokens, status=status.HTTP_200_OK)
+
+        return Response(get_errors(form.errors.as_data()), status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
 
 class UserLogoutAPIView(APIView):
     permission_classes = (IsAuthenticated,)
 
     def post(self, request, *args, **kwargs):
-        serializer = LogoutSerializer(data=request.data)
-        if serializer.is_valid():
-            serializer.save()
-            return Response(status=status.HTTP_204_NO_CONTENT)
-        return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
-
+        token = request.POST.get('refresh', None)
+        if not token:
+            return Response({_("token field is required")}, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
-class ChangePasswordAPIView(UpdateAPIView):
-    serializer_class = ChangePasswordSerializer
-    model = UserModel
-    permission_classes = [IsAuthenticated]
-
-    def update(self, request, *args, **kwargs):
-        serializer = self.get_serializer(data=request.data, context={'request': request})
+        try:
+            RefreshToken(token).blacklist()
+        except TokenError:
+            raise ValidationError({"refresh": _('Invalid token.')})
 
-        if serializer.is_valid():
-            serializer.save()
-            return Response(status=status.HTTP_200_OK, data={'msg': _("Password updated successfully")})
-        return Response(status=status.HTTP_422_UNPROCESSABLE_ENTITY, data=serializer.errors)
+        return Response(status=status.HTTP_204_NO_CONTENT)
 
 
 class PasswordResetAPIView(APIView):
     permission_classes = []
     authentication_classes = []
     email_template_name = 'dj_accounts/password_reset_email.html'
     extra_email_context = None
     from_email = None
     html_email_template_name = None
     subject_template_name = 'dj_accounts/password_reset_subject.txt'
     token_generator = default_token_generator
 
     def post(self, request, *args, **kwargs):
-        serializer = PasswordResetSerializer(data=request.data)
-        if serializer.is_valid():
+        form = PasswordResetForm(data=request.data)
+        if form.is_valid():
             opts = {
                 'use_https': self.request.is_secure(),
                 'token_generator': self.token_generator,
                 'from_email': self.from_email,
                 'email_template_name': self.email_template_name,
                 'subject_template_name': self.subject_template_name,
                 'request': self.request,
                 'html_email_template_name': self.html_email_template_name,
                 'extra_email_context': self.extra_email_context,
             }
-            serializer.save(opts=opts)
+            form.save(**opts)
             return Response({"message": "{} {}".format(
                 _('We’ve emailed you instructions for setting your password, '
                   'if an account exists with the email you entered. You should receive them shortly.'),
                 _('If you don’t receive an email, please make sure you’ve entered '
                   'the address you registered with, and check your spam folder.'))},
                 status=status.HTTP_200_OK)
-        return Response(serializer.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+        return Response(get_errors(form.errors.as_data()), status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
 
 class VerifyPhoneAPIView(APIView):
     permission_classes = [IsAuthenticated, ]
 
     def post(self, request, *args, **kwargs):
         if request.user.phone_verified_at is not None:
@@ -204,64 +206,93 @@
             user = None
         if user is not None and account_activation_token.check_token(user, token):
             user.email_verified_at = now()
             user.save()
         return Response({"message": _('Email was verified successfully.')}, status=status.HTTP_200_OK)
 
 
+class ProfileDetailsAPIView(APIView):
+    permission_classes = (IsAuthenticated,)
+
+    def get_profile_serializer(self):
+        profile_handler = getattr(settings, "PROFILE_SERIALIZER_HANDLER",
+                                  'dj_accounts.tests.profile_handlers.profile_serializer_handler')
+        profile_handler_split = profile_handler.split('.')
+        class_name = profile_handler_split[-1:][0]
+        module_name = profile_handler_split[:-1]
+        return getattr(importlib.import_module('.'.join(module_name)), class_name)()
+
+    def get(self, request, *args, **kwargs):
+        return Response(self.get_profile_serializer()(self.request.user).data, status=status.HTTP_200_OK)
+
+
 class UpdateProfileAPIView(APIView):
-    """
-    An endpoint for changing User Profile Data.
-    """
-
-    def get_serializer_class(self):
-        serializer_class = getattr(settings, "PROFILE_SERIALIZER", 'dj_accounts.serializer.UpdateUserDataSerializer')
-        if type(serializer_class) is str:
-            form_class_split = serializer_class.split('.')
+    permission_classes = (IsAuthenticated,)
+
+    def get_form_class(self):
+        form_class = getattr(settings, "PROFILE_FORM", 'dj_accounts.forms.UserChangeForm')
+        if type(form_class) is str:
+            form_class_split = form_class.split('.')
             class_name = form_class_split[-1:][0]
             module_name = form_class_split[:-1]
             return getattr(importlib.import_module('.'.join(module_name)), class_name)
-        return serializer_class
+        return form_class
 
-    permission_classes = (IsAuthenticated,)
+    def get_profile_serializer(self):
+        profile_handler = getattr(settings, "PROFILE_SERIALIZER_HANDLER",
+                                  'dj_accounts.tests.profile_handlers.profile_serializer_handler')
+        profile_handler_split = profile_handler.split('.')
+        class_name = profile_handler_split[-1:][0]
+        module_name = profile_handler_split[:-1]
+        return getattr(importlib.import_module('.'.join(module_name)), class_name)()
+
+    def post(self, request, *args, **kwargs):
+        form = self.get_form_class()(data=request.data, instance=request.user)
+        if form.is_valid():
+            form.save()
+            self.request.user.refresh_from_db()
+            return Response(self.get_profile_serializer()(self.request.user).data, status=status.HTTP_200_OK)
+        return Response(form.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+
+
+class ChangePasswordAPIView(APIView):
+    permission_classes = [IsAuthenticated]
 
-    def put(self, request, *args, **kwargs):
-        serializer = self.get_serializer_class()(data=request.data, instance=request.user)
-        if serializer.is_valid():
-            serializer.save()
-            return Response(serializer.data, status=status.HTTP_201_CREATED)
-        return Response(serializer.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+    def post(self, request, *args, **kwargs):
+        form = PasswordChangeForm(data=request.data, user=request.user)
+        if form.is_valid():
+            form.save()
+            return Response(data={'message': _("Password updated successfully")}, status=status.HTTP_200_OK)
+        return Response(get_errors(form.errors.as_data()), status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
 
 class ChangeEmailAPIView(APIView):
-    """
-    An endpoint for changing Email.
-    """
     permission_classes = (IsAuthenticated,)
 
-    def get_serializer_class(self):
-        # todo: change this serializer to basic Update Email Form
-        return getattr(settings, "UPDATE_EMAIL_FORM", UpdateEmailForm)
-
-    def put(self, request, *args, **kwargs):
-        validation_from = self.get_serializer_class()(data=request.data, user=request.user)
-        if validation_from.is_valid():
-            validation_from.save()
-            return Response({'message': _('Email Changed Successfully')}, status=status.HTTP_201_CREATED)
-        return Response(validation_from.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+    def post(self, request, *args, **kwargs):
+        form = UpdateEmailForm(data=request.data, user=request.user)
+        if form.is_valid():
+            form.save()
+            return Response({'message': _('Email Changed Successfully')}, status=status.HTTP_200_OK)
+        return Response(get_errors(form.errors.as_data()), status=status.HTTP_422_UNPROCESSABLE_ENTITY)
 
 
 class ChangePhoneAPIView(APIView):
-    """
-    An endpoint for changing Phone.
-    """
     permission_classes = (IsAuthenticated,)
 
-    def get_serializer_class(self):
-        return getattr(settings, "UPDATE_PHONE_FORM", UpdatePhoneNumberForm)
+    def post(self, request, *args, **kwargs):
+        form = UpdatePhoneNumberForm(data=request.data, user=request.user)
+        if form.is_valid():
+            form.save()
+            return Response({'message': _('Phone Changed Successfully')}, status=status.HTTP_200_OK)
+        return Response(get_errors(form.errors.as_data()), status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+
 
-    def put(self, request, *args, **kwargs):
-        validated_fields = self.get_serializer_class()(data=request.data, user=request.user)
-        if validated_fields.is_valid():
-            validated_fields.save()
-            return Response(status=status.HTTP_201_CREATED)
-        return Response(validated_fields.errors, status=status.HTTP_422_UNPROCESSABLE_ENTITY)
+class DeleteProfileAPIView(APIView):
+    permission_classes = [IsAuthenticated]
+
+    def post(self, request, *args, **kwargs):
+        UserLogoutAPIView().post(request, *args, **kwargs)
+        request.user.delete()
+        return Response({
+            "message": _("Account Deleted Successfully!")
+        })
```

### Comparing `dj-accounts-3.0.9/dj_accounts.egg-info/PKG-INFO` & `dj-accounts-3.1.0/dj_accounts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.9
+Version: 3.1.0
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
 Description: ## Installation
```

### Comparing `dj-accounts-3.0.9/dj_accounts.egg-info/SOURCES.txt` & `dj-accounts-3.1.0/dj_accounts.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 accounts_pkg/settings.py
 accounts_pkg/urls.py
 accounts_pkg/wsgi.py
 dj_accounts/__init__.py
 dj_accounts/apps.py
 dj_accounts/backends.py
 dj_accounts/forms.py
-dj_accounts/serializers.py
 dj_accounts/utils.py
 dj_accounts/verify_phone.py
 dj_accounts/views.py
 dj_accounts/views_api.py
 dj_accounts.egg-info/PKG-INFO
 dj_accounts.egg-info/SOURCES.txt
 dj_accounts.egg-info/dependency_links.txt
@@ -64,17 +63,17 @@
 dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
 dj_accounts/templates/dj_accounts/partials/fields/username.html
 dj_accounts/tests/__init__.py
 dj_accounts/tests/apps.py
 dj_accounts/tests/factories.py
 dj_accounts/tests/mocks.py
 dj_accounts/tests/models.py
+dj_accounts/tests/profile_handlers.py
 dj_accounts/tests/test_backends.py
 dj_accounts/tests/test_forms.py
-dj_accounts/tests/test_serializers.py
 dj_accounts/tests/test_tokens.py
 dj_accounts/tests/test_urls.py
 dj_accounts/tests/test_verify_phone.py
 dj_accounts/tests/test_view_api.py
 dj_accounts/tests/test_views.py
 dj_accounts/tests/migrations/0001_initial.py
 dj_accounts/tests/migrations/__init__.py
```

### Comparing `dj-accounts-3.0.9/docs/PhoneVerificationService.md` & `dj-accounts-3.1.0/docs/PhoneVerificationService.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/docs/index.md` & `dj-accounts-3.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.9/setup.cfg` & `dj-accounts-3.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-accounts
-version = 3.0.9
+version = 3.1.0
 author = fritill
 author_email = dev@fritill.com
 description = this application is for handling all auth operations
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritill-team/django-accounts
 license = MIT
```

