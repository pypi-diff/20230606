# Comparing `tmp/stigg_api_client-0.458.4.tar.gz` & `tmp/stigg_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.458.4.tar", max compression
+gzip compressed data, was "stigg_api_client-0.5.0.tar", max compression
```

## Comparing `stigg_api_client-0.458.4.tar` & `stigg_api_client-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-06-06 10:25:40.468297 stigg_api_client-0.458.4/README.md
--rw-r--r--   0        0        0      460 2023-06-06 10:26:12.348635 stigg_api_client-0.458.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-06 10:25:40.468297 stigg_api_client-0.458.4/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-06-06 10:25:40.468297 stigg_api_client-0.458.4/stigg/client.py
--rw-r--r--   0        0        0        0 2023-06-06 10:26:10.420618 stigg_api_client-0.458.4/stigg/generated/__init__.py
--rw-r--r--   0        0        0    46503 2023-06-06 10:26:10.840622 stigg_api_client-0.458.4/stigg/generated/operations.py
--rw-r--r--   0        0        0   460528 2023-06-06 10:26:10.684620 stigg_api_client-0.458.4/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.458.4/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-24 14:47:14.271119 stigg_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-23 10:33:15.442973 stigg_api_client-0.5.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-24 07:23:15.920589 stigg_api_client-0.5.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg_api_client-0.5.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    44689 2023-04-24 14:46:41.477637 stigg_api_client-0.5.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   443944 2023-04-24 14:46:41.312733 stigg_api_client-0.5.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 stigg_api_client-0.5.0/PKG-INFO
```

### Comparing `stigg_api_client-0.458.4/README.md` & `stigg_api_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.458.4/stigg/client.py` & `stigg_api_client-0.5.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.458.4/stigg/generated/operations.py` & `stigg_api_client-0.5.0/stigg/generated/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     _frag_schedule_variables__as__DowngradeChangeVariables.addon_ref_ids()
     _frag_schedule_variables__as__DowngradeChangeVariables.billing_period()
     _frag_schedule_variables__as__DowngradeChangeVariables.downgrade_plan_ref_id()
     _frag_schedule_variables__as__BillingPeriodChangeVariables = _frag_schedule_variables.__as__(_schema.BillingPeriodChangeVariables)
     _frag_schedule_variables__as__BillingPeriodChangeVariables.billing_period()
     _frag_schedule_variables__as__UnitAmountChangeVariables = _frag_schedule_variables.__as__(_schema.UnitAmountChangeVariables)
     _frag_schedule_variables__as__UnitAmountChangeVariables.new_unit_amount()
-    _frag_schedule_variables__as__UnitAmountChangeVariables.feature_id()
     return _frag
 
 
 def fragment_subscription_fragment():
     _frag = sgqlc.operation.Fragment(_schema.CustomerSubscription, 'SubscriptionFragment')
     _frag.id()
     _frag.start_date()
@@ -288,64 +287,42 @@
     _frag_coupon.__fragment__(fragment_coupon_fragment())
     _frag_eligible_for_trial = _frag.eligible_for_trial()
     _frag_eligible_for_trial.product_id()
     _frag_eligible_for_trial.product_ref_id()
     _frag_eligible_for_trial.eligible()
     _frag_promotional_entitlements = _frag.promotional_entitlements()
     _frag_promotional_entitlements.__fragment__(fragment_promotional_entitlement_fragment())
-    return _frag
-
-
-def fragment_customer_with_subscriptions_fragment():
-    _frag = sgqlc.operation.Fragment(_schema.Customer, 'CustomerWithSubscriptionsFragment')
-    _frag.__fragment__(fragment_customer_fragment())
     _frag_subscriptions = _frag.subscriptions()
     _frag_subscriptions.__fragment__(fragment_subscription_fragment())
     return _frag
 
 
 def fragment_subscription_preview_fragment():
     _frag = sgqlc.operation.Fragment(_schema.SubscriptionPreview, 'SubscriptionPreviewFragment')
     _frag_sub_total = _frag.sub_total()
     _frag_sub_total.amount()
     _frag_sub_total.currency()
-    _frag_total_excluding_tax = _frag.total_excluding_tax()
-    _frag_total_excluding_tax.amount()
-    _frag_total_excluding_tax.currency()
     _frag_total = _frag.total()
     _frag_total.amount()
     _frag_total.currency()
-    _frag_tax_details = _frag.tax_details()
-    _frag_tax_details.display_name()
-    _frag_tax_details.percentage()
-    _frag_tax_details.inclusive()
-    _frag_tax = _frag.tax()
-    _frag_tax.amount()
-    _frag_tax.currency()
     _frag_billing_period_range = _frag.billing_period_range()
     _frag_billing_period_range.start()
     _frag_billing_period_range.end()
     _frag_discount = _frag.discount()
     _frag_discount.type()
     _frag_discount.value()
     _frag_discount.duration_type()
     _frag_discount.duration_in_months()
     _frag_subscription = _frag.subscription()
     _frag_subscription_sub_total = _frag_subscription.sub_total()
     _frag_subscription_sub_total.amount()
     _frag_subscription_sub_total.currency()
-    _frag_subscription_total_excluding_tax = _frag_subscription.total_excluding_tax()
-    _frag_subscription_total_excluding_tax.amount()
-    _frag_subscription_total_excluding_tax.currency()
     _frag_subscription_total = _frag_subscription.total()
     _frag_subscription_total.amount()
     _frag_subscription_total.currency()
-    _frag_subscription_tax = _frag_subscription.tax()
-    _frag_subscription_tax.amount()
-    _frag_subscription_tax.currency()
     _frag_proration = _frag.proration()
     _frag_proration.proration_date()
     _frag_proration_credit = _frag_proration.credit()
     _frag_proration_credit.amount()
     _frag_proration_credit.currency()
     _frag_proration_debit = _frag_proration.debit()
     _frag_proration_debit.amount()
@@ -654,15 +631,14 @@
     _frag_schedule_variables__as__DowngradeChangeVariables.addon_ref_ids()
     _frag_schedule_variables__as__DowngradeChangeVariables.billing_period()
     _frag_schedule_variables__as__DowngradeChangeVariables.downgrade_plan_ref_id()
     _frag_schedule_variables__as__BillingPeriodChangeVariables = _frag_schedule_variables.__as__(_schema.BillingPeriodChangeVariables)
     _frag_schedule_variables__as__BillingPeriodChangeVariables.billing_period()
     _frag_schedule_variables__as__UnitAmountChangeVariables = _frag_schedule_variables.__as__(_schema.UnitAmountChangeVariables)
     _frag_schedule_variables__as__UnitAmountChangeVariables.new_unit_amount()
-    _frag_schedule_variables__as__UnitAmountChangeVariables.feature_id()
     return _frag
 
 
 def fragment_customer_portal_entitlement():
     _frag = sgqlc.operation.Fragment(_schema.Entitlement, 'CustomerPortalEntitlement')
     _frag.is_granted()
     _frag.usage_limit()
@@ -788,16 +764,14 @@
     _frag_plans.__fragment__(fragment_plan_fragment())
     _frag_currency = _frag.currency()
     _frag_currency.__fragment__(fragment_paywall_currency())
     _frag_configuration = _frag.configuration()
     _frag_configuration.__fragment__(fragment_paywall_configuration_fragment())
     _frag_customer = _frag.customer()
     _frag_customer.__fragment__(fragment_customer_fragment())
-    _frag_active_subscriptions = _frag.active_subscriptions()
-    _frag_active_subscriptions.__fragment__(fragment_subscription_fragment())
     _frag_resource = _frag.resource()
     _frag_resource.__fragment__(fragment_customer_resource_fragment())
     return _frag
 
 
 class Fragment:
     addon_fragment = fragment_addon_fragment()
@@ -808,15 +782,14 @@
     customer_portal_entitlement = fragment_customer_portal_entitlement()
     customer_portal_fragment = fragment_customer_portal_fragment()
     customer_portal_promotional_entitlement = fragment_customer_portal_promotional_entitlement()
     customer_portal_subscription_addon = fragment_customer_portal_subscription_addon()
     customer_portal_subscription_fragment = fragment_customer_portal_subscription_fragment()
     customer_portal_subscription_scheduled_update_data = fragment_customer_portal_subscription_scheduled_update_data()
     customer_resource_fragment = fragment_customer_resource_fragment()
