# Comparing `tmp/azure-identity-1.9.0.zip` & `tmp/azure-identity-1.9.0b1.zip`

## zipinfo {}

```diff
@@ -1,190 +1,190 @@
-Zip file size: 311782 bytes, number of entries: 188
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/
--rw-rw-r--  2.0 unx      147 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/MANIFEST.in
--rw-rw-r--  2.0 unx    33027 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/CHANGELOG.md
--rw-rw-r--  2.0 unx    19695 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/README.md
--rw-rw-r--  2.0 unx     1073 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/LICENSE
--rw-rw-r--  2.0 unx    23499 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     2664 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/setup.py
--rw-rw-r--  2.0 unx     5784 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/migration_guide.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/setup.cfg
--rw-rw-r--  2.0 unx    62197 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/PKG-INFO
--rw-rw-r--  2.0 unx     2339 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/samples/custom_credentials.py
--rw-rw-r--  2.0 unx     2511 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/samples/key_vault_cert.py
--rw-rw-r--  2.0 unx     3142 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/samples/user_authentication.py
--rw-rw-r--  2.0 unx     1786 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/samples/control_interactive_prompts.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/vscode-live/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/pod-identity/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/managed-identity-live/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/perfstress_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/azure-functions/
--rw-rw-r--  2.0 unx     8695 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_imds_credential.py
--rw-rw-r--  2.0 unx     8705 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_username_password_credential.py
--rw-rw-r--  2.0 unx     1980 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_auth_record.py
--rw-rw-r--  2.0 unx     9698 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_cli_credential_async.py
--rw-rw-r--  2.0 unx     1663 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_azure_application_async.py
--rw-rw-r--  2.0 unx    12176 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_client_secret_credential_async.py
--rw-rw-r--  2.0 unx    38900 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_managed_identity_async.py
--rw-rw-r--  2.0 unx     8137 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_cli_credential.py
--rw-rw-r--  2.0 unx     1508 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/recorded_test_case.py
--rw-rw-r--  2.0 unx    17224 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_certificate_credential.py
--rw-rw-r--  2.0 unx    14009 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_interactive_credential.py
--rw-rw-r--  2.0 unx     2015 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/credscan_ignore.py
--rw-rw-r--  2.0 unx     9405 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_obo_async.py
--rw-rw-r--  2.0 unx     4098 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_context_manager.py
--rw-rw-r--  2.0 unx     1834 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_live_async.py
--rw-rw-r--  2.0 unx     2660 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_app_service.py
--rw-rw-r--  2.0 unx     5997 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_cae.py
--rw-rw-r--  2.0 unx     3603 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/recording_processors.py
--rw-rw-r--  2.0 unx     8934 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_obo.py
--rw-rw-r--  2.0 unx     1616 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/helpers_async.py
--rw-rw-r--  2.0 unx     5302 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_application_credential_async.py
--rw-rw-r--  2.0 unx     4330 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_get_token_mixin_async.py
--rw-rw-r--  2.0 unx    10919 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_client_secret_credential.py
--rw-rw-r--  2.0 unx     7663 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_auth_code_async.py
--rw-rw-r--  2.0 unx     3687 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_chained_credential.py
--rw-rw-r--  2.0 unx     6842 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_auth_code.py
--rw-rw-r--  2.0 unx     1769 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_msal_client.py
--rw-rw-r--  2.0 unx     3724 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_chained_token_credential_async.py
--rw-rw-r--  2.0 unx    14622 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_browser_credential.py
--rw-rw-r--  2.0 unx    15557 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_default_async.py
--rw-rw-r--  2.0 unx     4919 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_managed_identity_client_async.py
--rw-rw-r--  2.0 unx    29643 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_shared_cache_credential_async.py
--rw-rw-r--  2.0 unx     4052 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_managed_identity_client.py
--rw-rw-r--  2.0 unx    13160 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_vscode_credential_async.py
--rw-rw-r--  2.0 unx    13059 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_device_code_credential.py
--rw-rw-r--  2.0 unx    11968 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_aad_client_async.py
--rw-rw-r--  2.0 unx     2555 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_live.py
--rw-rw-r--  2.0 unx     9850 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_imds_credential_async.py
--rw-rw-r--  2.0 unx     4220 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_get_token_mixin.py
--rw-rw-r--  2.0 unx     1731 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_azure_application.py
--rw-rw-r--  2.0 unx     6211 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_environment_credential_async.py
--rw-rw-r--  2.0 unx    14416 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_powershell_credential_async.py
--rw-rw-r--  2.0 unx     2286 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_persistent_cache.py
--rw-rw-r--  2.0 unx     2792 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_app_service_async.py
--rw-rw-r--  2.0 unx    39984 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_managed_identity.py
--rw-rw-r--  2.0 unx    19349 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_default.py
--rw-rw-r--  2.0 unx    14061 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_powershell_credential.py
--rw-rw-r--  2.0 unx     7491 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/helpers.py
--rw-rw-r--  2.0 unx     2075 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_authority.py
--rw-rw-r--  2.0 unx    13411 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_vscode_credential.py
--rw-rw-r--  2.0 unx     5501 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_application_credential.py
--rw-rw-r--  2.0 unx    11668 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_aad_client.py
--rw-rw-r--  2.0 unx     5483 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_environment_credential.py
--rw-rw-r--  2.0 unx    13196 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_certificate_credential_async.py
--rw-rw-r--  2.0 unx    41723 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/test_shared_cache_credential.py
--rw-rw-r--  2.0 unx      398 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/vscode-live/run-test.py
--rw-rw-r--  2.0 unx     3215 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/pod-identity/run-test.py
--rw-rw-r--  2.0 unx     1113 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell.py
--rw-rw-r--  2.0 unx      822 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live_async.py
--rw-rw-r--  2.0 unx      765 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live.py
--rw-rw-r--  2.0 unx     2013 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/managed-identity-live/conftest.py
--rw-rw-r--  2.0 unx     1186 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell_async.py
--rw-rw-r--  2.0 unx      309 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1421 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/perfstress_tests/memory_cache_read.py
--rw-rw-r--  2.0 unx     1644 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/perfstress_tests/persistent_cache_read.py
--rw-rw-r--  2.0 unx     1727 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/perfstress_tests/bearer_token_auth_policy.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/azure-functions/RunTest/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/tests/azure-functions/RunAsyncTest/
--rw-rw-r--  2.0 unx     1277 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/azure-functions/RunTest/__init__.py
--rw-rw-r--  2.0 unx     1297 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/tests/azure-functions/RunAsyncTest/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/
--rw-rw-r--  2.0 unx      267 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/_internal/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/_credentials/
--rw-rw-r--  2.0 unx     1699 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/__init__.py
--rw-rw-r--  2.0 unx      169 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_version.py
--rw-rw-r--  2.0 unx     1947 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_constants.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/py.typed
--rw-rw-r--  2.0 unx     2772 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_auth_record.py
--rw-rw-r--  2.0 unx     5295 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_persistent_cache.py
--rw-rw-r--  2.0 unx     1727 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_exceptions.py
--rw-rw-r--  2.0 unx     2627 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_enums.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/aio/_internal/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-04 15:10 azure-identity-1.9.0/azure/identity/aio/_credentials/
--rw-rw-r--  2.0 unx     1034 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/__init__.py
--rw-rw-r--  2.0 unx      526 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/__init__.py
--rw-rw-r--  2.0 unx     4366 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/aad_client.py
--rw-rw-r--  2.0 unx     2729 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/decorators.py
--rw-rw-r--  2.0 unx     3474 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/get_token_mixin.py
--rw-rw-r--  2.0 unx     2051 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_base.py
--rw-rw-r--  2.0 unx     1609 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_client.py
--rw-rw-r--  2.0 unx     3818 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/chained.py
--rw-rw-r--  2.0 unx     3645 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/certificate.py
--rw-rw-r--  2.0 unx     4463 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/azure_cli.py
--rw-rw-r--  2.0 unx     1220 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/__init__.py
--rw-rw-r--  2.0 unx     4555 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/azure_powershell.py
--rw-rw-r--  2.0 unx     5971 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/managed_identity.py
--rw-rw-r--  2.0 unx     3872 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/imds.py
--rw-rw-r--  2.0 unx      871 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/app_service.py
--rw-rw-r--  2.0 unx     2950 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/client_secret.py
--rw-rw-r--  2.0 unx     4004 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/shared_cache.py
--rw-rw-r--  2.0 unx     5080 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/environment.py
--rw-rw-r--  2.0 unx     2282 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/client_assertion.py
--rw-rw-r--  2.0 unx     3639 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/vscode.py
--rw-rw-r--  2.0 unx     4230 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/application.py
--rw-rw-r--  2.0 unx      794 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/token_exchange.py
--rw-rw-r--  2.0 unx     5668 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/on_behalf_of.py
--rw-rw-r--  2.0 unx     4563 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/authorization_code.py
--rw-rw-r--  2.0 unx     1953 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/azure_arc.py
--rw-rw-r--  2.0 unx      862 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/azure_ml.py
--rw-rw-r--  2.0 unx     1062 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/cloud_shell.py
--rw-rw-r--  2.0 unx      880 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/service_fabric.py
--rw-rw-r--  2.0 unx     8203 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/aio/_credentials/default.py
--rw-rw-r--  2.0 unx      319 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/user_agent.py
--rw-rw-r--  2.0 unx     2543 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/pipeline.py
--rw-rw-r--  2.0 unx     2933 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/linux_vscode_adapter.py
--rw-rw-r--  2.0 unx     4113 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/__init__.py
--rw-rw-r--  2.0 unx     9744 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/interactive.py
--rw-rw-r--  2.0 unx     2426 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/win_vscode_adapter.py
--rw-rw-r--  2.0 unx     3340 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/aad_client.py
--rw-rw-r--  2.0 unx     2533 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/auth_code_redirect_handler.py
--rw-rw-r--  2.0 unx     3147 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/decorators.py
--rw-rw-r--  2.0 unx     3662 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/get_token_mixin.py
--rw-rw-r--  2.0 unx     5052 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/msal_client.py
--rw-rw-r--  2.0 unx    12089 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/aad_client_base.py
--rw-rw-r--  2.0 unx     1184 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/macos_vscode_adapter.py
--rw-rw-r--  2.0 unx     1710 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/client_credential_base.py
--rw-rw-r--  2.0 unx     2084 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/managed_identity_base.py
--rw-rw-r--  2.0 unx     3091 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/msal_credentials.py
--rw-rw-r--  2.0 unx     5046 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/managed_identity_client.py
--rw-rw-r--  2.0 unx     9756 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/shared_token_cache.py
--rw-rw-r--  2.0 unx     1944 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_internal/aadclient_certificate.py
--rw-rw-r--  2.0 unx     5285 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/device_code.py
--rw-rw-r--  2.0 unx     4207 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/chained.py
--rw-rw-r--  2.0 unx     7501 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/certificate.py
--rw-rw-r--  2.0 unx     5928 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/azure_cli.py
--rw-rw-r--  2.0 unx     1494 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/__init__.py
--rw-rw-r--  2.0 unx     5324 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/silent.py
--rw-rw-r--  2.0 unx     6603 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/azure_powershell.py
--rw-rw-r--  2.0 unx     3054 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/user_password.py
--rw-rw-r--  2.0 unx     5724 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/managed_identity.py
--rw-rw-r--  2.0 unx     4592 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/imds.py
--rw-rw-r--  2.0 unx     1792 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/app_service.py
--rw-rw-r--  2.0 unx     1950 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/client_secret.py
--rw-rw-r--  2.0 unx     5283 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/shared_cache.py
--rw-rw-r--  2.0 unx     6696 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/environment.py
--rw-rw-r--  2.0 unx     2301 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/client_assertion.py
--rw-rw-r--  2.0 unx     7772 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/vscode.py
--rw-rw-r--  2.0 unx     4288 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/application.py
--rw-rw-r--  2.0 unx     1356 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/token_exchange.py
--rw-rw-r--  2.0 unx     5859 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/on_behalf_of.py
--rw-rw-r--  2.0 unx     4664 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/authorization_code.py
--rw-rw-r--  2.0 unx     3816 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/azure_arc.py
--rw-rw-r--  2.0 unx     3313 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/azure_ml.py
--rw-rw-r--  2.0 unx     1274 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/cloud_shell.py
--rw-rw-r--  2.0 unx     6730 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/browser.py
--rw-rw-r--  2.0 unx     1822 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/service_fabric.py
--rw-rw-r--  2.0 unx     9862 b- defN 22-Apr-04 15:09 azure-identity-1.9.0/azure/identity/_credentials/default.py
--rw-rw-r--  2.0 unx        6 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    62197 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     6379 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       99 b- defN 22-Apr-04 15:10 azure-identity-1.9.0/azure_identity.egg-info/requires.txt
-188 files, 1077931 bytes uncompressed, 276384 bytes compressed:  74.4%
+Zip file size: 307233 bytes, number of entries: 188
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/setup.cfg
+-rw-rw-r--  2.0 unx     2651 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/setup.py
+-rw-rw-r--  2.0 unx    13845 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx    19393 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/README.md
+-rw-rw-r--  2.0 unx    61050 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx     5784 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/migration_guide.md
+-rw-rw-r--  2.0 unx    32329 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx      147 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx        1 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     6379 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx       99 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    61050 b- defN 22-Mar-07 20:45 azure-identity-1.9.0b1/azure_identity.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/vscode-live/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/azure-functions/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/managed-identity-live/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/perfstress_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/pod-identity/
+-rw-rw-r--  2.0 unx    12176 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_client_secret_credential_async.py
+-rw-rw-r--  2.0 unx     9405 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_obo_async.py
+-rw-rw-r--  2.0 unx     2660 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_app_service.py
+-rw-rw-r--  2.0 unx    14416 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_powershell_credential_async.py
+-rw-rw-r--  2.0 unx     5483 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_environment_credential.py
+-rw-rw-r--  2.0 unx     1769 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_msal_client.py
+-rw-rw-r--  2.0 unx    11968 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_aad_client_async.py
+-rw-rw-r--  2.0 unx    41723 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_shared_cache_credential.py
+-rw-rw-r--  2.0 unx    10919 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_client_secret_credential.py
+-rw-rw-r--  2.0 unx     4098 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_context_manager.py
+-rw-rw-r--  2.0 unx     8695 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_imds_credential.py
+-rw-rw-r--  2.0 unx    14061 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_powershell_credential.py
+-rw-rw-r--  2.0 unx     5501 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_application_credential.py
+-rw-rw-r--  2.0 unx    29643 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_shared_cache_credential_async.py
+-rw-rw-r--  2.0 unx     8705 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_username_password_credential.py
+-rw-rw-r--  2.0 unx     5997 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_cae.py
+-rw-rw-r--  2.0 unx     4220 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_get_token_mixin.py
+-rw-rw-r--  2.0 unx     7663 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_auth_code_async.py
+-rw-rw-r--  2.0 unx     9698 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_cli_credential_async.py
+-rw-rw-r--  2.0 unx    13411 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_vscode_credential.py
+-rw-rw-r--  2.0 unx     4330 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_get_token_mixin_async.py
+-rw-rw-r--  2.0 unx     2075 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_authority.py
+-rw-rw-r--  2.0 unx     9850 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_imds_credential_async.py
+-rw-rw-r--  2.0 unx     3724 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_chained_token_credential_async.py
+-rw-rw-r--  2.0 unx    13160 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_vscode_credential_async.py
+-rw-rw-r--  2.0 unx     4919 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_managed_identity_client_async.py
+-rw-rw-r--  2.0 unx     1616 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/helpers_async.py
+-rw-rw-r--  2.0 unx     2015 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/credscan_ignore.py
+-rw-rw-r--  2.0 unx    17224 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_certificate_credential.py
+-rw-rw-r--  2.0 unx     2555 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_live.py
+-rw-rw-r--  2.0 unx     1834 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_live_async.py
+-rw-rw-r--  2.0 unx     1731 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_azure_application.py
+-rw-rw-r--  2.0 unx    13059 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_device_code_credential.py
+-rw-rw-r--  2.0 unx    13196 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_certificate_credential_async.py
+-rw-rw-r--  2.0 unx     6211 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_environment_credential_async.py
+-rw-rw-r--  2.0 unx    14009 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_interactive_credential.py
+-rw-rw-r--  2.0 unx     4052 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_managed_identity_client.py
+-rw-rw-r--  2.0 unx     1508 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/recorded_test_case.py
+-rw-rw-r--  2.0 unx    38101 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_managed_identity.py
+-rw-rw-r--  2.0 unx     6842 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_auth_code.py
+-rw-rw-r--  2.0 unx    14622 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_browser_credential.py
+-rw-rw-r--  2.0 unx     3687 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_chained_credential.py
+-rw-rw-r--  2.0 unx     7491 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/helpers.py
+-rw-rw-r--  2.0 unx     2286 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_persistent_cache.py
+-rw-rw-r--  2.0 unx     5302 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_application_credential_async.py
+-rw-rw-r--  2.0 unx    11668 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_aad_client.py
+-rw-rw-r--  2.0 unx     8934 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_obo.py
+-rw-rw-r--  2.0 unx     1663 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_azure_application_async.py
+-rw-rw-r--  2.0 unx     2792 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_app_service_async.py
+-rw-rw-r--  2.0 unx    19349 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_default.py
+-rw-rw-r--  2.0 unx    36908 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_managed_identity_async.py
+-rw-rw-r--  2.0 unx     3603 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/recording_processors.py
+-rw-rw-r--  2.0 unx     8137 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_cli_credential.py
+-rw-rw-r--  2.0 unx    15557 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_default_async.py
+-rw-rw-r--  2.0 unx     1980 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/test_auth_record.py
+-rw-rw-r--  2.0 unx      398 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/vscode-live/run-test.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/azure-functions/RunTest/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/tests/azure-functions/RunAsyncTest/
+-rw-rw-r--  2.0 unx     1277 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/azure-functions/RunTest/__init__.py
+-rw-rw-r--  2.0 unx     1297 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/azure-functions/RunAsyncTest/__init__.py
+-rw-rw-r--  2.0 unx     1186 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell_async.py
+-rw-rw-r--  2.0 unx      822 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live_async.py
+-rw-rw-r--  2.0 unx      765 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live.py
+-rw-rw-r--  2.0 unx     1113 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell.py
+-rw-rw-r--  2.0 unx     2013 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/managed-identity-live/conftest.py
+-rw-rw-r--  2.0 unx     1644 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/perfstress_tests/persistent_cache_read.py
+-rw-rw-r--  2.0 unx     1727 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/perfstress_tests/bearer_token_auth_policy.py
+-rw-rw-r--  2.0 unx     1421 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/perfstress_tests/memory_cache_read.py
+-rw-rw-r--  2.0 unx      309 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     3215 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/tests/pod-identity/run-test.py
+-rw-rw-r--  2.0 unx     1786 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/samples/control_interactive_prompts.py
+-rw-rw-r--  2.0 unx     2511 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/samples/key_vault_cert.py
+-rw-rw-r--  2.0 unx     2339 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/samples/custom_credentials.py
+-rw-rw-r--  2.0 unx     3142 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/samples/user_authentication.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/
+-rw-rw-r--  2.0 unx      267 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/_internal/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/_credentials/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/aio/
+-rw-rw-r--  2.0 unx     1947 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_constants.py
+-rw-rw-r--  2.0 unx     2627 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_enums.py
+-rw-rw-r--  2.0 unx     2772 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_auth_record.py
+-rw-rw-r--  2.0 unx     1727 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_exceptions.py
+-rw-rw-r--  2.0 unx      171 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_version.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/py.typed
+-rw-rw-r--  2.0 unx     5295 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_persistent_cache.py
+-rw-rw-r--  2.0 unx     1699 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/__init__.py
+-rw-rw-r--  2.0 unx     1928 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/decorators.py
+-rw-rw-r--  2.0 unx     2933 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/linux_vscode_adapter.py
+-rw-rw-r--  2.0 unx     1184 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/macos_vscode_adapter.py
+-rw-rw-r--  2.0 unx     2533 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/auth_code_redirect_handler.py
+-rw-rw-r--  2.0 unx     3087 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/msal_credentials.py
+-rw-rw-r--  2.0 unx     9744 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/interactive.py
+-rw-rw-r--  2.0 unx     2543 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/pipeline.py
+-rw-rw-r--  2.0 unx     5164 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_client.py
+-rw-rw-r--  2.0 unx      319 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/user_agent.py
+-rw-rw-r--  2.0 unx     3662 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/get_token_mixin.py
+-rw-rw-r--  2.0 unx     1710 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/client_credential_base.py
+-rw-rw-r--  2.0 unx     3340 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/aad_client.py
+-rw-rw-r--  2.0 unx    11246 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/aad_client_base.py
+-rw-rw-r--  2.0 unx     9756 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/shared_token_cache.py
+-rw-rw-r--  2.0 unx     1944 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/aadclient_certificate.py
+-rw-rw-r--  2.0 unx     4946 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/msal_client.py
+-rw-rw-r--  2.0 unx     2084 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_base.py
+-rw-rw-r--  2.0 unx     2426 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/win_vscode_adapter.py
+-rw-rw-r--  2.0 unx     4113 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_internal/__init__.py
+-rw-rw-r--  2.0 unx     5285 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/device_code.py
+-rw-rw-r--  2.0 unx     6603 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/azure_powershell.py
+-rw-rw-r--  2.0 unx     3816 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/azure_arc.py
+-rw-rw-r--  2.0 unx     6058 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/managed_identity.py
+-rw-rw-r--  2.0 unx     4664 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/authorization_code.py
+-rw-rw-r--  2.0 unx     5928 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/azure_cli.py
+-rw-rw-r--  2.0 unx     2355 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/client_assertion.py
+-rw-rw-r--  2.0 unx     1950 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/client_secret.py
+-rw-rw-r--  2.0 unx     4288 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/application.py
+-rw-rw-r--  2.0 unx     5859 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/on_behalf_of.py
+-rw-rw-r--  2.0 unx     4207 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/chained.py
+-rw-rw-r--  2.0 unx     6027 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/environment.py
+-rw-rw-r--  2.0 unx     5283 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/shared_cache.py
+-rw-rw-r--  2.0 unx     1956 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/azure_ml.py
+-rw-rw-r--  2.0 unx     1822 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/service_fabric.py
+-rw-rw-r--  2.0 unx     7501 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/certificate.py
+-rw-rw-r--  2.0 unx     1892 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/app_service.py
+-rw-rw-r--  2.0 unx     7435 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/vscode.py
+-rw-rw-r--  2.0 unx     3054 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/user_password.py
+-rw-rw-r--  2.0 unx     9862 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/default.py
+-rw-rw-r--  2.0 unx     1274 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/cloud_shell.py
+-rw-rw-r--  2.0 unx     5324 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/silent.py
+-rw-rw-r--  2.0 unx     1365 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/token_exchange.py
+-rw-rw-r--  2.0 unx     6730 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/browser.py
+-rw-rw-r--  2.0 unx     4619 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/imds.py
+-rw-rw-r--  2.0 unx     1494 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/_credentials/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/aio/_internal/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-07 20:45 azure-identity-1.9.0b1/azure/identity/aio/_credentials/
+-rw-rw-r--  2.0 unx      970 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/__init__.py
+-rw-rw-r--  2.0 unx     1579 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/decorators.py
+-rw-rw-r--  2.0 unx     1609 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_client.py
+-rw-rw-r--  2.0 unx     3474 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/get_token_mixin.py
+-rw-rw-r--  2.0 unx     3866 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/aad_client.py
+-rw-rw-r--  2.0 unx     2051 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_base.py
+-rw-rw-r--  2.0 unx      526 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_internal/__init__.py
+-rw-rw-r--  2.0 unx     4555 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_powershell.py
+-rw-rw-r--  2.0 unx     1953 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_arc.py
+-rw-rw-r--  2.0 unx     5971 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/managed_identity.py
+-rw-rw-r--  2.0 unx     4563 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/authorization_code.py
+-rw-rw-r--  2.0 unx     4463 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_cli.py
+-rw-rw-r--  2.0 unx     2336 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_assertion.py
+-rw-rw-r--  2.0 unx     2950 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_secret.py
+-rw-rw-r--  2.0 unx     4230 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/application.py
+-rw-rw-r--  2.0 unx     5609 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/on_behalf_of.py
+-rw-rw-r--  2.0 unx     3818 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/chained.py
+-rw-rw-r--  2.0 unx     4634 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/environment.py
+-rw-rw-r--  2.0 unx     4004 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/shared_cache.py
+-rw-rw-r--  2.0 unx      862 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_ml.py
+-rw-rw-r--  2.0 unx      880 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/service_fabric.py
+-rw-rw-r--  2.0 unx     3645 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/certificate.py
+-rw-rw-r--  2.0 unx      871 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/app_service.py
+-rw-rw-r--  2.0 unx     3310 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/vscode.py
+-rw-rw-r--  2.0 unx     8203 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/default.py
+-rw-rw-r--  2.0 unx     1062 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/cloud_shell.py
+-rw-rw-r--  2.0 unx      803 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/token_exchange.py
+-rw-rw-r--  2.0 unx     3872 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/imds.py
+-rw-rw-r--  2.0 unx     1131 b- defN 22-Mar-07 20:44 azure-identity-1.9.0b1/azure/identity/aio/_credentials/__init__.py
+188 files, 1054630 bytes uncompressed, 271083 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,565 +1,565 @@
-Filename: azure-identity-1.9.0/
+Filename: azure-identity-1.9.0b1/
 Comment: 
 
-Filename: azure-identity-1.9.0/samples/
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/
+Filename: azure-identity-1.9.0b1/tests/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/
+Filename: azure-identity-1.9.0b1/samples/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/
+Filename: azure-identity-1.9.0b1/azure/
 Comment: 
 
-Filename: azure-identity-1.9.0/MANIFEST.in
+Filename: azure-identity-1.9.0b1/LICENSE
 Comment: 
 
-Filename: azure-identity-1.9.0/CHANGELOG.md
+Filename: azure-identity-1.9.0b1/setup.cfg
 Comment: 
 
-Filename: azure-identity-1.9.0/README.md
+Filename: azure-identity-1.9.0b1/setup.py
 Comment: 
 
-Filename: azure-identity-1.9.0/LICENSE
+Filename: azure-identity-1.9.0b1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-identity-1.9.0/TROUBLESHOOTING.md
+Filename: azure-identity-1.9.0b1/README.md
 Comment: 
 
-Filename: azure-identity-1.9.0/setup.py
+Filename: azure-identity-1.9.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-identity-1.9.0/migration_guide.md
+Filename: azure-identity-1.9.0b1/migration_guide.md
 Comment: 
 
-Filename: azure-identity-1.9.0/setup.cfg
+Filename: azure-identity-1.9.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-identity-1.9.0/PKG-INFO
+Filename: azure-identity-1.9.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-identity-1.9.0/samples/custom_credentials.py
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-identity-1.9.0/samples/key_vault_cert.py
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-identity-1.9.0/samples/user_authentication.py
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-identity-1.9.0/samples/control_interactive_prompts.py
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/vscode-live/
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/requires.txt
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/pod-identity/
+Filename: azure-identity-1.9.0b1/azure_identity.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/
+Filename: azure-identity-1.9.0b1/tests/vscode-live/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/perfstress_tests/
+Filename: azure-identity-1.9.0b1/tests/azure-functions/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/azure-functions/
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_imds_credential.py
+Filename: azure-identity-1.9.0b1/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_username_password_credential.py
+Filename: azure-identity-1.9.0b1/tests/pod-identity/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_auth_record.py
+Filename: azure-identity-1.9.0b1/tests/test_client_secret_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_cli_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_obo_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_azure_application_async.py
+Filename: azure-identity-1.9.0b1/tests/test_app_service.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_client_secret_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_powershell_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_managed_identity_async.py
+Filename: azure-identity-1.9.0b1/tests/test_environment_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_cli_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_msal_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/recorded_test_case.py
+Filename: azure-identity-1.9.0b1/tests/test_aad_client_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_certificate_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_shared_cache_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_interactive_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_client_secret_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/credscan_ignore.py
+Filename: azure-identity-1.9.0b1/tests/test_context_manager.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_obo_async.py
+Filename: azure-identity-1.9.0b1/tests/test_imds_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_context_manager.py
+Filename: azure-identity-1.9.0b1/tests/test_powershell_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_live_async.py
+Filename: azure-identity-1.9.0b1/tests/test_application_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_app_service.py
+Filename: azure-identity-1.9.0b1/tests/test_shared_cache_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_cae.py
+Filename: azure-identity-1.9.0b1/tests/test_username_password_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/recording_processors.py
+Filename: azure-identity-1.9.0b1/tests/test_cae.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_obo.py
+Filename: azure-identity-1.9.0b1/tests/test_get_token_mixin.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/helpers_async.py
+Filename: azure-identity-1.9.0b1/tests/test_auth_code_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_application_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_cli_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_get_token_mixin_async.py
+Filename: azure-identity-1.9.0b1/tests/test_vscode_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_client_secret_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_get_token_mixin_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_auth_code_async.py
+Filename: azure-identity-1.9.0b1/tests/test_authority.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_chained_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_imds_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_auth_code.py
+Filename: azure-identity-1.9.0b1/tests/test_chained_token_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_msal_client.py
+Filename: azure-identity-1.9.0b1/tests/test_vscode_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_chained_token_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_managed_identity_client_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_browser_credential.py
+Filename: azure-identity-1.9.0b1/tests/helpers_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_default_async.py
+Filename: azure-identity-1.9.0b1/tests/credscan_ignore.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_managed_identity_client_async.py
+Filename: azure-identity-1.9.0b1/tests/test_certificate_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_shared_cache_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_live.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_managed_identity_client.py
+Filename: azure-identity-1.9.0b1/tests/test_live_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_vscode_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_azure_application.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_device_code_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_device_code_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_aad_client_async.py
+Filename: azure-identity-1.9.0b1/tests/test_certificate_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_live.py
+Filename: azure-identity-1.9.0b1/tests/test_environment_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_imds_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_interactive_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_get_token_mixin.py
+Filename: azure-identity-1.9.0b1/tests/test_managed_identity_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_azure_application.py
+Filename: azure-identity-1.9.0b1/tests/recorded_test_case.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_environment_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_managed_identity.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_powershell_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/test_auth_code.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_persistent_cache.py
+Filename: azure-identity-1.9.0b1/tests/test_browser_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_app_service_async.py
+Filename: azure-identity-1.9.0b1/tests/test_chained_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_managed_identity.py
+Filename: azure-identity-1.9.0b1/tests/helpers.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_default.py
+Filename: azure-identity-1.9.0b1/tests/test_persistent_cache.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_powershell_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_application_credential_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/helpers.py
+Filename: azure-identity-1.9.0b1/tests/test_aad_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_authority.py
+Filename: azure-identity-1.9.0b1/tests/test_obo.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_vscode_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_azure_application_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_application_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_app_service_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_aad_client.py
+Filename: azure-identity-1.9.0b1/tests/test_default.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_environment_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_managed_identity_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_certificate_credential_async.py
+Filename: azure-identity-1.9.0b1/tests/recording_processors.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/test_shared_cache_credential.py
+Filename: azure-identity-1.9.0b1/tests/test_cli_credential.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/vscode-live/run-test.py
+Filename: azure-identity-1.9.0b1/tests/test_default_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/pod-identity/run-test.py
+Filename: azure-identity-1.9.0b1/tests/test_auth_record.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell.py
+Filename: azure-identity-1.9.0b1/tests/vscode-live/run-test.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live_async.py
+Filename: azure-identity-1.9.0b1/tests/azure-functions/RunTest/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live.py
+Filename: azure-identity-1.9.0b1/tests/azure-functions/RunAsyncTest/
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/conftest.py
+Filename: azure-identity-1.9.0b1/tests/azure-functions/RunTest/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell_async.py
+Filename: azure-identity-1.9.0b1/tests/azure-functions/RunAsyncTest/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/perfstress_tests/__init__.py
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/perfstress_tests/memory_cache_read.py
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live_async.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/perfstress_tests/persistent_cache_read.py
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/perfstress_tests/bearer_token_auth_policy.py
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/azure-functions/RunTest/
+Filename: azure-identity-1.9.0b1/tests/managed-identity-live/conftest.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/azure-functions/RunAsyncTest/
+Filename: azure-identity-1.9.0b1/tests/perfstress_tests/persistent_cache_read.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/azure-functions/RunTest/__init__.py
+Filename: azure-identity-1.9.0b1/tests/perfstress_tests/bearer_token_auth_policy.py
 Comment: 
 
-Filename: azure-identity-1.9.0/tests/azure-functions/RunAsyncTest/__init__.py
+Filename: azure-identity-1.9.0b1/tests/perfstress_tests/memory_cache_read.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/
+Filename: azure-identity-1.9.0b1/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/__init__.py
+Filename: azure-identity-1.9.0b1/tests/pod-identity/run-test.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/
+Filename: azure-identity-1.9.0b1/samples/control_interactive_prompts.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/
+Filename: azure-identity-1.9.0b1/samples/key_vault_cert.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/
+Filename: azure-identity-1.9.0b1/samples/custom_credentials.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/__init__.py
+Filename: azure-identity-1.9.0b1/samples/user_authentication.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_version.py
+Filename: azure-identity-1.9.0b1/azure/identity/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_constants.py
+Filename: azure-identity-1.9.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/py.typed
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_auth_record.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_persistent_cache.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_exceptions.py
+Filename: azure-identity-1.9.0b1/azure/identity/_constants.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_enums.py
+Filename: azure-identity-1.9.0b1/azure/identity/_enums.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/
+Filename: azure-identity-1.9.0b1/azure/identity/_auth_record.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/
+Filename: azure-identity-1.9.0b1/azure/identity/_exceptions.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/__init__.py
+Filename: azure-identity-1.9.0b1/azure/identity/_version.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/__init__.py
+Filename: azure-identity-1.9.0b1/azure/identity/py.typed
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/aad_client.py
+Filename: azure-identity-1.9.0b1/azure/identity/_persistent_cache.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/decorators.py
+Filename: azure-identity-1.9.0b1/azure/identity/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/get_token_mixin.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/decorators.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_base.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/linux_vscode_adapter.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_client.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/macos_vscode_adapter.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/chained.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/auth_code_redirect_handler.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/certificate.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/msal_credentials.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/azure_cli.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/interactive.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/__init__.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/pipeline.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/azure_powershell.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/managed_identity.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/user_agent.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/imds.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/get_token_mixin.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/app_service.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/client_credential_base.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/client_secret.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/aad_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/shared_cache.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/aad_client_base.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/environment.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/shared_token_cache.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/client_assertion.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/aadclient_certificate.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/vscode.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/msal_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/application.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_base.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/token_exchange.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/win_vscode_adapter.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/on_behalf_of.py
+Filename: azure-identity-1.9.0b1/azure/identity/_internal/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/authorization_code.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/device_code.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/azure_arc.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/azure_powershell.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/azure_ml.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/azure_arc.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/cloud_shell.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/managed_identity.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/service_fabric.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/authorization_code.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/aio/_credentials/default.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/azure_cli.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/user_agent.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/client_assertion.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/pipeline.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/client_secret.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/linux_vscode_adapter.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/application.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/__init__.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/on_behalf_of.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/interactive.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/chained.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/win_vscode_adapter.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/environment.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/aad_client.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/shared_cache.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/auth_code_redirect_handler.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/azure_ml.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/decorators.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/service_fabric.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/get_token_mixin.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/certificate.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/msal_client.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/app_service.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/aad_client_base.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/vscode.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/macos_vscode_adapter.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/user_password.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/client_credential_base.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/default.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/managed_identity_base.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/cloud_shell.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/msal_credentials.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/silent.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/managed_identity_client.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/token_exchange.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/shared_token_cache.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/browser.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_internal/aadclient_certificate.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/imds.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/device_code.py
+Filename: azure-identity-1.9.0b1/azure/identity/_credentials/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/chained.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/certificate.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/azure_cli.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/__init__.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/decorators.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/silent.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/azure_powershell.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/get_token_mixin.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/user_password.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/aad_client.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/managed_identity.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_base.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/imds.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_internal/__init__.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/app_service.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_powershell.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/client_secret.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_arc.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/shared_cache.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/managed_identity.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/environment.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/authorization_code.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/client_assertion.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_cli.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/vscode.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_assertion.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/application.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_secret.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/token_exchange.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/application.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/on_behalf_of.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/on_behalf_of.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/authorization_code.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/chained.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/azure_arc.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/environment.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/azure_ml.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/shared_cache.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/cloud_shell.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_ml.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/browser.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/service_fabric.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/service_fabric.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/certificate.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure/identity/_credentials/default.py
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/app_service.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/top_level.txt
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/vscode.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/PKG-INFO
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/default.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/not-zip-safe
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/cloud_shell.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/dependency_links.txt
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/token_exchange.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/SOURCES.txt
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/imds.py
 Comment: 
 
-Filename: azure-identity-1.9.0/azure_identity.egg-info/requires.txt
+Filename: azure-identity-1.9.0b1/azure/identity/aio/_credentials/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-identity-1.9.0/CHANGELOG.md` & `azure-identity-1.9.0b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,9 @@
 # Release History
 
-## 1.9.0 (2022-04-05)
-
-### Features Added
-
-- Added PII logging if logging.DEBUG is enabled.    ([#23203](https://github.com/Azure/azure-sdk-for-python/issues/23203))
-
-### Breaking Changes
-
-- `validate_authority` support is not available in 1.9.0.
-
-### Bugs Fixed
-
-- Added check on `content` from msal response.    ([#23483](https://github.com/Azure/azure-sdk-for-python/issues/23483))
-- Fixed the issue that async OBO credential does not refresh correctly.    ([#21981](https://github.com/Azure/azure-sdk-for-python/issues/21981))
-
-### Other Changes
-
-- Removed `resource_id`, please use `identity_config` instead.
-- Renamed argument name `get_assertion` to `func` for `ClientAssertionCredential`.
-
 ## 1.9.0b1 (2022-03-08)
 
 ### Features Added
 
 - Added `validate_authority` support for msal client  ([#22625](https://github.com/Azure/azure-sdk-for-python/issues/22625))
 - Added `resource_id` support for user-assigned managed identity  ([#22329](https://github.com/Azure/azure-sdk-for-python/issues/22329))
 - Added `ClientAssertionCredential` support  ([#22328](https://github.com/Azure/azure-sdk-for-python/issues/22328))
```