-    customer_with_subscriptions_fragment = fragment_customer_with_subscriptions_fragment()
     entitlement_fragment = fragment_entitlement_fragment()
     entitlement_usage_updated = fragment_entitlement_usage_updated()
     entitlements_updated_payload = fragment_entitlements_updated_payload()
     feature_fragment = fragment_feature_fragment()
     font_variant_fragment = fragment_font_variant_fragment()
     layout_configuration_fragment = fragment_layout_configuration_fragment()
     mock_paywall_addon_fragment = fragment_mock_paywall_addon_fragment()
@@ -868,15 +841,15 @@
     _op_import_customer.__fragment__(fragment_slim_customer_fragment())
     return _op
 
 
 def mutation_update_customer():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='UpdateCustomer', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.UpdateCustomerInput))))
     _op_update_customer = _op.update_one_customer(input=sgqlc.types.Variable('input'), __alias__='update_customer')
-    _op_update_customer.__fragment__(fragment_slim_customer_fragment())
+    _op_update_customer.__fragment__(fragment_customer_fragment())
     return _op
 
 
 def mutation_provision_subscription():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='ProvisionSubscription', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.ProvisionSubscriptionInput))))
     _op_provision_subscription = _op.provision_subscription_v2(input=sgqlc.types.Variable('input'), __alias__='provision_subscription')
     _op_provision_subscription.checkout_url()
@@ -953,44 +926,36 @@
 def mutation_create_subscription():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='CreateSubscription', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.SubscriptionInput))))
     _op_create_subscription = _op.create_subscription(subscription=sgqlc.types.Variable('input'))
     _op_create_subscription.__fragment__(fragment_slim_subscription_fragment())
     return _op
 
 
-def mutation_migrate_subscription_to_latest():
-    _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='MigrateSubscriptionToLatest', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.SubscriptionMigrationInput))))
-    _op_migrate_subscription_to_latest = _op.migrate_subscription_to_latest(input=sgqlc.types.Variable('input'))
-    _op_migrate_subscription_to_latest.subscription_id()
-    return _op
-
-
 class Mutation:
     cancel_subscription = mutation_cancel_subscription()
     cancel_subscription_updates = mutation_cancel_subscription_updates()
     create_subscription = mutation_create_subscription()
     estimate_subscription = mutation_estimate_subscription()
     estimate_subscription_update = mutation_estimate_subscription_update()
     import_customer = mutation_import_customer()
     import_customer_bulk = mutation_import_customer_bulk()
     import_subscriptions_bulk = mutation_import_subscriptions_bulk()
     initiate_checkout = mutation_initiate_checkout()
-    migrate_subscription_to_latest = mutation_migrate_subscription_to_latest()
     provision_customer = mutation_provision_customer()
     provision_subscription = mutation_provision_subscription()
     report_entitlement_check_requested = mutation_report_entitlement_check_requested()
     report_usage = mutation_report_usage()
     update_customer = mutation_update_customer()
     update_subscription = mutation_update_subscription()
 
 
 def query_get_customer_by_id():
     _op = sgqlc.operation.Operation(_schema_root.query_type, name='GetCustomerById', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.GetCustomerByRefIdInput))))
     _op_get_customer_by_ref_id = _op.get_customer_by_ref_id(input=sgqlc.types.Variable('input'))
-    _op_get_customer_by_ref_id.__fragment__(fragment_customer_with_subscriptions_fragment())
+    _op_get_customer_by_ref_id.__fragment__(fragment_customer_fragment())
     return _op
 
 
 def query_get_active_subscriptions():
     _op = sgqlc.operation.Operation(_schema_root.query_type, name='GetActiveSubscriptions', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.GetActiveSubscriptionsInput))))
     _op_get_active_subscriptions = _op.get_active_subscriptions(input=sgqlc.types.Variable('input'))
     _op_get_active_subscriptions.__fragment__(fragment_subscription_fragment())
```

### Comparing `stigg_api_client-0.458.4/stigg/generated/schema.py` & `stigg_api_client-0.5.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,14 @@
 
 
 class AddonSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'description', 'displayName', 'environmentId', 'id', 'isLatest', 'pricingType', 'productId', 'refId', 'status', 'updatedAt', 'versionNumber')
 
 
-class AggregationFunction(sgqlc.types.Enum):
-    __schema__ = schema
-    __choices__ = ('AVG', 'COUNT', 'MAX', 'MIN', 'SUM', 'UNIQUE')
-
-
 class Alignment(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('CENTER', 'LEFT', 'RIGHT')
 
 
 class ApiKeySortFields(sgqlc.types.Enum):
     __schema__ = schema
@@ -68,19 +63,14 @@
 Boolean = sgqlc.types.Boolean
 
 class ChangeType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('ADDED', 'DELETED', 'MODIFIED', 'REORDERED')
 
 
-class ConditionOperation(sgqlc.types.Enum):
-    __schema__ = schema
-    __choices__ = ('EQUALS', 'GREATER_THAN', 'GREATER_THAN_OR_EQUAL', 'IS_NOT_NULL', 'IS_NULL', 'LESS_THAN', 'LESS_THAN_OR_EQUAL', 'NOT_EQUALS')
-
-
 class ConnectionCursor(sgqlc.types.Scalar):
     __schema__ = schema
 
 
 class CouponSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'description', 'environmentId', 'id', 'name', 'refId', 'status', 'type', 'updatedAt')
@@ -109,15 +99,15 @@
 class CustomerSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('billingId', 'createdAt', 'crmHubspotCompanyId', 'crmHubspotCompanyUrl', 'crmId', 'customerId', 'email', 'environmentId', 'id', 'name', 'refId', 'updatedAt')
 
 
 class CustomerSubscriptionSortFields(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('billingId', 'cancelReason', 'cancellationDate', 'createdAt', 'crmId', 'crmLinkUrl', 'effectiveEndDate', 'endDate', 'environmentId', 'id', 'oldBillingId', 'pricingType', 'refId', 'resourceId', 'startDate', 'status', 'subscriptionId', 'trialEndDate')
+    __choices__ = ('billingId', 'cancelReason', 'cancellationDate', 'createdAt', 'crmId', 'crmLinkUrl', 'effectiveEndDate', 'endDate', 'environmentId', 'id', 'oldBillingId', 'pricingType', 'refId', 'startDate', 'status', 'subscriptionId', 'trialEndDate')
 
 
 DateTime = sgqlc.types.datetime.DateTime
 
 class Department(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('CEO_OR_FOUNDER', 'ENGINEERING', 'GROWTH', 'MARKETING', 'MONETIZATION', 'OTHER', 'PRODUCT')
@@ -151,15 +141,15 @@
 class EnvironmentSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'displayName', 'id', 'slug')
 
 
 class ErrorCode(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('AccountNotFoundError', 'AddonHasToHavePriceError', 'AddonNotFound', 'AddonWithDraftCannotBeDeletedError', 'ArchivedCouponCantBeApplied', 'AuthCustomerMismatch', 'BadUserInput', 'BillingPeriodMissingError', 'CannotDeleteCustomerError', 'CannotDeleteFeatureError', 'CannotDeleteProductError', 'CannotEditPackageInNonDraftMode', 'CheckoutIsNotSupported', 'CheckoutOptionsMissing', 'CouponNotFound', 'CustomerAlreadyHaveCustomerCoupon', 'CustomerAlreadyUsesCoupon', 'CustomerHasNoPaymentMethod', 'CustomerNoBillingId', 'CustomerNotFound', 'CustomerResourceNotFound', 'DowngradeBillingPeriodNotSupportedError', 'DraftPlanCantBeArchived', 'DuplicatedEntityNotAllowed', 'EditAllowedOnDraftPackageOnlyError', 'EntitlementsMustBelongToSamePackage', 'EntityIdDifferentFromRefIdError', 'EnvironmentMissing', 'ExperimentAlreadyRunning', 'ExperimentNotFoundError', 'ExperimentStatusError', 'FailedToCreateCheckoutSessionError', 'FailedToImportCustomer', 'FeatureNotFound', 'FetchAllCountriesPricesNotAllowed', 'IdentityForbidden', 'ImportAlreadyInProgress', 'InitStripePaymentMethodError', 'IntegrationNotFound', 'IntegrityViolation', 'InvalidAddressError', 'InvalidArgumentError', 'InvalidCancellationDate', 'InvalidEntitlementResetPeriod', 'InvalidMemberDelete', 'InvalidQuantity', 'InvalidSubscriptionStatus', 'InvalidUpdatePriceUnitAmountError', 'MemberInvitationError', 'MemberNotFound', 'MeterDoesNotBelongToTheEntitlementFeature', 'MeterMustBeAssociatedToIncrementalFeature', 'MeteringNotAvailableForFeatureType', 'MissingEntityIdError', 'NoFeatureEntitlementInSubscription', 'NoProductsAvailable', 'OperationNotAllowedDuringInProgressExperiment', 'PackageAlreadyPublished', 'PackagePricingTypeNotSet', 'PaymentMethodNotFoundError', 'PlanAlreadyExtended', 'PlanCannotBePublishWhenBasePlanIsDraft', 'PlanIsUsedAsDefaultStartPlan', 'PlanIsUsedAsDowngradePlan', 'PlanNotFound', 'PlanWithChildCantBeDeleted', 'PlansCircularDependencyError', 'PriceNotFound', 'PromotionCodeCustomerNotFirstPurchase', 'PromotionCodeMaxRedemptionsReached', 'PromotionCodeMinimumAmountNotReached', 'PromotionCodeNotActive', 'PromotionCodeNotForCustomer', 'PromotionCodeNotFound', 'RateLimitExceeded', 'ResyncAlreadyInProgress', 'ScheduledMigrationAlreadyExistsError', 'SelectedBillingModelDoesntMatchImportedItemError', 'StripeCustomerIsDeleted', 'StripeError', 'SubscriptionAlreadyCanceledOrExpired', 'SubscriptionAlreadyOnLatestPlanError', 'SubscriptionMustHaveSinglePlanError', 'SubscriptionNotFound', 'TooManySubscriptionsPerCustomer', 'TrialMinDateError', 'TrialMustBeCancelledImmediately', 'UnPublishedPackage', 'Unauthenticated', 'UncompatibleSubscriptionAddon', 'UnexpectedError', 'UnsupportedFeatureType', 'UnsupportedSubscriptionScheduleType', 'UnsupportedVendorIdentifier')
+    __choices__ = ('AccountNotFoundError', 'AddonHasToHavePriceError', 'AddonNotFound', 'ArchivedCouponCantBeApplied', 'AuthCustomerMismatch', 'BadUserInput', 'BillingPeriodMissingError', 'CannotDeleteCustomerError', 'CannotDeleteFeatureError', 'CannotDeleteProductError', 'CannotEditPackageInNonDraftMode', 'CheckoutIsNotSupported', 'CheckoutOptionsMissing', 'CouponNotFound', 'CustomerAlreadyHaveCustomerCoupon', 'CustomerAlreadyUsesCoupon', 'CustomerHasNoPaymentMethod', 'CustomerNoBillingId', 'CustomerNotFound', 'CustomerResourceNotFound', 'DowngradeBillingPeriodNotSupportedError', 'DraftPlanCantBeArchived', 'DuplicatedEntityNotAllowed', 'EditAllowedOnDraftPackageOnlyError', 'EntitlementsMustBelongToSamePackage', 'EntityIdDifferentFromRefIdError', 'EnvironmentMissing', 'ExperimentAlreadyRunning', 'ExperimentNotFoundError', 'ExperimentStatusError', 'FailedToCreateCheckoutSessionError', 'FailedToImportCustomer', 'FeatureNotFound', 'FetchAllCountriesPricesNotAllowed', 'IdentityForbidden', 'ImportAlreadyInProgress', 'InitStripePaymentMethodError', 'IntegrationNotFound', 'IntegrityViolation', 'InvalidAddressError', 'InvalidArgumentError', 'InvalidCancellationDate', 'InvalidEntitlementResetPeriod', 'InvalidMemberDelete', 'InvalidQuantity', 'InvalidSubscriptionStatus', 'InvalidUpdatePriceUnitAmountError', 'InvalidUsageValueForIncrementalFeatureError', 'MemberInvitationError', 'MemberNotFound', 'MeteringNotAvailableForFeatureType', 'MissingEntityIdError', 'NoFeatureEntitlementInSubscription', 'NoProductsAvailable', 'OperationNotAllowedDuringInProgressExperiment', 'PackageAlreadyPublished', 'PackagePricingTypeNotSet', 'PlanAlreadyExtended', 'PlanCannotBePublishWhenBasePlanIsDraft', 'PlanIsUsedAsDefaultStartPlan', 'PlanIsUsedAsDowngradePlan', 'PlanNotFound', 'PlanWithChildCantBeDeleted', 'PlansCircularDependencyError', 'PriceNotFound', 'PromotionCodeCustomerNotFirstPurchase', 'PromotionCodeMaxRedemptionsReached', 'PromotionCodeMinimumAmountNotReached', 'PromotionCodeNotActive', 'PromotionCodeNotForCustomer', 'PromotionCodeNotFound', 'RateLimitExceeded', 'ResyncAlreadyInProgress', 'SelectedBillingModelDoesntMatchImportedItemError', 'StripeCustomerIsDeleted', 'SubscriptionAlreadyCanceledOrExpired', 'SubscriptionMustHaveSinglePlanError', 'SubscriptionNotFound', 'TrialMinDateError', 'TrialMustBeCancelledImmediately', 'UnPublishedPackage', 'Unauthenticated', 'UncompatibleSubscriptionAddon', 'UnexpectedError', 'UnsupportedFeatureType', 'UnsupportedSubscriptionScheduleType', 'UnsupportedVendorIdentifier')
 
 
 class EventLogType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('ADDON_CREATED', 'ADDON_DELETED', 'ADDON_UPDATED', 'COUPON_ARCHIVED', 'COUPON_CREATED', 'COUPON_UPDATED', 'CREATE_SUBSCRIPTION_FAILED', 'CUSTOMER_CREATED', 'CUSTOMER_DELETED', 'CUSTOMER_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_PAYMENT_FAILED', 'CUSTOMER_RESOURCE_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_UPDATED', 'EDGE_API_DATA_RESYNC', 'ENTITLEMENTS_UPDATED', 'ENTITLEMENT_DENIED', 'ENTITLEMENT_GRANTED', 'ENTITLEMENT_REQUESTED', 'ENVIRONMENT_DELETED', 'FEATURE_CREATED', 'FEATURE_DELETED', 'FEATURE_UPDATED', 'IMPORT_INTEGRATION_CATALOG_TRIGGERED', 'IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED', 'MEASUREMENT_REPORTED', 'PACKAGE_PUBLISHED', 'PLAN_CREATED', 'PLAN_DELETED', 'PLAN_UPDATED', 'PRODUCT_CREATED', 'PRODUCT_DELETED', 'PRODUCT_UPDATED', 'PROMOTIONAL_ENTITLEMENT_EXPIRED', 'PROMOTIONAL_ENTITLEMENT_GRANTED', 'PROMOTIONAL_ENTITLEMENT_REVOKED', 'PROMOTIONAL_ENTITLEMENT_UPDATED', 'RESYNC_INTEGRATION_TRIGGERED', 'SUBSCRIPTION_CANCELED', 'SUBSCRIPTION_CREATED', 'SUBSCRIPTION_EXPIRED', 'SUBSCRIPTION_TRIAL_CONVERTED', 'SUBSCRIPTION_TRIAL_ENDS_SOON', 'SUBSCRIPTION_TRIAL_EXPIRED', 'SUBSCRIPTION_TRIAL_STARTED', 'SUBSCRIPTION_UPDATED', 'SUBSCRIPTION_USAGE_UPDATED', 'SYNC_FAILED', 'WIDGET_CONFIGURATION_UPDATED')
 
 
@@ -229,19 +219,14 @@
 
 
 class MemberStatus(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('INVITED', 'REGISTERED')
 
 
-class MeterSortFields(sgqlc.types.Enum):
-    __schema__ = schema
-    __choices__ = ('createdAt', 'environmentId', 'id', 'updatedAt')
-
-
 class MeterType(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('Fluctuating', 'Incremental', 'None')
 
 
 class MonthlyAccordingTo(sgqlc.types.Enum):
     __schema__ = schema
@@ -366,32 +351,27 @@
 
 
 class SubscriptionMigrationTaskSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id', 'status', 'taskType')
 
 
-class SubscriptionMigrationTime(sgqlc.types.Enum):
-    __schema__ = schema
-    __choices__ = ('END_OF_BILLING_PERIOD', 'IMMEDIATE')
-
-
 class SubscriptionPriceSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'id', 'updatedAt', 'usageLimit')
 
 
 class SubscriptionScheduleStatus(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('Canceled', 'Done', 'Failed', 'Scheduled')
 
 
 class SubscriptionScheduleType(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('BillingPeriod', 'Downgrade', 'MigrateToLatest', 'UnitAmount')
+    __choices__ = ('BillingPeriod', 'Downgrade', 'UnitAmount')
 
 
 class SubscriptionStartSetup(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('FREE_PLAN', 'PLAN_SELECTION', 'TRIAL_PERIOD')
 
 
@@ -563,21 +543,14 @@
     customer_id = sgqlc.types.Field(String, graphql_name='customerId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     payment_method_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='paymentMethodId')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     vendor_identifier = sgqlc.types.Field(sgqlc.types.non_null(VendorIdentifier), graphql_name='vendorIdentifier')
 
 
-class BillableFeatureInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('feature_id', 'quantity')
-    feature_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureId')
-    quantity = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='quantity')
-
-
 class BillingModelFilterComparison(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
     eq = sgqlc.types.Field(BillingModel, graphql_name='eq')
     gt = sgqlc.types.Field(BillingModel, graphql_name='gt')
     gte = sgqlc.types.Field(BillingModel, graphql_name='gte')
     i_like = sgqlc.types.Field(BillingModel, graphql_name='iLike')
@@ -797,23 +770,14 @@
 
 class CreateManyPromotionalEntitlementsInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('promotional_entitlements',)
     promotional_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PromotionalEntitlementInput'))), graphql_name='promotionalEntitlements')
 
 
-class CreateMeter(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('aggregation', 'environment_id', 'feature_id', 'filters')
-    aggregation = sgqlc.types.Field(sgqlc.types.non_null('MeterAggregation'), graphql_name='aggregation')
-    environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
-    feature_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureId')
-    filters = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MeterFilterDefinitionInput'))), graphql_name='filters')
-
-
 class CreateOneEnvironmentInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('environment', 'options')
     environment = sgqlc.types.Field(sgqlc.types.non_null(CreateEnvironment), graphql_name='environment')
     options = sgqlc.types.Field(CreateEnvironmentOptions, graphql_name='options')
 
 
@@ -831,20 +795,14 @@
 
 class CreateOneIntegrationInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('integration',)
     integration = sgqlc.types.Field(sgqlc.types.non_null(CreateIntegrationInput), graphql_name='integration')
 
 
-class CreateOneMeterInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('meter',)
-    meter = sgqlc.types.Field(sgqlc.types.non_null(CreateMeter), graphql_name='meter')
-
-
 class CreateOneProductInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('product',)
     product = sgqlc.types.Field(sgqlc.types.non_null('ProductCreateInput'), graphql_name='product')
 
 
 class CursorPaging(sgqlc.types.Input):
@@ -889,15 +847,15 @@
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     subscriptions = sgqlc.types.Field('CustomerFilterCustomerSubscriptionFilter', graphql_name='subscriptions')
     updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
 
 
 class CustomerFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
     crm_link_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmLinkUrl')
@@ -905,15 +863,14 @@
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerFilterCustomerSubscriptionFilter')), graphql_name='or')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
-    resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
 
 
 class CustomerFilterPromotionalEntitlementFilter(sgqlc.types.Input):
@@ -1001,15 +958,15 @@
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerFilter')), graphql_name='or')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
 
 
 class CustomerResourceFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
     crm_link_url = sgqlc.types.Field('StringFieldComparison', graphql_name='crmLinkUrl')
@@ -1017,15 +974,14 @@
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerResourceFilterCustomerSubscriptionFilter')), graphql_name='or')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
-    resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
 
 
 class CustomerResourceSort(sgqlc.types.Input):
@@ -1042,15 +998,15 @@
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(CustomerSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
 class CustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('addons', 'and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'customer', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'plan', 'prices', 'pricing_type', 'ref_id', 'resource', 'resource_id', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('addons', 'and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'customer', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'prices', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_entitlements', 'subscription_id', 'trial_end_date')
     addons = sgqlc.types.Field('CustomerSubscriptionFilterSubscriptionAddonFilter', graphql_name='addons')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field('DateFieldComparison', graphql_name='cancellationDate')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     crm_id = sgqlc.types.Field('StringFieldComparison', graphql_name='crmId')
@@ -1058,20 +1014,17 @@
     customer = sgqlc.types.Field('CustomerSubscriptionFilterCustomerFilter', graphql_name='customer')
     effective_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='endDate')
     environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     old_billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilter')), graphql_name='or')
-    plan = sgqlc.types.Field('CustomerSubscriptionFilterPlanFilter', graphql_name='plan')
     prices = sgqlc.types.Field('CustomerSubscriptionFilterSubscriptionPriceFilter', graphql_name='prices')
     pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
-    resource = sgqlc.types.Field('CustomerSubscriptionFilterCustomerResourceFilter', graphql_name='resource')
-    resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
     start_date = sgqlc.types.Field('DateFieldComparison', graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_entitlements = sgqlc.types.Field('CustomerSubscriptionFilterSubscriptionEntitlementFilter', graphql_name='subscriptionEntitlements')
     subscription_id = sgqlc.types.Field('StringFieldComparison', graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field('DateFieldComparison', graphql_name='trialEndDate')
 
 
@@ -1090,44 +1043,14 @@
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     name = sgqlc.types.Field('StringFieldComparison', graphql_name='name')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterCustomerFilter')), graphql_name='or')
     ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
     updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
 
 
-class CustomerSubscriptionFilterCustomerResourceFilter(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('and_', 'created_at', 'environment_id', 'or_', 'resource_id')
-    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterCustomerResourceFilter')), graphql_name='and')
-    created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
-    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
-    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterCustomerResourceFilter')), graphql_name='or')
-    resource_id = sgqlc.types.Field('StringFieldComparison', graphql_name='resourceId')
-
-
-class CustomerSubscriptionFilterPlanFilter(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'created_at', 'description', 'display_name', 'environment_id', 'id', 'is_latest', 'or_', 'pricing_type', 'product_id', 'ref_id', 'status', 'updated_at', 'version_number')
-    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterPlanFilter')), graphql_name='and')
-    billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
-    created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
-    description = sgqlc.types.Field('StringFieldComparison', graphql_name='description')
-    display_name = sgqlc.types.Field('StringFieldComparison', graphql_name='displayName')
-    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
-    id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
-    is_latest = sgqlc.types.Field(BooleanFieldComparison, graphql_name='isLatest')
-    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterPlanFilter')), graphql_name='or')
-    pricing_type = sgqlc.types.Field('PricingTypeFilterComparison', graphql_name='pricingType')
-    product_id = sgqlc.types.Field('StringFieldComparison', graphql_name='productId')
-    ref_id = sgqlc.types.Field('StringFieldComparison', graphql_name='refId')
-    status = sgqlc.types.Field('PackageStatusFilterComparison', graphql_name='status')
-    updated_at = sgqlc.types.Field('DateFieldComparison', graphql_name='updatedAt')
-    version_number = sgqlc.types.Field('IntFieldComparison', graphql_name='versionNumber')
-
-
 class CustomerSubscriptionFilterSubscriptionAddonFilter(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('and_', 'created_at', 'id', 'or_', 'quantity', 'updated_at')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterSubscriptionAddonFilter')), graphql_name='and')
     created_at = sgqlc.types.Field('DateFieldComparison', graphql_name='createdAt')
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionFilterSubscriptionAddonFilter')), graphql_name='or')
@@ -1326,28 +1249,27 @@
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(EnvironmentSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
 class EstimateSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('addons', 'billing_country_code', 'billing_information', 'billing_period', 'customer_id', 'environment_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'resource_id', 'skip_trial', 'start_date', 'unit_quantity')
+    __field_names__ = ('addons', 'billing_country_code', 'billing_information', 'billing_period', 'customer_id', 'environment_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'resource_id', 'skip_trial', 'start_date')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     skip_trial = sgqlc.types.Field(Boolean, graphql_name='skipTrial')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
-    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
 
 
 class EstimateSubscriptionUpdateInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('addons', 'environment_id', 'promotion_code', 'subscription_id', 'unit_quantity')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
@@ -1781,54 +1703,14 @@
     __schema__ = schema
     __field_names__ = ('direction', 'field', 'nulls')
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(MemberSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
-class MeterAggregation(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('field', 'function')
-    field = sgqlc.types.Field(String, graphql_name='field')
-    function = sgqlc.types.Field(sgqlc.types.non_null(AggregationFunction), graphql_name='function')
-
-
-class MeterConditionInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('field', 'operation', 'value')
-    field = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='field')
-    operation = sgqlc.types.Field(sgqlc.types.non_null(ConditionOperation), graphql_name='operation')
-    value = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='value')
-
-
-class MeterFilter(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('and_', 'created_at', 'environment_id', 'id', 'or_', 'updated_at')
-    and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('MeterFilter')), graphql_name='and')
-    created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
-    environment_id = sgqlc.types.Field('StringFieldComparison', graphql_name='environmentId')
-    id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
-    or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('MeterFilter')), graphql_name='or')
-    updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
-
-
-class MeterFilterDefinitionInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('conditions',)
-    conditions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MeterConditionInput))), graphql_name='conditions')
-
-
-class MeterSort(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('direction', 'field', 'nulls')
-    direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
-    field = sgqlc.types.Field(sgqlc.types.non_null(MeterSortFields), graphql_name='field')
-    nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
-
-
 class MeterTypeFilterComparison(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('eq', 'gt', 'gte', 'i_like', 'in_', 'is_', 'is_not', 'like', 'lt', 'lte', 'neq', 'not_ilike', 'not_in', 'not_like')
     eq = sgqlc.types.Field(MeterType, graphql_name='eq')
     gt = sgqlc.types.Field(MeterType, graphql_name='gt')
     gte = sgqlc.types.Field(MeterType, graphql_name='gte')
     i_like = sgqlc.types.Field(MeterType, graphql_name='iLike')
@@ -1958,23 +1840,22 @@
     status = sgqlc.types.Field('PackageStatusFilterComparison', graphql_name='status')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     version_number = sgqlc.types.Field(IntFieldComparison, graphql_name='versionNumber')
 
 
 class PackageEntitlementInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('description', 'display_name_override', 'environment_id', 'feature_id', 'has_unlimited_usage', 'hidden_from_widgets', 'is_custom', 'meter_id', 'monthly_reset_period_configuration', 'order', 'package_id', 'reset_period', 'usage_limit', 'weekly_reset_period_configuration')
+    __field_names__ = ('description', 'display_name_override', 'environment_id', 'feature_id', 'has_unlimited_usage', 'hidden_from_widgets', 'is_custom', 'monthly_reset_period_configuration', 'order', 'package_id', 'reset_period', 'usage_limit', 'weekly_reset_period_configuration')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name_override = sgqlc.types.Field(String, graphql_name='displayNameOverride')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     feature_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureId')
     has_unlimited_usage = sgqlc.types.Field(Boolean, graphql_name='hasUnlimitedUsage')
     hidden_from_widgets = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(WidgetType)), graphql_name='hiddenFromWidgets')
     is_custom = sgqlc.types.Field(Boolean, graphql_name='isCustom')
-    meter_id = sgqlc.types.Field(String, graphql_name='meterId')
     monthly_reset_period_configuration = sgqlc.types.Field(MonthlyResetPeriodConfigInput, graphql_name='monthlyResetPeriodConfiguration')
     order = sgqlc.types.Field(Float, graphql_name='order')
     package_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='packageId')
     reset_period = sgqlc.types.Field(EntitlementResetPeriod, graphql_name='resetPeriod')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
     weekly_reset_period_configuration = sgqlc.types.Field('WeeklyResetPeriodConfigInput', graphql_name='weeklyResetPeriodConfiguration')
 
@@ -2000,19 +1881,18 @@
     reset_period = sgqlc.types.Field(EntitlementResetPeriod, graphql_name='resetPeriod')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
     weekly_reset_period_configuration = sgqlc.types.Field('WeeklyResetPeriodConfigInput', graphql_name='weeklyResetPeriodConfiguration')
 
 
 class PackagePricingInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('environment_id', 'package_id', 'pricing_model', 'pricing_models', 'pricing_type')
+    __field_names__ = ('environment_id', 'package_id', 'pricing_model', 'pricing_type')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     package_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='packageId')
     pricing_model = sgqlc.types.Field('PricingModelCreateInput', graphql_name='pricingModel')
-    pricing_models = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('PricingModelCreateInput')), graphql_name='pricingModels')
     pricing_type = sgqlc.types.Field(sgqlc.types.non_null(PricingType), graphql_name='pricingType')
 
 
 class PackagePublishInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('id', 'migration_type')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
@@ -2380,86 +2260,80 @@
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     should_sync_free = sgqlc.types.Field(Boolean, graphql_name='shouldSyncFree')
     subscription_params = sgqlc.types.Field('ProvisionCustomerSubscriptionInput', graphql_name='subscriptionParams')
 
 
 class ProvisionCustomerSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billable_features', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_id', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
-    billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
-    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
 
 
 class ProvisionSandboxInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('billing_model', 'display_name')
     billing_model = sgqlc.types.Field(sgqlc.types.non_null(BillingModel), graphql_name='billingModel')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
 
 
 class ProvisionSubscription(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billable_features', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
-    billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     checkout_options = sgqlc.types.Field(CheckoutOptions, graphql_name='checkoutOptions')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     skip_trial = sgqlc.types.Field(Boolean, graphql_name='skipTrial')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
-    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
 
 
 class ProvisionSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billable_features', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
-    billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     checkout_options = sgqlc.types.Field(CheckoutOptions, graphql_name='checkoutOptions')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     skip_trial = sgqlc.types.Field(Boolean, graphql_name='skipTrial')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
-    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
 
 
 class RemoveBasePlanFromPlanInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('id', 'relation_id')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     relation_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='relationId')
@@ -2645,15 +2519,15 @@
     status = sgqlc.types.Field(PackageStatusFilterComparison, graphql_name='status')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     version_number = sgqlc.types.Field(IntFieldComparison, graphql_name='versionNumber')
 
 
 class SubscriptionAddonFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field('SubscriptionCancelReasonFilterComparison', graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
@@ -2661,15 +2535,14 @@
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonFilterCustomerSubscriptionFilter')), graphql_name='or')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
-    resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
 
 
 class SubscriptionAddonFilterPriceFilter(sgqlc.types.Input):
@@ -2745,15 +2618,15 @@
     subscription = sgqlc.types.Field('SubscriptionEntitlementFilterCustomerSubscriptionFilter', graphql_name='subscription')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
 
 
 class SubscriptionEntitlementFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionEntitlementFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReasonFilterComparison, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
@@ -2761,15 +2634,14 @@
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionEntitlementFilterCustomerSubscriptionFilter')), graphql_name='or')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
-    resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
 
 
 class SubscriptionEntitlementFilterFeatureFilter(sgqlc.types.Input):
@@ -2807,19 +2679,18 @@
     direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='direction')
     field = sgqlc.types.Field(sgqlc.types.non_null(SubscriptionEntitlementSortFields), graphql_name='field')
     nulls = sgqlc.types.Field(SortNulls, graphql_name='nulls')
 
 
 class SubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billable_features', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'crm_id', 'customer_id', 'end_date', 'environment_id', 'is_custom_price_subscription', 'is_overriding_trial_config', 'is_trial', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_entitlements', 'subscription_id', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'crm_id', 'customer_id', 'end_date', 'environment_id', 'is_custom_price_subscription', 'is_overriding_trial_config', 'is_trial', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_entitlements', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonInput)), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
-    billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field(SubscriptionBillingInfo, graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
@@ -2831,23 +2702,21 @@
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     subscription_entitlements = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionEntitlementInput)), graphql_name='subscriptionEntitlements')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
-    unit_quantity = sgqlc.types.Field(Float, graphql_name='unitQuantity')
 
 
 class SubscriptionMigrationInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('environment_id', 'subscription_id', 'subscription_migration_time')
+    __field_names__ = ('environment_id', 'subscription_id')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     subscription_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='subscriptionId')
-    subscription_migration_time = sgqlc.types.Field(SubscriptionMigrationTime, graphql_name='subscriptionMigrationTime')
 
 
 class SubscriptionMigrationTaskFilter(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('and_', 'created_at', 'environment_id', 'id', 'or_', 'status', 'task_type')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionMigrationTaskFilter')), graphql_name='and')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
@@ -2877,15 +2746,15 @@
     subscription = sgqlc.types.Field('SubscriptionPriceFilterCustomerSubscriptionFilter', graphql_name='subscription')
     updated_at = sgqlc.types.Field(DateFieldComparison, graphql_name='updatedAt')
     usage_limit = sgqlc.types.Field(NumberFieldComparison, graphql_name='usageLimit')
 
 
 class SubscriptionPriceFilterCustomerSubscriptionFilter(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('and_', 'billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'or_', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterCustomerSubscriptionFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReasonFilterComparison, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateFieldComparison, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateFieldComparison, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(StringFieldComparison, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(StringFieldComparison, graphql_name='crmLinkUrl')
@@ -2893,15 +2762,14 @@
     end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='endDate')
     environment_id = sgqlc.types.Field(StringFieldComparison, graphql_name='environmentId')
     id = sgqlc.types.Field(StringFieldComparison, graphql_name='id')
     old_billing_id = sgqlc.types.Field(StringFieldComparison, graphql_name='oldBillingId')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionPriceFilterCustomerSubscriptionFilter')), graphql_name='or')
     pricing_type = sgqlc.types.Field(PricingTypeFilterComparison, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(StringFieldComparison, graphql_name='refId')
-    resource_id = sgqlc.types.Field(StringFieldComparison, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateFieldComparison, graphql_name='startDate')
     status = sgqlc.types.Field('SubscriptionStatusFilterComparison', graphql_name='status')
     subscription_id = sgqlc.types.Field(StringFieldComparison, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateFieldComparison, graphql_name='trialEndDate')
 
 
 class SubscriptionPriceFilterPriceFilter(sgqlc.types.Input):
@@ -3013,15 +2881,15 @@
     h3 = sgqlc.types.Field(FontVariantInput, graphql_name='h3')
 
 
 class UpdateAccountInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('display_name', 'id', 'subscription_billing_anchor', 'subscription_proration_behavior', 'timezone')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
-    id = sgqlc.types.Field(String, graphql_name='id')
+    id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     subscription_billing_anchor = sgqlc.types.Field(BillingAnchor, graphql_name='subscriptionBillingAnchor')
     subscription_proration_behavior = sgqlc.types.Field(ProrationBehavior, graphql_name='subscriptionProrationBehavior')
     timezone = sgqlc.types.Field(String, graphql_name='timezone')
 
 
 class UpdateCouponInput(sgqlc.types.Input):
     __schema__ = schema
@@ -3186,18 +3054,17 @@
     reset_period = sgqlc.types.Field(EntitlementResetPeriod, graphql_name='resetPeriod')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
     weekly_reset_period_configuration = sgqlc.types.Field('WeeklyResetPeriodConfigInput', graphql_name='weeklyResetPeriodConfiguration')
 
 
 class UpdateSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'billable_features', 'billing_period', 'environment_id', 'promotion_code', 'ref_id', 'subscription_entitlements', 'subscription_id', 'trial_end_date', 'unit_quantity')
+    __field_names__ = ('additional_meta_data', 'addons', 'billing_period', 'environment_id', 'promotion_code', 'ref_id', 'subscription_entitlements', 'subscription_id', 'trial_end_date', 'unit_quantity')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(SubscriptionAddonInput)), graphql_name='addons')
-    billable_features = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(BillableFeatureInput)), graphql_name='billableFeatures')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     subscription_entitlements = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(UpdateSubscriptionEntitlementInput)), graphql_name='subscriptionEntitlements')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
@@ -3207,32 +3074,14 @@
 class UpdateUserInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('department', 'name')
     department = sgqlc.types.Field(Department, graphql_name='department')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
 
 