## Comparing `azure-identity-1.9.0/README.md` & `azure-identity-1.9.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,20 @@
 When debugging and executing code locally it is typical for developers to use
 their own accounts for authenticating calls to Azure services. The Azure
 Identity library supports authenticating through developer tools to simplify
 local development.
 
 #### Authenticate via Visual Studio Code
 
-Developers using Visual Studio Code can use the [Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account) to authenticate via the editor. Apps using `DefaultAzureCredential` or `VisualStudioCodeCredential` can then use this account to authenticate calls in their app when running locally.
-
-To authenticate in Visual Studio Code, ensure **version 0.9.11 or earlier** of the Azure Account extension is installed. To track progress toward supporting newer extension versions, see [this GitHub issue](https://github.com/Azure/azure-sdk-for-net/issues/27263). Once installed, open the **Command Palette** and run the **Azure: Sign In** command.
+`DefaultAzureCredential` and `VisualStudioCodeCredential` can authenticate as
+the user signed in to Visual Studio Code's
+[Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account).
+After installing the extension, sign in to Azure in Visual Studio Code by
+pressing `F1` to open the command palette and running the `Azure: Sign In`
+command.
 
 #### Authenticate via the Azure CLI
 
 `DefaultAzureCredential` and `AzureCliCredential` can authenticate as the user
 signed in to the [Azure CLI][azure_cli]. To sign in to the Azure CLI, run
 `az login`. On a system with a default web browser, the Azure CLI will launch
 the browser to authenticate a user.
```

## Comparing `azure-identity-1.9.0/LICENSE` & `azure-identity-1.9.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/setup.py` & `azure-identity-1.9.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     long_description=README + "\n\n" + CHANGELOG,
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity",
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

## Comparing `azure-identity-1.9.0/migration_guide.md` & `azure-identity-1.9.0b1/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/PKG-INFO` & `azure-identity-1.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-identity
-Version: 1.9.0
+Version: 1.9.0b1
 Summary: Microsoft Azure Identity Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Azure Identity client library for Python
         
@@ -40,17 +40,20 @@
         When debugging and executing code locally it is typical for developers to use
         their own accounts for authenticating calls to Azure services. The Azure
         Identity library supports authenticating through developer tools to simplify
         local development.
         
         #### Authenticate via Visual Studio Code
         
-        Developers using Visual Studio Code can use the [Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account) to authenticate via the editor. Apps using `DefaultAzureCredential` or `VisualStudioCodeCredential` can then use this account to authenticate calls in their app when running locally.
-        
-        To authenticate in Visual Studio Code, ensure **version 0.9.11 or earlier** of the Azure Account extension is installed. To track progress toward supporting newer extension versions, see [this GitHub issue](https://github.com/Azure/azure-sdk-for-net/issues/27263). Once installed, open the **Command Palette** and run the **Azure: Sign In** command.
+        `DefaultAzureCredential` and `VisualStudioCodeCredential` can authenticate as
+        the user signed in to Visual Studio Code's
+        [Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account).
+        After installing the extension, sign in to Azure in Visual Studio Code by
+        pressing `F1` to open the command palette and running the `Azure: Sign In`
+        command.
         
         #### Authenticate via the Azure CLI
         
         `DefaultAzureCredential` and `AzureCliCredential` can authenticate as the user
         signed in to the [Azure CLI][azure_cli]. To sign in to the Azure CLI, run
         `az login`. On a system with a default web browser, the Azure CLI will launch
         the browser to authenticate a user.
@@ -406,34 +409,14 @@
         [vscode_cred_ref]: https://aka.ms/azsdk/python/identity/vscodecredential
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fidentity%2Fazure-identity%2FREADME.png)
         
         
         # Release History
         
-        ## 1.9.0 (2022-04-05)
-        
-        ### Features Added
-        
-        - Added PII logging if logging.DEBUG is enabled.    ([#23203](https://github.com/Azure/azure-sdk-for-python/issues/23203))
-        
-        ### Breaking Changes
-        
-        - `validate_authority` support is not available in 1.9.0.
-        
-        ### Bugs Fixed
-        
-        - Added check on `content` from msal response.    ([#23483](https://github.com/Azure/azure-sdk-for-python/issues/23483))
-        - Fixed the issue that async OBO credential does not refresh correctly.    ([#21981](https://github.com/Azure/azure-sdk-for-python/issues/21981))
-        
-        ### Other Changes
-        
-        - Removed `resource_id`, please use `identity_config` instead.
-        - Renamed argument name `get_assertion` to `func` for `ClientAssertionCredential`.
-        
         ## 1.9.0b1 (2022-03-08)
         
         ### Features Added
         
         - Added `validate_authority` support for msal client  ([#22625](https://github.com/Azure/azure-sdk-for-python/issues/22625))
         - Added `resource_id` support for user-assigned managed identity  ([#22329](https://github.com/Azure/azure-sdk-for-python/issues/22329))
         - Added `ClientAssertionCredential` support  ([#22328](https://github.com/Azure/azure-sdk-for-python/issues/22328))
@@ -1076,15 +1059,15 @@
         for more details. User authentication will be added in an upcoming preview
         release.
         
         This release supports only global Azure Active Directory tenants, i.e. those
         using the https://login.microsoftonline.com authentication endpoint.
         
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `azure-identity-1.9.0/samples/custom_credentials.py` & `azure-identity-1.9.0b1/samples/custom_credentials.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/samples/key_vault_cert.py` & `azure-identity-1.9.0b1/samples/key_vault_cert.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/samples/user_authentication.py` & `azure-identity-1.9.0b1/samples/user_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/samples/control_interactive_prompts.py` & `azure-identity-1.9.0b1/samples/control_interactive_prompts.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_imds_credential.py` & `azure-identity-1.9.0b1/tests/test_imds_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_username_password_credential.py` & `azure-identity-1.9.0b1/tests/test_username_password_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_auth_record.py` & `azure-identity-1.9.0b1/tests/test_auth_record.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_cli_credential_async.py` & `azure-identity-1.9.0b1/tests/test_cli_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_azure_application_async.py` & `azure-identity-1.9.0b1/tests/test_azure_application_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_client_secret_credential_async.py` & `azure-identity-1.9.0b1/tests/test_client_secret_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_managed_identity_async.py` & `azure-identity-1.9.0b1/tests/test_managed_identity_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,74 +376,14 @@
         credential = ManagedIdentityCredential(transport=transport, identity_config={param_name: param_value})
         token = await credential.get_token(scope)
         assert token.token == expected_token
         assert token.expires_on == expires_on
 
 
 @pytest.mark.asyncio
-async def test_app_service_2017_09_01():
-    """When the environment for 2019-08-01 is not configured, 2017-09-01 should be used."""
-
-    access_token = "****"
-    expires_on = 42
-    expected_token = AccessToken(access_token, expires_on)
-    url = "http://localhost:42/token"
-    secret = "expected-secret"
-    scope = "scope"
-
-    transport = async_validating_transport(
-        requests=[
-            Request(
-                url,
-                method="GET",
-                required_headers={"secret": secret, "User-Agent": USER_AGENT},
-                required_params={"api-version": "2017-09-01", "resource": scope},
-            )
-        ]
-        * 2,
-        responses=[
-            mock_response(
-                json_payload={
-                    "access_token": access_token,
-                    "expires_on": "01/01/1970 00:00:{} +00:00".format(expires_on),  # linux format
-                    "resource": scope,
-                    "token_type": "Bearer",
-                }
-            ),
-            mock_response(
-                json_payload={
-                    "access_token": access_token,
-                    "expires_on": "1/1/1970 12:00:{} AM +00:00".format(expires_on),  # windows format
-                    "resource": scope,
-                    "token_type": "Bearer",
-                }
-            ),
-        ],
-    )
-
-    with mock.patch.dict(
-        MANAGED_IDENTITY_ENVIRON,
-        {
-            EnvironmentVariables.MSI_ENDPOINT: url,
-            EnvironmentVariables.MSI_SECRET: secret,
-        },
-        clear=True,
-    ):
-        credential = ManagedIdentityCredential(transport=transport)
-        token = await credential.get_token(scope)
-        assert token == expected_token
-        assert token.expires_on == expires_on
-
-        credential = ManagedIdentityCredential(transport=transport)
-        token = await credential.get_token(scope)
-        assert token == expected_token
-        assert token.expires_on == expires_on
-
-
-@pytest.mark.asyncio
 async def test_app_service_2019_08_01():
     """App Service 2019-08-01: IDENTITY_ENDPOINT, IDENTITY_HEADER set"""
 
     access_token = "****"
     expires_on = 42
     endpoint = "http://localhost:42/token"
     new_endpoint = "http://localhost:42/new-token"
```

## Comparing `azure-identity-1.9.0/tests/test_cli_credential.py` & `azure-identity-1.9.0b1/tests/test_cli_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/recorded_test_case.py` & `azure-identity-1.9.0b1/tests/recorded_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_certificate_credential.py` & `azure-identity-1.9.0b1/tests/test_certificate_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_interactive_credential.py` & `azure-identity-1.9.0b1/tests/test_interactive_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/credscan_ignore.py` & `azure-identity-1.9.0b1/tests/credscan_ignore.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_obo_async.py` & `azure-identity-1.9.0b1/tests/test_obo_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_context_manager.py` & `azure-identity-1.9.0b1/tests/test_context_manager.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_live_async.py` & `azure-identity-1.9.0b1/tests/test_live_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_app_service.py` & `azure-identity-1.9.0b1/tests/test_app_service.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_cae.py` & `azure-identity-1.9.0b1/tests/test_cae.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/recording_processors.py` & `azure-identity-1.9.0b1/tests/recording_processors.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_obo.py` & `azure-identity-1.9.0b1/tests/test_obo.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/helpers_async.py` & `azure-identity-1.9.0b1/tests/helpers_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_application_credential_async.py` & `azure-identity-1.9.0b1/tests/test_application_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_get_token_mixin_async.py` & `azure-identity-1.9.0b1/tests/test_get_token_mixin_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_client_secret_credential.py` & `azure-identity-1.9.0b1/tests/test_client_secret_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_auth_code_async.py` & `azure-identity-1.9.0b1/tests/test_auth_code_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_chained_credential.py` & `azure-identity-1.9.0b1/tests/test_chained_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_auth_code.py` & `azure-identity-1.9.0b1/tests/test_auth_code.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_msal_client.py` & `azure-identity-1.9.0b1/tests/test_msal_client.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_chained_token_credential_async.py` & `azure-identity-1.9.0b1/tests/test_chained_token_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_browser_credential.py` & `azure-identity-1.9.0b1/tests/test_browser_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_default_async.py` & `azure-identity-1.9.0b1/tests/test_default_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_managed_identity_client_async.py` & `azure-identity-1.9.0b1/tests/test_managed_identity_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_shared_cache_credential_async.py` & `azure-identity-1.9.0b1/tests/test_shared_cache_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_managed_identity_client.py` & `azure-identity-1.9.0b1/tests/test_managed_identity_client.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_vscode_credential_async.py` & `azure-identity-1.9.0b1/tests/test_vscode_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_device_code_credential.py` & `azure-identity-1.9.0b1/tests/test_device_code_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_aad_client_async.py` & `azure-identity-1.9.0b1/tests/test_aad_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_live.py` & `azure-identity-1.9.0b1/tests/test_live.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_imds_credential_async.py` & `azure-identity-1.9.0b1/tests/test_imds_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_get_token_mixin.py` & `azure-identity-1.9.0b1/tests/test_get_token_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_azure_application.py` & `azure-identity-1.9.0b1/tests/test_azure_application.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_environment_credential_async.py` & `azure-identity-1.9.0b1/tests/test_environment_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_powershell_credential_async.py` & `azure-identity-1.9.0b1/tests/test_powershell_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_persistent_cache.py` & `azure-identity-1.9.0b1/tests/test_persistent_cache.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_app_service_async.py` & `azure-identity-1.9.0b1/tests/test_app_service_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_managed_identity.py` & `azure-identity-1.9.0b1/tests/test_managed_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,71 +374,14 @@
 
         credential = ManagedIdentityCredential(transport=transport, identity_config={param_name: param_value})
         token = credential.get_token(scope)
         assert token.token == expected_token
         assert token.expires_on == expires_on
 
 
-def test_app_service_2017_09_01():
-    """When the environment for 2019-08-01 is not configured, 2017-09-01 should be used."""
-
-    access_token = "****"
-    expires_on = 42
-    expected_token = AccessToken(access_token, expires_on)
-    url = "http://localhost:42/token"
-    secret = "expected-secret"
-    scope = "scope"
-
-    transport = validating_transport(
-        requests=[
-            Request(
-                url,
-                method="GET",
-                required_headers={"secret": secret, "User-Agent": USER_AGENT},
-                required_params={"api-version": "2017-09-01", "resource": scope},
-            )
-        ]
-        * 2,
-        responses=[
-            mock_response(
-                json_payload={
-                    "access_token": access_token,
-                    "expires_on": "01/01/1970 00:00:{} +00:00".format(expires_on),  # linux format
-                    "resource": scope,
-                    "token_type": "Bearer",
-                }
-            ),
-            mock_response(
-                json_payload={
-                    "access_token": access_token,
-                    "expires_on": "1/1/1970 12:00:{} AM +00:00".format(expires_on),  # windows format
-                    "resource": scope,
-                    "token_type": "Bearer",
-                }
-            ),
-        ],
-    )
-
-    with mock.patch.dict(
-        MANAGED_IDENTITY_ENVIRON,
-        {
-            EnvironmentVariables.MSI_ENDPOINT: url,
-            EnvironmentVariables.MSI_SECRET: secret,
-        },
-        clear=True,
-    ):
-        token = ManagedIdentityCredential(transport=transport).get_token(scope)
-        assert token == expected_token
-        assert token.expires_on == expires_on
-
-        token = ManagedIdentityCredential(transport=transport).get_token(scope)
-        assert token == expected_token
-        assert token.expires_on == expires_on
-
-
 def test_prefers_app_service_2019_08_01():
     """When the environment is configured for both App Service versions, the credential should prefer the most recent"""
 
     access_token = "****"
     expires_on = 42
     endpoint = "http://localhost:42/token"
     secret = "expected-secret"
```

## Comparing `azure-identity-1.9.0/tests/test_default.py` & `azure-identity-1.9.0b1/tests/test_default.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_powershell_credential.py` & `azure-identity-1.9.0b1/tests/test_powershell_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/helpers.py` & `azure-identity-1.9.0b1/tests/helpers.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_authority.py` & `azure-identity-1.9.0b1/tests/test_authority.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_vscode_credential.py` & `azure-identity-1.9.0b1/tests/test_vscode_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_application_credential.py` & `azure-identity-1.9.0b1/tests/test_application_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_aad_client.py` & `azure-identity-1.9.0b1/tests/test_aad_client.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_environment_credential.py` & `azure-identity-1.9.0b1/tests/test_environment_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_certificate_credential_async.py` & `azure-identity-1.9.0b1/tests/test_certificate_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/test_shared_cache_credential.py` & `azure-identity-1.9.0b1/tests/test_shared_cache_credential.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/pod-identity/run-test.py` & `azure-identity-1.9.0b1/tests/pod-identity/run-test.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell.py` & `azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live_async.py` & `azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/managed-identity-live/test_managed_identity_live.py` & `azure-identity-1.9.0b1/tests/managed-identity-live/test_managed_identity_live.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/managed-identity-live/conftest.py` & `azure-identity-1.9.0b1/tests/managed-identity-live/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/managed-identity-live/test_cloud_shell_async.py` & `azure-identity-1.9.0b1/tests/managed-identity-live/test_cloud_shell_async.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/perfstress_tests/memory_cache_read.py` & `azure-identity-1.9.0b1/tests/perfstress_tests/memory_cache_read.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/perfstress_tests/persistent_cache_read.py` & `azure-identity-1.9.0b1/tests/perfstress_tests/persistent_cache_read.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/perfstress_tests/bearer_token_auth_policy.py` & `azure-identity-1.9.0b1/tests/perfstress_tests/bearer_token_auth_policy.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/azure-functions/RunTest/__init__.py` & `azure-identity-1.9.0b1/tests/azure-functions/RunTest/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/tests/azure-functions/RunAsyncTest/__init__.py` & `azure-identity-1.9.0b1/tests/azure-functions/RunAsyncTest/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/__init__.py` & `azure-identity-1.9.0b1/azure/identity/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_constants.py` & `azure-identity-1.9.0b1/azure/identity/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_auth_record.py` & `azure-identity-1.9.0b1/azure/identity/_auth_record.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_persistent_cache.py` & `azure-identity-1.9.0b1/azure/identity/_persistent_cache.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_exceptions.py` & `azure-identity-1.9.0b1/azure/identity/_exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_enums.py` & `azure-identity-1.9.0b1/azure/identity/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/__init__.py` & `azure-identity-1.9.0b1/azure/identity/aio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     ClientSecretCredential,
     DefaultAzureCredential,
     EnvironmentCredential,
     ManagedIdentityCredential,
     OnBehalfOfCredential,
     SharedTokenCacheCredential,
     VisualStudioCodeCredential,
-    ClientAssertionCredential,
 )
 
 
 __all__ = [
     "AuthorizationCodeCredential",
     "AzureCliCredential",
     "AzurePowerShellCredential",
@@ -30,9 +29,8 @@
     "DefaultAzureCredential",
     "EnvironmentCredential",
     "ManagedIdentityCredential",
     "OnBehalfOfCredential",
     "ChainedTokenCredential",
     "SharedTokenCacheCredential",
     "VisualStudioCodeCredential",
-    "ClientAssertionCredential",
 ]
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/__init__.py` & `azure-identity-1.9.0b1/azure/identity/aio/_internal/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/aad_client.py` & `azure-identity-1.9.0b1/azure/identity/aio/_internal/aad_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,28 +67,14 @@
 
     async def obtain_token_by_refresh_token(
         self, scopes: "Iterable[str]", refresh_token: str, **kwargs: "Any"
     ) -> "AccessToken":
         request = self._get_refresh_token_request(scopes, refresh_token, **kwargs)
         return await self._run_pipeline(request, **kwargs)
 
-    async def obtain_token_by_refresh_token_on_behalf_of(
-        self,
-        scopes: "Iterable[str]",
-        client_credential: "Union[str, AadClientCertificate]",
-        refresh_token: str,
-        **kwargs: "Any"
-    ) -> "AccessToken":
-        request = self._get_refresh_token_on_behalf_of_request(
-            scopes,
-            client_credential=client_credential,
-            refresh_token=refresh_token,
-            **kwargs)
-        return await self._run_pipeline(request, **kwargs)
-
     async def obtain_token_on_behalf_of(
         self,
         scopes: "Iterable[str]",
         client_credential: "Union[str, AadClientCertificate]",
         user_assertion: str,
         **kwargs: "Any"
     ) -> "AccessToken":
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/decorators.py` & `azure-identity-1.9.0b1/azure/identity/_internal/win_vscode_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
-import functools
-import logging
+import os
 import json
-import base64
-
-from azure.core.exceptions import ClientAuthenticationError
+import logging
+import ctypes as ct
+from .._constants import VSCODE_CREDENTIALS_SECTION
 
-from ..._internal import within_credential_chain
+try:
+    import ctypes.wintypes as wt
+except (IOError, ValueError):
+    pass
 
 _LOGGER = logging.getLogger(__name__)
 
+SUPPORTED_CREDKEYS = set(("Type", "TargetName", "Persist", "UserName", "Comment", "CredentialBlob"))
+
+_PBYTE = ct.POINTER(ct.c_byte)
 
-def log_get_token_async(fn):
-    @functools.wraps(fn)
-    async def wrapper(*args, **kwargs):
-        try:
-            token = await fn(*args, **kwargs)
-            _LOGGER.log(
-                logging.DEBUG if within_credential_chain.get() else logging.INFO, "%s succeeded", fn.__qualname__
-            )
-            if _LOGGER.isEnabledFor(logging.DEBUG):
-                try:
-                    base64_meta_data = token.token.split(".")[1].encode("utf-8") + b'=='
-                    json_bytes = base64.decodebytes(base64_meta_data)
-                    json_string = json_bytes.decode('utf-8')
-                    json_dict = json.loads(json_string)
-                    upn = json_dict.get('upn', 'unavailableUpn')
-                    log_string = '[Authenticated account] Client ID: {}. Tenant ID: {}. User Principal Name: {}. ' \
-                                 'Object ID (user): {}'.format(json_dict['appid'],
-                                                               json_dict['tid'],
-                                                               upn,
-                                                               json_dict['oid']
-                                                               )
-                    _LOGGER.debug(log_string)
-                except Exception:  # pylint: disable=broad-except
-                    _LOGGER.debug("Fail to log the account information")
-            return token
-        except Exception as ex: # pylint: disable=broad-except
-            _LOGGER.log(
-                logging.DEBUG if within_credential_chain.get() else logging.WARNING,
-                "%s failed: %s",
-                fn.__qualname__,
-                ex,
-                exc_info=_LOGGER.isEnabledFor(logging.DEBUG),
-            )
-            raise
-
-    return wrapper
-
-
-def wrap_exceptions(fn):
-    """Prevents leaking exceptions defined outside azure-core by raising ClientAuthenticationError from them."""
-
-    @functools.wraps(fn)
-    async def wrapper(*args, **kwargs):
-        try:
-            result = await fn(*args, **kwargs)
-            return result
-        except ClientAuthenticationError:
-            raise
-        except Exception as ex:  # pylint:disable=broad-except
-            auth_error = ClientAuthenticationError(message="Authentication failed: {}".format(ex))
-            raise auth_error from ex
 
-    return wrapper
+class _CREDENTIAL(ct.Structure):
+    _fields_ = [
+        ("Flags", wt.DWORD),
+        ("Type", wt.DWORD),
+        ("TargetName", ct.c_wchar_p),
+        ("Comment", ct.c_wchar_p),
+        ("LastWritten", wt.FILETIME),
+        ("CredentialBlobSize", wt.DWORD),
+        ("CredentialBlob", _PBYTE),
+        ("Persist", wt.DWORD),
+        ("AttributeCount", wt.DWORD),
+        ("Attributes", ct.c_void_p),
+        ("TargetAlias", ct.c_wchar_p),
+        ("UserName", ct.c_wchar_p),
+    ]
+
+
+_PCREDENTIAL = ct.POINTER(_CREDENTIAL)
+
+_advapi = ct.WinDLL("advapi32")  # type: ignore
+_advapi.CredReadW.argtypes = [wt.LPCWSTR, wt.DWORD, wt.DWORD, ct.POINTER(_PCREDENTIAL)]
+_advapi.CredReadW.restype = wt.BOOL
+_advapi.CredFree.argtypes = [_PCREDENTIAL]
+
+
+def _read_credential(service_name, account_name):
+    target = "{}/{}".format(service_name, account_name)
+    cred_ptr = _PCREDENTIAL()
+    if _advapi.CredReadW(target, 1, 0, ct.byref(cred_ptr)):
+        cred_blob = cred_ptr.contents.CredentialBlob
+        cred_blob_size = cred_ptr.contents.CredentialBlobSize
+        cred = "".join(map(chr, cred_blob[:cred_blob_size]))
+        _advapi.CredFree(cred_ptr)
+        return cred
+    return None
+
+
+def get_user_settings():
+    try:
+        path = os.path.join(os.environ["APPDATA"], "Code", "User", "settings.json")
+        with open(path) as file:
+            return json.load(file)
+    except Exception as ex:  # pylint:disable=broad-except
+        _LOGGER.debug('Exception reading VS Code user settings: "%s"', ex, exc_info=_LOGGER.isEnabledFor(logging.DEBUG))
+        return {}
+
+
+def get_refresh_token(cloud_name):
+    try:
+        return _read_credential(VSCODE_CREDENTIALS_SECTION, cloud_name)
+    except Exception as ex:  # pylint: disable=broad-except
+        _LOGGER.debug(
+            'Exception retrieving VS Code credentials: "%s"', ex, exc_info=_LOGGER.isEnabledFor(logging.DEBUG)
+        )
+        return None
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/get_token_mixin.py` & `azure-identity-1.9.0b1/azure/identity/aio/_internal/get_token_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_base.py` & `azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_base.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_internal/managed_identity_client.py` & `azure-identity-1.9.0b1/azure/identity/aio/_internal/managed_identity_client.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/chained.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/chained.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/certificate.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/certificate.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/azure_cli.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_cli.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/__init__.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .managed_identity import ManagedIdentityCredential
 from .on_behalf_of import OnBehalfOfCredential
 from .certificate import CertificateCredential
 from .client_secret import ClientSecretCredential
 from .shared_cache import SharedTokenCacheCredential
 from .azure_cli import AzureCliCredential
 from .vscode import VisualStudioCodeCredential
-from .client_assertion import ClientAssertionCredential
 
 
 __all__ = [
     "AuthorizationCodeCredential",
     "AzureCliCredential",
     "AzurePowerShellCredential",
     "CertificateCredential",
@@ -26,9 +25,8 @@
     "ClientSecretCredential",
     "DefaultAzureCredential",
     "EnvironmentCredential",
     "ManagedIdentityCredential",
     "OnBehalfOfCredential",
     "SharedTokenCacheCredential",
     "VisualStudioCodeCredential",
-    "ClientAssertionCredential",
 ]
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/azure_powershell.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_powershell.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/managed_identity.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/managed_identity.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/imds.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/imds.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/app_service.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/app_service.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/client_secret.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_secret.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/shared_cache.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/shared_cache.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/environment.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,20 @@
     This credential is capable of authenticating as a service principal using a client secret or a certificate, or as
     a user with a username and password. Configuration is attempted in this order, using these environment variables:
 
     Service principal with secret:
       - **AZURE_TENANT_ID**: ID of the service principal's tenant. Also called its 'directory' ID.
       - **AZURE_CLIENT_ID**: the service principal's client ID
       - **AZURE_CLIENT_SECRET**: one of the service principal's client secrets
-      - **AZURE_AUTHORITY_HOST**: authority of an Azure Active Directory endpoint, for example
-        "login.microsoftonline.com", the authority for Azure Public Cloud, which is the default
-        when no value is given.
 
     Service principal with certificate:
       - **AZURE_TENANT_ID**: ID of the service principal's tenant. Also called its 'directory' ID.
       - **AZURE_CLIENT_ID**: the service principal's client ID
       - **AZURE_CLIENT_CERTIFICATE_PATH**: path to a PEM or PKCS12 certificate file including the private key. The
         certificate must not be password-protected.
-      - **AZURE_AUTHORITY_HOST**: authority of an Azure Active Directory endpoint, for example
-        "login.microsoftonline.com", the authority for Azure Public Cloud, which is the default
-        when no value is given.
     """
 
     def __init__(self, **kwargs: "Any") -> None:
         self._credential = None  # type: Optional[Union[CertificateCredential, ClientSecretCredential]]
 
         if all(os.environ.get(v) is not None for v in EnvironmentVariables.CLIENT_SECRET_VARS):
             self._credential = ClientSecretCredential(
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/client_assertion.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/client_assertion.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Optional
     from azure.core.credentials import AccessToken
 
 
 class ClientAssertionCredential(AsyncContextManager, GetTokenMixin):
-    def __init__(self, tenant_id: str, client_id: str, func: "Callable[[], str]", **kwargs: "Any") -> None:
+    def __init__(self, tenant_id: str, client_id: str, get_assertion: "Callable[[], str]", **kwargs: "Any") -> None:
         """Authenticates a service principal with a JWT assertion.
 
         This credential is for advanced scenarios. :class:`~azure.identity.ClientCertificateCredential` has a more
         convenient API for the most common assertion scenario, authenticating a service principal with a certificate.
 
         :param str tenant_id: ID of the principal's tenant. Also called its "directory" ID.
         :param str client_id: the principal's client ID
-        :param func: a callable that returns a string assertion. The credential will call this every time it
+        :param get_assertion: a callable that returns a string assertion. The credential will call this every time it
             acquires a new token.
-        :paramtype func: Callable[[], str]
+        :paramtype get_assertion: Callable[[], str]
 
         :keyword str authority: authority of an Azure Active Directory endpoint, for example
             "login.microsoftonline.com", the authority for Azure Public Cloud (which is the default).
             :class:`~azure.identity.AzureAuthorityHosts` defines authorities for other clouds.
         """
-        self._func = func
+        self._get_assertion = get_assertion
         self._client = AadClient(tenant_id, client_id, **kwargs)
         super().__init__(**kwargs)
 
     async def __aenter__(self):
         await self._client.__aenter__()
         return self
 
@@ -41,10 +41,10 @@
         """Close the credential's transport session."""
         await self._client.close()
 
     async def _acquire_token_silently(self, *scopes: str, **kwargs: "Any") -> "Optional[AccessToken]":
         return self._client.get_cached_access_token(scopes, **kwargs)
 
     async def _request_token(self, *scopes: str, **kwargs: "Any") -> "AccessToken":
-        assertion = self._func()
+        assertion = self._get_assertion()
         token = await self._client.obtain_token_by_jwt_assertion(scopes, assertion, **kwargs)
         return token
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/vscode.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/vscode.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # ------------------------------------
 from typing import cast, TYPE_CHECKING
 
 from ..._exceptions import CredentialUnavailableError
 from .._internal import AsyncContextManager
 from .._internal.aad_client import AadClient
 from .._internal.get_token_mixin import GetTokenMixin
-from .._internal.decorators import log_get_token_async
 from ..._credentials.vscode import _VSCodeCredentialBase
 
 if TYPE_CHECKING:
     # pylint:disable=unused-import,ungrouped-imports
     from typing import Any, Optional
     from azure.core.credentials import AccessToken
 
@@ -36,34 +35,29 @@
 
     async def close(self) -> None:
         """Close the credential's transport session."""
 
         if self._client:
             await self._client.__aexit__()
 
-    @log_get_token_async
     async def get_token(self, *scopes: str, **kwargs: "Any") -> "AccessToken":
         """Request an access token for `scopes` as the user currently signed in to Visual Studio Code.
 
         This method is called automatically by Azure SDK clients.
 
         :param str scopes: desired scopes for the access token. This method requires at least one scope.
         :keyword str tenant_id: optional tenant to include in the token request.
 
         :rtype: :class:`azure.core.credentials.AccessToken`
 
         :raises ~azure.identity.CredentialUnavailableError: the credential cannot retrieve user details from Visual
             Studio Code
         """
         if self._unavailable_reason:
-            error_message = self._unavailable_reason \
-                            + '\n' \
-                              "Visit https://aka.ms/azsdk/python/identity/vscodecredential/troubleshoot" \
-                              " to troubleshoot this issue."
-            raise CredentialUnavailableError(message=error_message)
+            raise CredentialUnavailableError(message=self._unavailable_reason)
         if not self._client:
             raise CredentialUnavailableError("Initialization failed")
 
         return await super().get_token(*scopes, **kwargs)
 
     async def _acquire_token_silently(self, *scopes: str, **kwargs: "Any") -> "Optional[AccessToken]":
         self._client = cast(AadClient, self._client)
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/application.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/application.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/token_exchange.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/token_exchange.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 
 class TokenExchangeCredential(ClientAssertionCredential, TokenFileMixin):
     def __init__(self, tenant_id: str, client_id: str, token_file_path: str, **kwargs: "Any") -> None:
         super().__init__(
             tenant_id=tenant_id,
             client_id=client_id,
-            func=self.get_service_account_token,
+            get_assertion=self.get_service_account_token,
             token_file_path=token_file_path,
             **kwargs
         )
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/on_behalf_of.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/on_behalf_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,15 @@
         # Note we assume the cache has tokens for one user only. That's okay because each instance of this class is
         # locked to a single user (assertion). This assumption will become unsafe if this class allows applications
         # to change an instance's assertion.
         refresh_tokens = self._client.get_cached_refresh_tokens(scopes)
         if len(refresh_tokens) == 1:  # there should be only one
             try:
                 refresh_token = refresh_tokens[0]["secret"]
-                return await self._client.obtain_token_by_refresh_token_on_behalf_of(
-                    scopes, self._client_credential, refresh_token, **kwargs)
+                return await self._client.obtain_token_by_refresh_token(scopes, refresh_token, **kwargs)
             except ClientAuthenticationError as ex:
                 _LOGGER.debug("silent authentication failed: %s", ex, exc_info=True)
             except (IndexError, KeyError, TypeError) as ex:
                 # this is purely defensive, hasn't been observed in practice
                 _LOGGER.debug("silent authentication failed due to malformed refresh token: %s", ex, exc_info=True)
 
         # we don't have a refresh token, or silent auth failed: acquire a new token from the assertion
```

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/authorization_code.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/authorization_code.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/azure_arc.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_arc.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/azure_ml.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/azure_ml.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/cloud_shell.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/cloud_shell.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/service_fabric.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/service_fabric.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/aio/_credentials/default.py` & `azure-identity-1.9.0b1/azure/identity/aio/_credentials/default.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/pipeline.py` & `azure-identity-1.9.0b1/azure/identity/_internal/pipeline.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/linux_vscode_adapter.py` & `azure-identity-1.9.0b1/azure/identity/_internal/linux_vscode_adapter.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/__init__.py` & `azure-identity-1.9.0b1/azure/identity/_internal/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/interactive.py` & `azure-identity-1.9.0b1/azure/identity/_internal/interactive.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/aad_client.py` & `azure-identity-1.9.0b1/azure/identity/_internal/aad_client.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/auth_code_redirect_handler.py` & `azure-identity-1.9.0b1/azure/identity/_internal/auth_code_redirect_handler.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/decorators.py` & `azure-identity-1.9.0b1/azure/identity/_internal/decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import functools
 import logging
-import json
-import base64
 
 from six import raise_from
 from azure.core.exceptions import ClientAuthenticationError
 
 from . import within_credential_chain
 
 
@@ -29,32 +27,16 @@
         @functools.wraps(fn)
         def wrapper(*args, **kwargs):
             try:
                 token = fn(*args, **kwargs)
                 _LOGGER.log(
                     logging.DEBUG if within_credential_chain.get() else logging.INFO, "%s succeeded", qualified_name
                 )
-                if _LOGGER.isEnabledFor(logging.DEBUG):
-                    try:
-                        base64_meta_data = token.token.split(".")[1].encode("utf-8") + b'=='
-                        json_bytes = base64.decodebytes(base64_meta_data)
-                        json_string = json_bytes.decode('utf-8')
-                        json_dict = json.loads(json_string)
-                        upn = json_dict.get('upn', 'unavailableUpn')
-                        log_string = '[Authenticated account] Client ID: {}. Tenant ID: {}. User Principal Name: {}. ' \
-                                     'Object ID (user): {}'.format(json_dict['appid'],
-                                                                   json_dict['tid'],
-                                                                   upn,
-                                                                   json_dict['oid']
-                                                                   )
-                        _LOGGER.debug(log_string)
-                    except Exception:     # pylint: disable=broad-except
-                        _LOGGER.debug("Fail to log the account information")
                 return token
-            except Exception as ex:   # pylint: disable=broad-except
+            except Exception as ex:
                 _LOGGER.log(
                     logging.DEBUG if within_credential_chain.get() else logging.WARNING,
                     "%s failed: %s",
                     qualified_name,
                     ex,
                     exc_info=_LOGGER.isEnabledFor(logging.DEBUG),
                 )
```

## Comparing `azure-identity-1.9.0/azure/identity/_internal/get_token_mixin.py` & `azure-identity-1.9.0b1/azure/identity/_internal/get_token_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/msal_client.py` & `azure-identity-1.9.0b1/azure/identity/_internal/msal_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,15 @@
 
     def raise_for_status(self):
         if self.status_code < 400:
             return
 
         if ContentDecodePolicy.CONTEXT_NAME in self._response.context:
             content = self._response.context[ContentDecodePolicy.CONTEXT_NAME]
-            if not content:
-                message = "Unexpected response from Azure Active Directory"
-            elif "error" in content or "error_description" in content:
+            if "error" in content or "error_description" in content:
                 message = "Authentication failed: {}".format(content.get("error_description") or content.get("error"))
             else:
                 for secret in ("access_token", "refresh_token"):
                     if secret in content:
                         content[secret] = "***"
                 message = 'Unexpected response from Azure Active Directory: "{}"'.format(content)
         else:
```

## Comparing `azure-identity-1.9.0/azure/identity/_internal/aad_client_base.py` & `azure-identity-1.9.0b1/azure/identity/_internal/aad_client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,31 +253,14 @@
             "scope": " ".join(scopes),
             "client_id": self._client_id,
             "client_info": 1,  # request AAD include home_account_id in its response
         }
         request = self._post(data, **kwargs)
         return request
 
-    def _get_refresh_token_on_behalf_of_request(self, scopes, client_credential, refresh_token, **kwargs):
-        # type: (Iterable[str], Union[str, AadClientCertificate], str, **Any) -> HttpRequest
-        data = {
-            "grant_type": "refresh_token",
-            "refresh_token": refresh_token,
-            "scope": " ".join(scopes),
-            "client_id": self._client_id,
-            "client_info": 1,  # request AAD include home_account_id in its response
-        }
-        if isinstance(client_credential, AadClientCertificate):
-            data["client_assertion"] = self._get_client_certificate_assertion(client_credential)
-            data["client_assertion_type"] = JWT_BEARER_ASSERTION
-        else:
-            data["client_secret"] = client_credential
-        request = self._post(data, **kwargs)
-        return request
-
     def _get_token_url(self, **kwargs):
         # type: (**Any) -> str
         tenant = resolve_tenant(self._tenant_id, **kwargs)
         return "/".join((self._authority, tenant, "oauth2/v2.0/token"))
 
     def _post(self, data, **kwargs):
         # type: (dict, **Any) -> HttpRequest
```

## Comparing `azure-identity-1.9.0/azure/identity/_internal/macos_vscode_adapter.py` & `azure-identity-1.9.0b1/azure/identity/_internal/macos_vscode_adapter.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/client_credential_base.py` & `azure-identity-1.9.0b1/azure/identity/_internal/client_credential_base.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/managed_identity_base.py` & `azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_base.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/msal_credentials.py` & `azure-identity-1.9.0b1/azure/identity/_internal/msal_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class MsalCredential(object):
     """Base class for credentials wrapping MSAL applications"""
 
     def __init__(self, client_id, client_credential=None, **kwargs):
         # type: (str, Optional[Union[str, Dict]], **Any) -> None
         authority = kwargs.pop("authority", None)
-        # self._validate_authority = kwargs.pop("validate_authority", True)
+        self._validate_authority = kwargs.pop("validate_authority", True)
         self._authority = normalize_authority(authority) if authority else get_default_authority()
         self._regional_authority = os.environ.get(EnvironmentVariables.AZURE_REGIONAL_AUTHORITY_NAME)
         self._tenant_id = kwargs.pop("tenant_id", None) or "organizations"
         validate_tenant_id(self._tenant_id)
         self._client = MsalClient(**kwargs)
         self._client_applications = {}  # type: Dict[str, msal.ClientApplication]
         self._client_credential = client_credential
@@ -69,11 +69,11 @@
                 client_id=self._client_id,
                 client_credential=self._client_credential,
                 client_capabilities=capabilities,
                 authority="{}/{}".format(self._authority, tenant_id),
                 azure_region=self._regional_authority,
                 token_cache=self._cache,
                 http_client=self._client,
-                # validate_authority=self._validate_authority
+                validate_authority=self._validate_authority
             )
 
         return self._client_applications[tenant_id]
```

## Comparing `azure-identity-1.9.0/azure/identity/_internal/managed_identity_client.py` & `azure-identity-1.9.0b1/azure/identity/_internal/managed_identity_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,23 @@
     from azure.core.pipeline.transport import HttpRequest
 
     PolicyType = Union[HTTPPolicy, SansIOHTTPPolicy]
 
 
 class ManagedIdentityClientBase(ABC):
     # pylint:disable=missing-client-constructor-parameter-credential
-    def __init__(self, request_factory, client_id=None, identity_config=None, **kwargs):
-        # type: (Callable[[str, dict], HttpRequest], Optional[str], Optional[Dict], **Any) -> None
+    def __init__(self, request_factory, client_id=None, resource_id=None, identity_config=None, **kwargs):
+        # type: (Callable[[str, dict], HttpRequest], Optional[str], Optional[str], Optional[Dict], **Any) -> None
         self._cache = kwargs.pop("_cache", None) or TokenCache()
         self._content_callback = kwargs.pop("_content_callback", None)
         self._identity_config = identity_config or {}
         if client_id:
             self._identity_config["client_id"] = client_id
+        if resource_id:
+            self._identity_config["mi_res_id"] = resource_id
         self._pipeline = self._build_pipeline(**kwargs)
         self._request_factory = request_factory
 
     def _process_response(self, response, request_time):
         # type: (PipelineResponse, int) -> AccessToken
 
         content = response.context.get(ContentDecodePolicy.CONTEXT_NAME)
```

## Comparing `azure-identity-1.9.0/azure/identity/_internal/shared_token_cache.py` & `azure-identity-1.9.0b1/azure/identity/_internal/shared_token_cache.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_internal/aadclient_certificate.py` & `azure-identity-1.9.0b1/azure/identity/_internal/aadclient_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/device_code.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/device_code.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/chained.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/chained.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/certificate.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/certificate.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/azure_cli.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/azure_cli.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/__init__.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/silent.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/silent.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/azure_powershell.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/azure_powershell.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/user_password.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/user_password.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/managed_identity.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/managed_identity.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     This credential defaults to using a system-assigned identity. To configure a user-assigned identity, use one of
     the keyword arguments. See `Azure Active Directory documentation
     <https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview>`_ for more
     information about configuring managed identity for applications.
 
     :keyword str client_id: a user-assigned identity's client ID or, when using Pod Identity, the client ID of an Azure
         AD app registration. This argument is supported in all hosting environments.
+    :keyword str resource_id: The resource ID to authenticate for a user-assigned managed identity.
+        See `Managed identity types
+        <https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview#managed-identity-types>`_
+        for more information about user-assigned managed identities.
     :keyword identity_config: a mapping ``{parameter_name: value}`` specifying a user-assigned identity by its object
         or resource ID, for example ``{"object_id": "..."}``. Check the documentation for your hosting environment to
         learn what values it expects.
     :paramtype identity_config: Mapping[str, str]
     """
 
     def __init__(self, **kwargs):
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/imds.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/imds.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         self._client = ManagedIdentityClient(get_request, **dict(PIPELINE_SETTINGS, **kwargs))
         if EnvironmentVariables.AZURE_POD_IDENTITY_AUTHORITY_HOST in os.environ:
             self._endpoint_available = True  # type: Optional[bool]
         else:
             self._endpoint_available = None
         self._error_message = None  # type: Optional[str]
-        self._user_assigned_identity = "client_id" in kwargs or "identity_config" in kwargs
+        self._user_assigned_identity = "client_id" in kwargs or "resource_id" in kwargs or "identity_config" in kwargs
 
     def __enter__(self):
         self._client.__enter__()
         return self
 
     def __exit__(self, *args):
         self._client.__exit__(*args)
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/app_service.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/app_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
     url = os.environ.get(EnvironmentVariables.IDENTITY_ENDPOINT)
     secret = os.environ.get(EnvironmentVariables.IDENTITY_HEADER)
     if not (url and secret):
         # App Service managed identity isn't available in this environment
         return None
 
+    if kwargs.get("resource_id"):
+        identity_config["mi_res_id"] = kwargs.pop("resource_id")
+
     return dict(
         kwargs,
         identity_config=identity_config,
         base_headers={"X-IDENTITY-HEADER": secret},
         request_factory=functools.partial(_get_request, url),
     )
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/client_secret.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/client_secret.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/shared_cache.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/shared_cache.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/environment.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,37 +34,28 @@
     This credential is capable of authenticating as a service principal using a client secret or a certificate, or as
     a user with a username and password. Configuration is attempted in this order, using these environment variables:
 
     Service principal with secret:
       - **AZURE_TENANT_ID**: ID of the service principal's tenant. Also called its 'directory' ID.
       - **AZURE_CLIENT_ID**: the service principal's client ID
       - **AZURE_CLIENT_SECRET**: one of the service principal's client secrets
-      - **AZURE_AUTHORITY_HOST**: authority of an Azure Active Directory endpoint, for example
-        "login.microsoftonline.com", the authority for Azure Public Cloud, which is the default
-        when no value is given.
 
     Service principal with certificate:
       - **AZURE_TENANT_ID**: ID of the service principal's tenant. Also called its 'directory' ID.
       - **AZURE_CLIENT_ID**: the service principal's client ID
       - **AZURE_CLIENT_CERTIFICATE_PATH**: path to a PEM or PKCS12 certificate file including the private key. The
         certificate must not be password-protected.
-      - **AZURE_AUTHORITY_HOST**: authority of an Azure Active Directory endpoint, for example
-        "login.microsoftonline.com", the authority for Azure Public Cloud, which is the default
-        when no value is given.
 
     User with username and password:
       - **AZURE_CLIENT_ID**: the application's client ID
       - **AZURE_USERNAME**: a username (usually an email address)
       - **AZURE_PASSWORD**: that user's password
       - **AZURE_TENANT_ID**: (optional) ID of the service principal's tenant. Also called its 'directory' ID.
         If not provided, defaults to the 'organizations' tenant, which supports only Azure Active Directory work or
         school accounts.
-      - **AZURE_AUTHORITY_HOST**: authority of an Azure Active Directory endpoint, for example
-        "login.microsoftonline.com", the authority for Azure Public Cloud, which is the default
-        when no value is given.
     """
 
     def __init__(self, **kwargs):
         # type: (Mapping[str, Any]) -> None
         self._credential = None  # type: Optional[EnvironmentCredentialTypes]
 
         if all(os.environ.get(v) is not None for v in EnvironmentVariables.CLIENT_SECRET_VARS):
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/client_assertion.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/client_assertion.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Optional
     from azure.core.credentials import AccessToken
 
 
 class ClientAssertionCredential(GetTokenMixin):
-    def __init__(self, tenant_id, client_id, func, **kwargs):
+    def __init__(self, tenant_id, client_id, get_assertion, **kwargs):
         # type: (str, str, Callable[[], str], **Any) -> None
         """Authenticates a service principal with a JWT assertion.
 
         This credential is for advanced scenarios. :class:`~azure.identity.ClientCertificateCredential` has a more
         convenient API for the most common assertion scenario, authenticating a service principal with a certificate.
 
         :param str tenant_id: ID of the principal's tenant. Also called its "directory" ID.
         :param str client_id: the principal's client ID
-        :param func: a callable that returns a string assertion. The credential will call this every time it
+        :param get_assertion: a callable that returns a string assertion. The credential will call this every time it
             acquires a new token.
-        :paramtype func: Callable[[], str]
+        :paramtype get_assertion: Callable[[], str]
 
         :keyword str authority: authority of an Azure Active Directory endpoint, for example
             "login.microsoftonline.com", the authority for Azure Public Cloud (which is the default).
             :class:`~azure.identity.AzureAuthorityHosts` defines authorities for other clouds.
         """
-        self._func = func
+        self._get_assertion = get_assertion
         self._client = AadClient(tenant_id, client_id, **kwargs)
         super(ClientAssertionCredential, self).__init__(**kwargs)
 
     def __enter__(self):
         self._client.__enter__()
         return self
 
@@ -47,10 +47,10 @@
 
     def _acquire_token_silently(self, *scopes, **kwargs):
         # type: (*str, **Any) -> Optional[AccessToken]
         return self._client.get_cached_access_token(scopes, **kwargs)
 
     def _request_token(self, *scopes, **kwargs):
         # type: (*str, **Any) -> AccessToken
-        assertion = self._func()
+        assertion = self._get_assertion()
         token = self._client.obtain_token_by_jwt_assertion(scopes, assertion, **kwargs)
         return token
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/vscode.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/vscode.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import cast, TYPE_CHECKING
 
 from .._exceptions import CredentialUnavailableError
 from .._constants import AzureAuthorityHosts, AZURE_VSCODE_CLIENT_ID, EnvironmentVariables
 from .._internal import normalize_authority, validate_tenant_id
 from .._internal.aad_client import AadClient
 from .._internal.get_token_mixin import GetTokenMixin
-from .._internal.decorators import log_get_token
 
 if sys.platform.startswith("win"):
     from .._internal.win_vscode_adapter import get_refresh_token, get_user_settings
 elif sys.platform.startswith("darwin"):
     from .._internal.macos_vscode_adapter import get_refresh_token, get_user_settings
 else:
     from .._internal.linux_vscode_adapter import get_refresh_token, get_user_settings
@@ -133,32 +132,27 @@
             self._client.__exit__(*args)
 
     def close(self):
         # type: () -> None
         """Close the credential's transport session."""
         self.__exit__()
 
-    @log_get_token("VSCodeCredential")
     def get_token(self, *scopes, **kwargs):
         # type: (*str, **Any) -> AccessToken
         """Request an access token for `scopes` as the user currently signed in to Visual Studio Code.
 
         This method is called automatically by Azure SDK clients.
 
         :param str scopes: desired scopes for the access token. This method requires at least one scope.
         :rtype: :class:`azure.core.credentials.AccessToken`
         :raises ~azure.identity.CredentialUnavailableError: the credential cannot retrieve user details from Visual
           Studio Code
         """
         if self._unavailable_reason:
-            error_message = self._unavailable_reason \
-                            + '\n' \
-                              "Visit https://aka.ms/azsdk/python/identity/vscodecredential/troubleshoot" \
-                              " to troubleshoot this issue."
-            raise CredentialUnavailableError(message=error_message)
+            raise CredentialUnavailableError(message=self._unavailable_reason)
         return super(VisualStudioCodeCredential, self).get_token(*scopes, **kwargs)
 
     def _acquire_token_silently(self, *scopes, **kwargs):
         # type: (*str, **Any) -> Optional[AccessToken]
         self._client = cast(AadClient, self._client)
         return self._client.get_cached_access_token(scopes, **kwargs)
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/application.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/application.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/token_exchange.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/token_exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 
 class TokenExchangeCredential(ClientAssertionCredential, TokenFileMixin):
     def __init__(self, tenant_id, client_id, token_file_path, **kwargs):
         # type: (str, str, str, **Any) -> None
         super(TokenExchangeCredential, self).__init__(
             tenant_id=tenant_id,
             client_id=client_id,
-            func=self.get_service_account_token,
+            get_assertion=self.get_service_account_token,
             token_file_path=token_file_path,
             **kwargs
         )
```

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/on_behalf_of.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/on_behalf_of.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/authorization_code.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/authorization_code.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/azure_arc.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/azure_arc.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/cloud_shell.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/cloud_shell.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/browser.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/browser.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/service_fabric.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/service_fabric.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure/identity/_credentials/default.py` & `azure-identity-1.9.0b1/azure/identity/_credentials/default.py`

 * *Files identical despite different names*

## Comparing `azure-identity-1.9.0/azure_identity.egg-info/PKG-INFO` & `azure-identity-1.9.0b1/azure_identity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-identity
-Version: 1.9.0
+Version: 1.9.0b1
 Summary: Microsoft Azure Identity Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Azure Identity client library for Python
         
@@ -40,17 +40,20 @@
         When debugging and executing code locally it is typical for developers to use
         their own accounts for authenticating calls to Azure services. The Azure
         Identity library supports authenticating through developer tools to simplify
         local development.
         
         #### Authenticate via Visual Studio Code
         
-        Developers using Visual Studio Code can use the [Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account) to authenticate via the editor. Apps using `DefaultAzureCredential` or `VisualStudioCodeCredential` can then use this account to authenticate calls in their app when running locally.
-        
-        To authenticate in Visual Studio Code, ensure **version 0.9.11 or earlier** of the Azure Account extension is installed. To track progress toward supporting newer extension versions, see [this GitHub issue](https://github.com/Azure/azure-sdk-for-net/issues/27263). Once installed, open the **Command Palette** and run the **Azure: Sign In** command.
+        `DefaultAzureCredential` and `VisualStudioCodeCredential` can authenticate as
+        the user signed in to Visual Studio Code's
+        [Azure Account extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azure-account).
+        After installing the extension, sign in to Azure in Visual Studio Code by
+        pressing `F1` to open the command palette and running the `Azure: Sign In`
+        command.
         
         #### Authenticate via the Azure CLI
         
         `DefaultAzureCredential` and `AzureCliCredential` can authenticate as the user
         signed in to the [Azure CLI][azure_cli]. To sign in to the Azure CLI, run
         `az login`. On a system with a default web browser, the Azure CLI will launch
         the browser to authenticate a user.
@@ -406,34 +409,14 @@
         [vscode_cred_ref]: https://aka.ms/azsdk/python/identity/vscodecredential
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fidentity%2Fazure-identity%2FREADME.png)
         
         
         # Release History
         
-        ## 1.9.0 (2022-04-05)
-        
-        ### Features Added
-        
-        - Added PII logging if logging.DEBUG is enabled.    ([#23203](https://github.com/Azure/azure-sdk-for-python/issues/23203))
-        
-        ### Breaking Changes
-        
-        - `validate_authority` support is not available in 1.9.0.
-        
-        ### Bugs Fixed
-        
-        - Added check on `content` from msal response.    ([#23483](https://github.com/Azure/azure-sdk-for-python/issues/23483))
-        - Fixed the issue that async OBO credential does not refresh correctly.    ([#21981](https://github.com/Azure/azure-sdk-for-python/issues/21981))
-        
-        ### Other Changes
-        
-        - Removed `resource_id`, please use `identity_config` instead.
-        - Renamed argument name `get_assertion` to `func` for `ClientAssertionCredential`.
-        
         ## 1.9.0b1 (2022-03-08)
         
         ### Features Added
         
         - Added `validate_authority` support for msal client  ([#22625](https://github.com/Azure/azure-sdk-for-python/issues/22625))
         - Added `resource_id` support for user-assigned managed identity  ([#22329](https://github.com/Azure/azure-sdk-for-python/issues/22329))
         - Added `ClientAssertionCredential` support  ([#22328](https://github.com/Azure/azure-sdk-for-python/issues/22328))
@@ -1076,15 +1059,15 @@
         for more details. User authentication will be added in an upcoming preview
         release.
         
         This release supports only global Azure Active Directory tenants, i.e. those
         using the https://login.microsoftonline.com authentication endpoint.
         
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `azure-identity-1.9.0/azure_identity.egg-info/SOURCES.txt` & `azure-identity-1.9.0b1/azure_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