-class UsageEventReportInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('customer_id', 'dimensions', 'event_name', 'idempotency_key', 'resource_id', 'timestamp')
-    customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
-    dimensions = sgqlc.types.Field(JSON, graphql_name='dimensions')
-    event_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='eventName')
-    idempotency_key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='idempotencyKey')
-    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
-    timestamp = sgqlc.types.Field(DateTime, graphql_name='timestamp')
-
-
-class UsageEventsReportInput(sgqlc.types.Input):
-    __schema__ = schema
-    __field_names__ = ('environment_id', 'usage_events')
-    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
-    usage_events = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(UsageEventReportInput))), graphql_name='usageEvents')
-
-
 class UsageHistoryInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('customer_ref_id', 'end_date', 'environment_id', 'feature_ref_id', 'monthly_reset_period_configuration', 'reset_period', 'resource_ref_id', 'start_date', 'weekly_reset_period_configuration')
     customer_ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerRefId')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     feature_ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureRefId')
@@ -3537,21 +3386,14 @@
 
 class AddonSumAggregate(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('version_number',)
     version_number = sgqlc.types.Field(Float, graphql_name='versionNumber')
 
 
-class Aggregation(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('field', 'function')
-    field = sgqlc.types.Field(String, graphql_name='field')
-    function = sgqlc.types.Field(sgqlc.types.non_null(AggregationFunction), graphql_name='function')
-
-
 class ApiKey(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('id', 'key_type', 'token')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     key_type = sgqlc.types.Field(sgqlc.types.non_null(ApiKeyType), graphql_name='keyType')
     token = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='token')
 
@@ -4082,29 +3924,28 @@
     total_price = sgqlc.types.Field('CustomerSubscriptionTotalPrice', graphql_name='totalPrice')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
     was_in_trial = sgqlc.types.Field(Boolean, graphql_name='wasInTrial')
 
 
 class CustomerSubscriptionAggregateGroupBy(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
-    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
 
 
 class CustomerSubscriptionConnection(sgqlc.types.relay.Connection):
@@ -4113,29 +3954,28 @@
     edges = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('CustomerSubscriptionEdge'))), graphql_name='edges')
     page_info = sgqlc.types.Field(sgqlc.types.non_null('PageInfo'), graphql_name='pageInfo')
     total_count = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalCount')
 
 
 class CustomerSubscriptionCountAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(Int, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(Int, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(Int, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(Int, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(Int, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(Int, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(Int, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(Int, graphql_name='endDate')
     environment_id = sgqlc.types.Field(Int, graphql_name='environmentId')
     id = sgqlc.types.Field(Int, graphql_name='id')
     old_billing_id = sgqlc.types.Field(Int, graphql_name='oldBillingId')
     pricing_type = sgqlc.types.Field(Int, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(Int, graphql_name='refId')
-    resource_id = sgqlc.types.Field(Int, graphql_name='resourceId')
     start_date = sgqlc.types.Field(Int, graphql_name='startDate')
     status = sgqlc.types.Field(Int, graphql_name='status')
     subscription_id = sgqlc.types.Field(Int, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(Int, graphql_name='trialEndDate')
 
 
 class CustomerSubscriptionEdge(sgqlc.types.Type):
@@ -4143,52 +3983,50 @@
     __field_names__ = ('cursor', 'node')
     cursor = sgqlc.types.Field(sgqlc.types.non_null(ConnectionCursor), graphql_name='cursor')
     node = sgqlc.types.Field(sgqlc.types.non_null(CustomerSubscription), graphql_name='node')
 
 
 class CustomerSubscriptionMaxAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
-    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
 
 
 class CustomerSubscriptionMinAggregate(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'resource_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
+    __field_names__ = ('billing_id', 'cancel_reason', 'cancellation_date', 'created_at', 'crm_id', 'crm_link_url', 'effective_end_date', 'end_date', 'environment_id', 'id', 'old_billing_id', 'pricing_type', 'ref_id', 'start_date', 'status', 'subscription_id', 'trial_end_date')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     cancel_reason = sgqlc.types.Field(SubscriptionCancelReason, graphql_name='cancelReason')
     cancellation_date = sgqlc.types.Field(DateTime, graphql_name='cancellationDate')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_id = sgqlc.types.Field(String, graphql_name='crmId')
     crm_link_url = sgqlc.types.Field(String, graphql_name='crmLinkUrl')
     effective_end_date = sgqlc.types.Field(DateTime, graphql_name='effectiveEndDate')
     end_date = sgqlc.types.Field(DateTime, graphql_name='endDate')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
     id = sgqlc.types.Field(String, graphql_name='id')
     old_billing_id = sgqlc.types.Field(String, graphql_name='oldBillingId')
     pricing_type = sgqlc.types.Field(PricingType, graphql_name='pricingType')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
-    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     status = sgqlc.types.Field(SubscriptionStatus, graphql_name='status')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
     trial_end_date = sgqlc.types.Field(DateTime, graphql_name='trialEndDate')
 
 
 class CustomerSubscriptionTotalPrice(sgqlc.types.Type):
@@ -5008,14 +4846,22 @@
 class InvalidSubscriptionStatus(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('code', 'is_validation_error')
     code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
     is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
 
 
+class InvalidUsageValueForIncrementalFeatureError(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('code', 'is_validation_error', 'usage_value')
+    code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
+    is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
+    usage_value = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='usageValue')
+
+
 class Member(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('account', 'created_at', 'cubejs_token', 'email', 'hide_getting_started_page', 'id', 'member_status', 'service_api_key', 'user')
     account = sgqlc.types.Field(sgqlc.types.non_null(Account), graphql_name='account')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     cubejs_token = sgqlc.types.Field(String, graphql_name='cubejsToken')
     email = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='email')
@@ -5086,93 +4932,14 @@
     __schema__ = schema
     __field_names__ = ('failed_invites', 'skipped_invites', 'success_invites')
     failed_invites = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='failedInvites')
     skipped_invites = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='skippedInvites')
     success_invites = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='successInvites')
 
 
-class Meter(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('account', 'aggregation', 'created_at', 'environment', 'environment_id', 'feature', 'filters', 'id', 'updated_at')
-    account = sgqlc.types.Field(Account, graphql_name='account')
-    aggregation = sgqlc.types.Field(sgqlc.types.non_null(Aggregation), graphql_name='aggregation')
-    created_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='createdAt')
-    environment = sgqlc.types.Field(Environment, graphql_name='environment')
-    environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
-    feature = sgqlc.types.Field(sgqlc.types.non_null(Feature), graphql_name='feature')
-    filters = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MeterFilterDefinition'))), graphql_name='filters')
-    id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
-    updated_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='updatedAt')
-
-
-class MeterAggregateGroupBy(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('created_at', 'environment_id', 'id', 'updated_at')
-    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
-    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
-    id = sgqlc.types.Field(String, graphql_name='id')
-    updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
-
-
-class MeterCondition(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('field', 'operation', 'value')
-    field = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='field')
-    operation = sgqlc.types.Field(sgqlc.types.non_null(ConditionOperation), graphql_name='operation')
-    value = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='value')
-
-
-class MeterConnection(sgqlc.types.relay.Connection):
-    __schema__ = schema
-    __field_names__ = ('edges', 'page_info', 'total_count')
-    edges = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MeterEdge'))), graphql_name='edges')
-    page_info = sgqlc.types.Field(sgqlc.types.non_null('PageInfo'), graphql_name='pageInfo')
-    total_count = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='totalCount')
-
-
-class MeterCountAggregate(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('created_at', 'environment_id', 'id', 'updated_at')
-    created_at = sgqlc.types.Field(Int, graphql_name='createdAt')
-    environment_id = sgqlc.types.Field(Int, graphql_name='environmentId')
-    id = sgqlc.types.Field(Int, graphql_name='id')
-    updated_at = sgqlc.types.Field(Int, graphql_name='updatedAt')
-
-
-class MeterEdge(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('cursor', 'node')
-    cursor = sgqlc.types.Field(sgqlc.types.non_null(ConnectionCursor), graphql_name='cursor')
-    node = sgqlc.types.Field(sgqlc.types.non_null(Meter), graphql_name='node')
-
-
-class MeterFilterDefinition(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('conditions',)
-    conditions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MeterCondition))), graphql_name='conditions')
-
-
-class MeterMaxAggregate(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('created_at', 'environment_id', 'id', 'updated_at')
-    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
-    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
-    id = sgqlc.types.Field(String, graphql_name='id')
-    updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
-
-
-class MeterMinAggregate(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('created_at', 'environment_id', 'id', 'updated_at')
-    created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
-    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
-    id = sgqlc.types.Field(String, graphql_name='id')
-    updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
-
-
 class MeteringNotAvailableForFeatureTypeError(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('code', 'feature_type', 'is_validation_error')
     code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
     feature_type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureType')
     is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
 
@@ -5195,15 +4962,15 @@
     __schema__ = schema
     __field_names__ = ('monthly_according_to',)
     monthly_according_to = sgqlc.types.Field(MonthlyAccordingTo, graphql_name='monthlyAccordingTo')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('add_compatible_addons_to_plan', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_meter', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_customer', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_customers_bulk', 'import_one_customer', 'import_subscriptions_bulk', 'init_add_stripe_customer_payment_method', 'initiate_checkout', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'report_event', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
+    __field_names__ = ('add_compatible_addons_to_plan', 'archive_one_coupon', 'archive_plan', 'attach_customer_payment_method', 'cancel_schedule', 'cancel_subscription', 'create_account', 'create_addon_draft', 'create_feature', 'create_many_package_entitlements', 'create_many_promotional_entitlements', 'create_one_addon', 'create_one_coupon', 'create_one_customer', 'create_one_environment', 'create_one_experiment', 'create_one_feature', 'create_one_hook', 'create_one_integration', 'create_one_plan', 'create_one_product', 'create_plan_draft', 'create_subscription', 'create_usage_measurement', 'delete_environment', 'delete_feature', 'delete_one_addon', 'delete_one_customer', 'delete_one_environment', 'delete_one_feature', 'delete_one_hook', 'delete_one_integration', 'delete_one_package_entitlement', 'delete_one_price', 'delete_one_product', 'delete_one_promotional_entitlement', 'estimate_subscription', 'estimate_subscription_update', 'hide_getting_started_page', 'import_customers_bulk', 'import_one_customer', 'import_subscriptions_bulk', 'init_add_stripe_customer_payment_method', 'initiate_checkout', 'invite_members', 'migrate_subscription_to_latest', 'provision_customer', 'provision_sandbox', 'provision_subscription', 'provision_subscription_v2', 'publish_addon', 'publish_plan', 'purge_customer_cache', 'register_member', 'remove_addon_draft', 'remove_base_plan_from_plan', 'remove_compatible_addons_from_plan', 'remove_coupon_from_customer', 'remove_coupon_from_customer_subscription', 'remove_experiment_from_customer', 'remove_experiment_from_customer_subscription', 'remove_member', 'remove_plan_draft', 'report_entitlement_check_requested', 'resend_email_verification', 'resync_integration', 'set_base_plan_on_plan', 'set_compatible_addons_on_plan', 'set_coupon_on_customer', 'set_coupon_on_customer_subscription', 'set_experiment_on_customer', 'set_experiment_on_customer_subscription', 'set_package_pricing', 'set_widget_configuration', 'start_experiment', 'stop_experiment', 'trigger_import_catalog', 'trigger_import_customers', 'update_account', 'update_entitlements_order', 'update_feature', 'update_one_addon', 'update_one_coupon', 'update_one_customer', 'update_one_environment', 'update_one_experiment', 'update_one_feature', 'update_one_hook', 'update_one_integration', 'update_one_package_entitlement', 'update_one_plan', 'update_one_product', 'update_one_promotional_entitlement', 'update_one_subscription', 'update_user')
     add_compatible_addons_to_plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='addCompatibleAddonsToPlan', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(AddCompatibleAddonsToPlanInput), graphql_name='input', default=None)),
 ))
     )
     archive_one_coupon = sgqlc.types.Field(sgqlc.types.non_null(Coupon), graphql_name='archiveOneCoupon', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ArchiveCouponInput), graphql_name='input', default=None)),
 ))
@@ -5272,18 +5039,14 @@
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(CreateOneHookInput), graphql_name='input', default=None)),
 ))
     )
     create_one_integration = sgqlc.types.Field(sgqlc.types.non_null(Integration), graphql_name='createOneIntegration', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(CreateOneIntegrationInput), graphql_name='input', default=None)),
 ))
     )
-    create_one_meter = sgqlc.types.Field(sgqlc.types.non_null(Meter), graphql_name='createOneMeter', args=sgqlc.types.ArgDict((
-        ('input', sgqlc.types.Arg(sgqlc.types.non_null(CreateOneMeterInput), graphql_name='input', default=None)),
-))
-    )
     create_one_plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='createOnePlan', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(PlanCreateInput), graphql_name='input', default=None)),
 ))
     )
     create_one_product = sgqlc.types.Field(sgqlc.types.non_null('Product'), graphql_name='createOneProduct', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(CreateOneProductInput), graphql_name='input', default=None)),
 ))
@@ -5453,18 +5216,14 @@
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(DiscardPackageDraftInput), graphql_name='input', default=None)),
 ))
     )
     report_entitlement_check_requested = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='reportEntitlementCheckRequested', args=sgqlc.types.ArgDict((
         ('entitlement_check_requested', sgqlc.types.Arg(sgqlc.types.non_null(EntitlementCheckRequested), graphql_name='entitlementCheckRequested', default=None)),
 ))
     )
-    report_event = sgqlc.types.Field(String, graphql_name='reportEvent', args=sgqlc.types.ArgDict((
-        ('events', sgqlc.types.Arg(sgqlc.types.non_null(UsageEventsReportInput), graphql_name='events', default=None)),
-))
-    )
     resend_email_verification = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='resendEmailVerification')
     resync_integration = sgqlc.types.Field(sgqlc.types.non_null('ResyncIntegrationResult'), graphql_name='resyncIntegration', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(ResyncIntegrationInput), graphql_name='input', default=None)),
 ))
     )
     set_base_plan_on_plan = sgqlc.types.Field(sgqlc.types.non_null('Plan'), graphql_name='setBasePlanOnPlan', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(SetBasePlanOnPlanInput), graphql_name='input', default=None)),
@@ -5651,26 +5410,25 @@
     updated_at = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='updatedAt')
     updated_by = sgqlc.types.Field(String, graphql_name='updatedBy')
     version = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='version')
 
 
 class PackageEntitlement(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('created_at', 'description', 'display_name_override', 'environment_id', 'feature', 'feature_id', 'has_unlimited_usage', 'hidden_from_widgets', 'id', 'is_custom', 'meter', 'order', 'package', 'package_id', 'reset_period', 'reset_period_configuration', 'updated_at', 'usage_limit')
+    __field_names__ = ('created_at', 'description', 'display_name_override', 'environment_id', 'feature', 'feature_id', 'has_unlimited_usage', 'hidden_from_widgets', 'id', 'is_custom', 'order', 'package', 'package_id', 'reset_period', 'reset_period_configuration', 'updated_at', 'usage_limit')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name_override = sgqlc.types.Field(String, graphql_name='displayNameOverride')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     feature = sgqlc.types.Field(sgqlc.types.non_null(Feature), graphql_name='feature')
     feature_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='featureId')
     has_unlimited_usage = sgqlc.types.Field(Boolean, graphql_name='hasUnlimitedUsage')
     hidden_from_widgets = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(WidgetType)), graphql_name='hiddenFromWidgets')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     is_custom = sgqlc.types.Field(Boolean, graphql_name='isCustom')
-    meter = sgqlc.types.Field(Meter, graphql_name='meter')
     order = sgqlc.types.Field(Float, graphql_name='order')
     package = sgqlc.types.Field(PackageDTO, graphql_name='package')
     package_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='packageId')
     reset_period = sgqlc.types.Field(EntitlementResetPeriod, graphql_name='resetPeriod')
     reset_period_configuration = sgqlc.types.Field('ResetPeriodConfiguration', graphql_name='resetPeriodConfiguration')
     updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
@@ -5789,16 +5547,15 @@
     has_next_page = sgqlc.types.Field(Boolean, graphql_name='hasNextPage')
     has_previous_page = sgqlc.types.Field(Boolean, graphql_name='hasPreviousPage')
     start_cursor = sgqlc.types.Field(ConnectionCursor, graphql_name='startCursor')
 
 
 class Paywall(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('active_subscriptions', 'configuration', 'currency', 'customer', 'plans', 'resource')
-    active_subscriptions = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscription)), graphql_name='activeSubscriptions')
+    __field_names__ = ('configuration', 'currency', 'customer', 'plans', 'resource')
     configuration = sgqlc.types.Field('PaywallConfiguration', graphql_name='configuration')
     currency = sgqlc.types.Field(sgqlc.types.non_null('PaywallCurrency'), graphql_name='currency')
     customer = sgqlc.types.Field(Customer, graphql_name='customer')
     plans = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Plan'))), graphql_name='plans')
     resource = sgqlc.types.Field(CustomerResource, graphql_name='resource')
 
 
@@ -6452,15 +6209,15 @@
     __schema__ = schema
     __field_names__ = ('task_id',)
     task_id = sgqlc.types.Field(String, graphql_name='taskId')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_resources', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_active_subscriptions', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'meter', 'meters', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
+    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_resources', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_active_subscriptions', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
     addons = sgqlc.types.Field(sgqlc.types.non_null(AddonConnection), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(AddonFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(AddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     cached_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement))), graphql_name='cachedEntitlements', args=sgqlc.types.ArgDict((
@@ -6580,24 +6337,14 @@
     )
     members = sgqlc.types.Field(sgqlc.types.non_null(MemberConnection), graphql_name='members', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(MemberFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(MemberSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
-    meter = sgqlc.types.Field(Meter, graphql_name='meter', args=sgqlc.types.ArgDict((
-        ('id', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='id', default=None)),
-))
-    )
-    meters = sgqlc.types.Field(sgqlc.types.non_null(MeterConnection), graphql_name='meters', args=sgqlc.types.ArgDict((
-        ('filter', sgqlc.types.Arg(MeterFilter, graphql_name='filter', default={})),
-        ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
-        ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(MeterSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
-))
-    )
     mock_paywall = sgqlc.types.Field(sgqlc.types.non_null(MockPaywall), graphql_name='mockPaywall', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(GetPaywallInput), graphql_name='input', default=None)),
 ))
     )
     package_entitlements = sgqlc.types.Field(sgqlc.types.non_null(PackageEntitlementConnection), graphql_name='packageEntitlements', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(PackageEntitlementFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
@@ -7021,24 +6768,21 @@
     code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
     is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
     ref_ids = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='refIds')
 
 
 class SubscriptionPreview(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('billing_period_range', 'discount', 'proration', 'sub_total', 'subscription', 'tax', 'tax_details', 'total', 'total_excluding_tax')
+    __field_names__ = ('billing_period_range', 'discount', 'proration', 'sub_total', 'subscription', 'total')
     billing_period_range = sgqlc.types.Field(sgqlc.types.non_null(DateRange), graphql_name='billingPeriodRange')
     discount = sgqlc.types.Field('SubscriptionPreviewDiscountDTO', graphql_name='discount')
     proration = sgqlc.types.Field('SubscriptionPreviewProrations', graphql_name='proration')
     sub_total = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='subTotal')
     subscription = sgqlc.types.Field('SubscriptionPricePreviewDTO', graphql_name='subscription')
-    tax = sgqlc.types.Field(Money, graphql_name='tax')
-    tax_details = sgqlc.types.Field('SubscriptionPreviewTaxDetails', graphql_name='taxDetails')
     total = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='total')
-    total_excluding_tax = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='totalExcludingTax')
 
 
 class SubscriptionPreviewDiscountDTO(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('duration_in_months', 'duration_type', 'type', 'value')
     duration_in_months = sgqlc.types.Field(Float, graphql_name='durationInMonths')
     duration_type = sgqlc.types.Field(sgqlc.types.non_null(DiscountDurationType), graphql_name='durationType')
@@ -7051,22 +6795,14 @@
     __field_names__ = ('credit', 'debit', 'net_amount', 'proration_date')
     credit = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='credit')
     debit = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='debit')
     net_amount = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='netAmount')
     proration_date = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='prorationDate')
 
 
-class SubscriptionPreviewTaxDetails(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('display_name', 'inclusive', 'percentage')
-    display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
-    inclusive = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='inclusive')
-    percentage = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='percentage')
-
-
 class SubscriptionPrice(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('created_at', 'id', 'price', 'subscription', 'updated_at', 'usage_limit')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     price = sgqlc.types.Field(Price, graphql_name='price')
     subscription = sgqlc.types.Field(sgqlc.types.non_null(CustomerSubscription), graphql_name='subscription')
@@ -7121,19 +6857,17 @@
     id = sgqlc.types.Field(String, graphql_name='id')
     updated_at = sgqlc.types.Field(DateTime, graphql_name='updatedAt')
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
 
 
 class SubscriptionPricePreviewDTO(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('sub_total', 'tax', 'total', 'total_excluding_tax')
+    __field_names__ = ('sub_total', 'total')
     sub_total = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='subTotal')
-    tax = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='tax')
     total = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='total')
-    total_excluding_tax = sgqlc.types.Field(sgqlc.types.non_null(Money), graphql_name='totalExcludingTax')
 
 
 class SubscriptionPriceSumAggregate(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('usage_limit',)
     usage_limit = sgqlc.types.Field(Float, graphql_name='usageLimit')
 
@@ -7223,16 +6957,15 @@
     is_validation_error = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isValidationError')
     non_compatible_addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='nonCompatibleAddons')
     plan_display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planDisplayName')
 
 
 class UnitAmountChangeVariables(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('feature_id', 'new_unit_amount')
-    feature_id = sgqlc.types.Field(String, graphql_name='featureId')
+    __field_names__ = ('new_unit_amount',)
     new_unit_amount = sgqlc.types.Field(Float, graphql_name='newUnitAmount')
 
 
 class UnsupportedFeatureTypeError(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('code', 'feature_type')
     code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='code')
```

### Comparing `stigg_api_client-0.458.4/PKG-INFO` & `stigg_api_client-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.458.4
+Version: 0.5.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: graphql-core (>=3.1,<4.0)
-Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: black (>=22.8.0,<23.0.0)
+Requires-Dist: flake8 (>=5.0.4,<6.0.0)
+Requires-Dist: graphql-core (==3.1.6)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sgqlc (>=16.0,<17.0)
 Description-Content-Type: text/markdown
 
 # stigg-api-client
 
 This library provides a Python wrapper to [Stigg's GraphQL API](https://docs.stigg.io/docs/graphql-api) based on 
 the operations that are in use by the [Stigg's Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).
```

