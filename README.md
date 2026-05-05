# ncr-gitops
'''
bsp-sre-gitops/
├── apps
│   ├── ASM
│   │   ├── business-services-platform
│   │   │   ├── APAC
│   │   │   │   └── production
│   │   │   │       ├── gateway-patch.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   ├── EMEA
│   │   │   │   └── production
│   │   │   │       ├── gateway-patch.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   ├── NAMER
│   │   │   │   ├── development
│   │   │   │   │   ├── gateway-patch.yaml
│   │   │   │   │   └── kustomization.yaml
│   │   │   │   ├── production
│   │   │   │   │   ├── gateway-patch.yaml
│   │   │   │   │   └── kustomization.yaml
│   │   │   │   └── staging
│   │   │   │       ├── gateway-patch.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   └── NAPAC
│   │   │       └── production
│   │   │           ├── gateway-patch.yaml
│   │   │           └── kustomization.yaml
│   │   ├── messaging
│   │   │   ├── APAC
│   │   │   │   └── prod
│   │   │   │       ├── gateway.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   ├── EMEA
│   │   │   │   └── prod
│   │   │   │       ├── gateway.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   ├── NAPAC
│   │   │   │   └── prod
│   │   │   │       ├── gateway.yaml
│   │   │   │       └── kustomization.yaml
│   │   │   └── US
│   │   │       ├── dev
│   │   │       │   ├── cnm-600.yaml
│   │   │       │   ├── core-test-509.yaml
│   │   │       │   ├── gateway.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── test-asm-507-test.yaml
│   │   │       │   ├── test-asm-600.yaml
│   │   │       │   ├── test-asm-601.yaml
│   │   │       │   └── test-asm-beta.yaml
│   │   │       ├── prod
│   │   │       │   ├── gateway.yaml
│   │   │       │   └── kustomization.yaml
│   │   │       └── stg
│   │   │           ├── core-beta.yaml
│   │   │           ├── gateway.yaml
│   │   │           ├── kustomization.yaml
│   │   │           └── test-asm-600.yaml
│   │   └── technical-services
│   │       └── NAMER
│   │           ├── development
│   │           │   ├── core-namer-dev
│   │           │   │   ├── core-user.yaml
│   │           │   │   ├── core.yaml
│   │           │   │   ├── kustomization.yaml
│   │           │   │   ├── namespace.yaml
│   │           │   │   └── platform-client-es.yaml
│   │           │   ├── core-namer-sandbox
│   │           │   │   ├── core-user.yaml
│   │           │   │   ├── core.yaml
│   │           │   │   ├── kustomization.yaml
│   │           │   │   ├── namespace.yaml
│   │           │   │   └── platform-client-es.yaml
│   │           │   ├── dev-apims
│   │           │   │   ├── analytics.yaml
│   │           │   │   ├── api-launch.yaml
│   │           │   │   ├── auditing.yaml
│   │           │   │   ├── bsp-security-proxy.yaml
│   │           │   │   ├── entitlements.yaml
│   │           │   │   ├── export-data.yaml
│   │           │   │   ├── kustomization.yaml
│   │           │   │   ├── namespace.yaml
│   │           │   │   ├── simulator.yaml
│   │           │   │   └── teams.yaml
│   │           │   ├── gateway-patch.yaml
│   │           │   ├── kustomization.yaml
│   │           │   └── rc-dev-apims
│   │           │       ├── api-launch.yaml
│   │           │       ├── kustomization.yaml
│   │           │       └── namespace.yaml
│   │           └── staging
│   │               └── kustomization.yaml
│   ├── bsp-sretools
│   │   └── bsp-sretools-cluster
│   │       ├── pe-ncrvoyix-site
│   │       ├── sre-gcpquotas
│   │       └── sre-ncrbot
│   ├── bsp-sretools-cug01-stg
│   │   └── bsp-sretools-stg-cluster
│   │       ├── argus
│   │       │   ├── helm-release.yaml
│   │       │   └── kustomization.yaml
│   │       ├── github-notifier
│   │       │   ├── github-notifier.yaml
│   │       │   └── kustomization.yaml
│   │       ├── kustomization.yaml
│   │       ├── pe-ncrvoyix-site
│   │       │   ├── helm-release.yaml
│   │       │   ├── kustomization.yaml
│   │       │   └── namespace.yaml
│   │       ├── sre-gcpquotas
│   │       │   ├── kustomization.yaml
│   │       │   └── sre-gcpquotas.yaml
│   │       └── sre-ncrbot
│   │           ├── kustomization.yaml
│   │           └── sre-ncrbot.yaml
│   ├── business-services-platform
│   │   ├── APAC
│   │   │   └── production
│   │   │       ├── cnm
│   │   │       │   ├── cdm.yaml
│   │   │       │   ├── digitalcoupon
│   │   │       │   │   ├── digitalcoupon.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── digitalreceipt
│   │   │       │   │   ├── digitalreceipt.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── flux-kustomize
│   │   │       │   │   ├── digitalcoupon-kustomize.yaml
│   │   │       │   │   ├── digitalreceipt-kustomize.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── git-repo.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── namespace.yaml
│   │   │       │   ├── promotion-execution-mock-adapter.yaml
│   │   │       │   ├── promotion-execution.yaml
│   │   │       │   ├── pubsub-processor.yaml
│   │   │       │   ├── segment.yaml
│   │   │       │   └── stored-value
│   │   │       │       ├── kustomization.yaml
│   │   │       │       ├── stored-value-partner.yaml
│   │   │       │       └── stored-value.yaml
│   │   │       ├── data
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── namespace.yaml
│   │   │       │   ├── tdm-billing.yaml
│   │   │       │   ├── tdm-count.yaml
│   │   │       │   ├── tdm-expiration-processor.yaml
│   │   │       │   ├── tdm-export.yaml
│   │   │       │   └── tdm.yaml
│   │   │       ├── items
│   │   │       │   ├── catalog-batch.yaml
│   │   │       │   ├── catalog.yaml
│   │   │       │   ├── gke-management
│   │   │       │   │   ├── kustomization.yaml
│   │   │       │   │   ├── secrets-management-role-binding.yaml
│   │   │       │   │   └── serviceaccount-clusterrolebinding.yaml
│   │   │       │   ├── image.yaml
│   │   │       │   ├── item-availability.yaml
│   │   │       │   ├── items-storage.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── menu-maker.yaml
│   │   │       │   ├── menu-v1.yaml
│   │   │       │   ├── menu.yaml
│   │   │       │   ├── modifier-codes.yaml
│   │   │       │   └── namespace.yaml
│   │   │       ├── items-ingest
│   │   │       │   ├── items-ingest-user.yaml
│   │   │       │   ├── items-ingest.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   └── namespace.yaml
│   │   │       ├── kustomization.yaml
│   │   │       └── ordering
│   │   │           ├── delivery-doordash-expiration-processor.yaml
│   │   │           ├── delivery-doordash.yaml
│   │   │           ├── delivery-expiration-processor.yaml
│   │   │           ├── delivery-mock.yaml
│   │   │           ├── delivery.yaml
│   │   │           ├── fulfillment-time.yaml
│   │   │           ├── kustomization.yaml
│   │   │           ├── namespace.yaml
│   │   │           ├── order-billing.yaml
│   │   │           ├── order-expiration-processor.yaml
│   │   │           ├── order-history.yaml
│   │   │           ├── order-monitor.yaml
│   │   │           ├── order-support-ui.yaml
│   │   │           ├── order.yaml
│   │   │           └── site.yaml
│   │   ├── EMEA
│   │   │   └── production
│   │   │       ├── cnm
│   │   │       │   ├── cdm.yaml
│   │   │       │   ├── digitalcoupon
│   │   │       │   │   ├── digitalcoupon.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── digitalreceipt
│   │   │       │   │   ├── digitalreceipt.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── flux-kustomize
│   │   │       │   │   ├── digitalcoupon-kustomize.yaml
│   │   │       │   │   ├── digitalreceipt-kustomize.yaml
│   │   │       │   │   └── kustomization.yaml
│   │   │       │   ├── git-repo.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── namespace.yaml
│   │   │       │   ├── promotion-execution-mock-adapter.yaml
│   │   │       │   ├── promotion-execution.yaml
│   │   │       │   ├── pubsub-processor.yaml
│   │   │       │   ├── segment.yaml
│   │   │       │   └── stored-value
│   │   │       │       ├── kustomization.yaml
│   │   │       │       ├── stored-value-partner.yaml
│   │   │       │       └── stored-value.yaml
│   │   │       ├── data
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── namespace.yaml
│   │   │       │   ├── tdm-billing.yaml
│   │   │       │   ├── tdm-count.yaml
│   │   │       │   ├── tdm-expiration-processor.yaml
│   │   │       │   ├── tdm-export.yaml
│   │   │       │   └── tdm.yaml
│   │   │       ├── items
│   │   │       │   ├── catalog-batch.yaml
│   │   │       │   ├── catalog.yaml
│   │   │       │   ├── gke-management
│   │   │       │   │   ├── kustomization.yaml
│   │   │       │   │   ├── secrets-management-role-binding.yaml
│   │   │       │   │   └── serviceaccount-clusterrolebinding.yaml
│   │   │       │   ├── image.yaml
│   │   │       │   ├── item-availability.yaml
│   │   │       │   ├── items-storage.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   ├── menu-maker.yaml
│   │   │       │   ├── menu-v1.yaml
│   │   │       │   ├── menu.yaml
│   │   │       │   ├── modifier-codes.yaml
│   │   │       │   └── namespace.yaml
│   │   │       ├── items-ingest
│   │   │       │   ├── items-ingest-user.yaml
│   │   │       │   ├── items-ingest.yaml
│   │   │       │   ├── kustomization.yaml
│   │   │       │   └── namespace.yaml
│   │   │       ├── kustomization.yaml
│   │   │       └── ordering
│   │   │           ├── delivery-doordash-expiration-processor.yaml
│   │   │           ├── delivery-doordash.yaml
│   │   │           ├── delivery-expiration-processor.yaml
│   │   │           ├── delivery-mock.yaml
│   │   │           ├── delivery.yaml
│   │   │           ├── fulfillment-time.yaml
│   │   │           ├── kustomization.yaml
│   │   │           ├── namespace.yaml
│   │   │           ├── order-billing.yaml
│   │   │           ├── order-expiration-processor.yaml
│   │   │           ├── order-history.yaml
│   │   │           ├── order-monitor.yaml
│   │   │           ├── order-support-ui.yaml
│   │   │           ├── order.yaml
│   │   │           └── site.yaml
│   │   ├── NAMER
│   │   │   ├── development
│   │   │   │   ├── cnm
│   │   │   │   │   ├── digitalcoupon
│   │   │   │   │   ├── digitalreceipt
│   │   │   │   │   ├── flux-kustomize
│   │   │   │   │   └── stored-value
│   │   │   │   ├── data
│   │   │   │   ├── github-notifier
│   │   │   │   ├── items
│   │   │   │   │   └── gke-management
│   │   │   │   ├── items-ingest
│   │   │   │   ├── ordering
│   │   │   │   ├── ordering-apigee
│   │   │   │   └── simple-app-java
│   │   │   ├── production
│   │   │   │   ├── cnm
│   │   │   │   │   ├── digitalcoupon
│   │   │   │   │   ├── digitalreceipt
│   │   │   │   │   ├── flux-kustomize
│   │   │   │   │   └── stored-value
│   │   │   │   ├── data
│   │   │   │   ├── items
│   │   │   │   │   └── gke-management
│   │   │   │   ├── items-ingest
│   │   │   │   └── ordering
│   │   │   └── staging
│   │   │       ├── cnm
│   │   │       │   ├── digitalcoupon
│   │   │       │   ├── digitalreceipt
│   │   │       │   ├── flux-kustomize
│   │   │       │   └── stored-value
│   │   │       ├── data
│   │   │       ├── items
│   │   │       │   └── gke-management
│   │   │       ├── items-ingest
│   │   │       └── ordering
│   │   └── NAPAC
│   │       └── production
│   │           ├── cnm
│   │           │   ├── digitalcoupon
│   │           │   ├── digitalreceipt
│   │           │   ├── flux-kustomize
│   │           │   └── stored-value
│   │           ├── data
│   │           │   ├── kustomization.yaml
│   │           │   ├── namespace.yaml
│   │           │   ├── tdm-billing.yaml
│   │           │   ├── tdm-count.yaml
│   │           │   ├── tdm-expiration-processor.yaml
│   │           │   ├── tdm-export.yaml
│   │           │   └── tdm.yaml
│   │           ├── items
│   │           │   ├── catalog-batch.yaml
│   │           │   ├── catalog.yaml
│   │           │   ├── gke-management
│   │           │   ├── image.yaml
│   │           │   ├── items-storage.yaml
│   │           │   ├── kustomization.yaml
│   │           │   ├── menu-maker.yaml
│   │           │   ├── menu.yaml
│   │           │   ├── modifier-codes.yaml
│   │           │   └── namespace.yaml
│   │           ├── items-ingest
│   │           ├── kustomization.yaml
│   │           └── ordering
│   ├── devex
│   │   ├── APAC
│   │   │   └── production
│   │   │       └── ocpx
│   │   ├── EMEA
│   │   │   └── production
│   │   │       └── ocpx
│   │   ├── NAMER
│   │   │   ├── development
│   │   │   │   ├── home
│   │   │   │   ├── home-public-api
│   │   │   │   ├── ocpx
│   │   │   │   └── react-common-components-reference-app
│   │   │   ├── production
│   │   │   │   ├── home
│   │   │   │   └── ocpx
│   │   │   ├── production-fedramp
│   │   │   │   └── ocpx
│   │   │   ├── staging
│   │   │   │   ├── home
│   │   │   │   ├── ncr-retail-demo
│   │   │   │   ├── ocpx
│   │   │   │   ├── react-common-components-reference-app
│   │   │   │   └── sample-app-burgers
│   │   │   └── staging-fedramp
│   │   │       └── ocpx
│   │   └── NAPAC
│   │       └── production
│   │           └── ocpx
│   └── technical-services
│       ├── APAC
│       │   └── production
│       │       ├── applications-apac-prd
│       │       │   ├── applications.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── core-apac-prd
│       │       │   ├── core-user.yaml
│       │       │   ├── core.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── flagger
│       │       │   ├── HelmRelease.yaml
│       │       │   └── kustomization.yaml
│       │       ├── journaling-apac-prd
│       │       │   ├── journaling-user.yaml
│       │       │   ├── journaling.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── kustomization.yaml
│       │       ├── messaging-health-monitor-apac-prd
│       │       │   ├── kustomization.yaml
│       │       │   ├── mhm.yaml
│       │       │   └── namespace.yaml
│       │       ├── notifications-apac-prd
│       │       │   ├── kustomization.yaml
│       │       │   ├── message-ingest.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── notifications.yaml
│       │       ├── prd-apims
│       │       │   ├── analytics.yaml
│       │       │   ├── api-launch.yaml
│       │       │   ├── auditing.yaml
│       │       │   ├── bsp-security-proxy.yaml
│       │       │   ├── entitlements.yaml
│       │       │   ├── export-data.yaml
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   ├── simulator.yaml
│       │       │   └── teams.yaml
│       │       └── users-apac-prd
│       │           ├── kustomization.yaml
│       │           ├── namespace.yaml
│       │           └── users.yaml
│       ├── EMEA
│       │   └── production
│       │       ├── applications-emea-prd
│       │       │   ├── applications.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── core-emea-prd
│       │       │   ├── core-user.yaml
│       │       │   ├── core.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── flagger
│       │       │   ├── HelmRelease.yaml
│       │       │   └── kustomization.yaml
│       │       ├── journaling-emea-prd
│       │       │   ├── journaling-user.yaml
│       │       │   ├── journaling.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── kustomization.yaml
│       │       ├── messaging-health-monitor-emea-prd
│       │       │   ├── kustomization.yaml
│       │       │   ├── mhm.yaml
│       │       │   └── namespace.yaml
│       │       ├── notifications-emea-prd
│       │       │   ├── kustomization.yaml
│       │       │   ├── message-ingest.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── notifications.yaml
│       │       ├── prd-apims
│       │       │   ├── analytics.yaml
│       │       │   ├── api-launch.yaml
│       │       │   ├── auditing.yaml
│       │       │   ├── bsp-security-proxy.yaml
│       │       │   ├── entitlements.yaml
│       │       │   ├── export-data.yaml
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   ├── simulator.yaml
│       │       │   └── teams.yaml
│       │       └── users-emea-prd
│       │           ├── kustomization.yaml
│       │           ├── namespace.yaml
│       │           └── users.yaml
│       ├── NAMER
│       │   ├── development
│       │   │   ├── applications-namer-dev
│       │   │   │   ├── applications.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── applications-namer-sandbox
│       │   │   │   ├── applications.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── core-namer-dev
│       │   │   │   ├── core-user.yaml
│       │   │   │   ├── core.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── platform-client-es.yaml
│       │   │   ├── core-namer-sandbox
│       │   │   │   ├── core-user.yaml
│       │   │   │   ├── core.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── platform-client-es.yaml
│       │   │   ├── dev-apims
│       │   │   │   ├── analytics.yaml
│       │   │   │   ├── api-launch.yaml
│       │   │   │   ├── auditing.yaml
│       │   │   │   ├── bsp-security-proxy.yaml
│       │   │   │   ├── entitlements.yaml
│       │   │   │   ├── export-data.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   ├── simulator.yaml
│       │   │   │   └── teams.yaml
│       │   │   ├── dev-apims-gitops
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── flagger
│       │   │   │   ├── HelmRelease.yaml
│       │   │   │   └── kustomization.yaml
│       │   │   ├── gateway.yaml
│       │   │   ├── github-notifier
│       │   │   │   ├── github-notifier.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── journaling-namer-dev
│       │   │   │   ├── journaling-user.yaml
│       │   │   │   ├── journaling.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── journaling-namer-sandbox
│       │   │   │   ├── journaling-user.yaml
│       │   │   │   ├── journaling.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── kustomization.yaml
│       │   │   ├── messaging-health-monitor-namer-dev
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── mhm.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── messaging-health-monitor-namer-sandbox
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── mhm.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── ncr-id
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── ncr-id.yaml
│       │   │   ├── ncr-id-test
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── ncr-id.yaml
│       │   │   ├── notifications-namer-dev
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── message-ingest.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── notifications.yaml
│       │   │   ├── notifications-namer-sandbox
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── message-ingest.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── notifications.yaml
│       │   │   ├── rc-dev-apims
│       │   │   │   ├── api-launch-v2.yaml
│       │   │   │   ├── api-launch.yaml
│       │   │   │   ├── bsp-security-proxy.yaml
│       │   │   │   ├── entitlements.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── site-security-namer-dev
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── site-security.yaml
│       │   │   ├── site-security-namer-sandbox
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── site-security.yaml
│       │   │   ├── users-namer-dev
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── users.yaml
│       │   │   └── users-namer-sandbox
│       │   │       ├── kustomization.yaml
│       │   │       ├── namespace.yaml
│       │   │       └── users.yaml
│       │   ├── production
│       │   │   ├── applications-namer-prd
│       │   │   │   ├── applications.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── core-namer-prd
│       │   │   │   ├── core-user.yaml
│       │   │   │   ├── core.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── dev-apims
│       │   │   │   ├── bsp-security-proxy.yaml
│       │   │   │   ├── entitlements.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   ├── simulator.yaml
│       │   │   │   └── teams.yaml
│       │   │   ├── flagger
│       │   │   │   ├── HelmRelease.yaml
│       │   │   │   └── kustomization.yaml
│       │   │   ├── gateway.yaml
│       │   │   ├── journaling-namer-prd
│       │   │   │   ├── journaling-user.yaml
│       │   │   │   ├── journaling.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── platform-client-es.yaml
│       │   │   ├── kustomization.yaml
│       │   │   ├── messaging-health-monitor-namer-prd
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── mhm.yaml
│       │   │   │   └── namespace.yaml
│       │   │   ├── ncr-id
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── ncr-id.yaml
│       │   │   ├── notifications-namer-prd
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── message-ingest.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   └── notifications.yaml
│       │   │   ├── prd-apims
│       │   │   │   ├── analytics.yaml
│       │   │   │   ├── api-launch.yaml
│       │   │   │   ├── auditing.yaml
│       │   │   │   ├── bsp-security-proxy.yaml
│       │   │   │   ├── entitlements.yaml
│       │   │   │   ├── export-data.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   ├── simulator.yaml
│       │   │   │   └── teams.yaml
│       │   │   ├── stg-apims
│       │   │   │   ├── bsp-security-proxy.yaml
│       │   │   │   ├── entitlements.yaml
│       │   │   │   ├── kustomization.yaml
│       │   │   │   ├── namespace.yaml
│       │   │   │   ├── simulator.yaml
│       │   │   │   └── teams.yaml
│       │   │   └── users-namer-prd
│       │   │       ├── kustomization.yaml
│       │   │       ├── namespace.yaml
│       │   │       └── users.yaml
│       │   └── staging
│       │       ├── applications-namer-stg
│       │       │   ├── applications.yaml
│       │       │   ├── kustomization.yaml
│       │       │   └── namespace.yaml
│       │       ├── core-namer-stg
│       │       │   ├── core-user.yaml
│       │       │   ├── core.yaml
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── platform-client-es.yaml
│       │       ├── flagger
│       │       │   ├── HelmRelease.yaml
│       │       │   └── kustomization.yaml
│       │       ├── gateway.yaml
│       │       ├── journaling-namer-stg
│       │       │   ├── journaling-user.yaml
│       │       │   ├── journaling.yaml
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── platform-client-es.yaml
│       │       ├── kustomization.yaml
│       │       ├── messaging-health-monitor-namer-stg
│       │       │   ├── kustomization.yaml
│       │       │   ├── mhm.yaml
│       │       │   └── namespace.yaml
│       │       ├── ncr-id
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── ncr-id.yaml
│       │       ├── notifications-namer-stg
│       │       │   ├── kustomization.yaml
│       │       │   ├── message-ingest.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── notifications.yaml
│       │       ├── site-security-namer-stg
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── site-security.yaml
│       │       ├── stg-apims
│       │       │   ├── analytics.yaml
│       │       │   ├── api-launch.yaml
│       │       │   ├── auditing.yaml
│       │       │   ├── bsp-security-proxy.yaml
│       │       │   ├── entitlements.yaml
│       │       │   ├── kustomization.yaml
│       │       │   ├── namespace.yaml
│       │       │   └── simulator.yaml
│       │       └── users-namer-stg
│       │           ├── kustomization.yaml
│       │           ├── namespace.yaml
│       │           └── users.yaml
│       └── NAPAC
│           └── production
│               ├── applications-napac-prd
│               │   ├── applications.yaml
│               │   ├── kustomization.yaml
│               │   └── namespace.yaml
│               ├── core-napac-prd
│               │   ├── core-user.yaml
│               │   ├── core.yaml
│               │   ├── kustomization.yaml
│               │   └── namespace.yaml
│               ├── flagger
│               │   ├── HelmRelease.yaml
│               │   └── kustomization.yaml
│               ├── journaling-napac-prd
│               │   ├── journaling-user.yaml
│               │   ├── journaling.yaml
│               │   ├── kustomization.yaml
│               │   └── namespace.yaml
│               ├── kustomization.yaml
│               ├── messaging-health-monitor-napac-prd
│               │   ├── kustomization.yaml
│               │   ├── mhm.yaml
│               │   └── namespace.yaml
│               ├── notifications-napac-prd
│               │   ├── kustomization.yaml
│               │   ├── message-ingest.yaml
│               │   ├── namespace.yaml
│               │   └── notifications.yaml
│               ├── prd-apims
│               │   ├── analytics.yaml
│               │   ├── api-launch.yaml
│               │   ├── auditing.yaml
│               │   ├── bsp-security-proxy.yaml
│               │   ├── entitlements.yaml
│               │   ├── export-data.yaml
│               │   ├── kustomization.yaml
│               │   ├── namespace.yaml
│               │   ├── simulator.yaml
│               │   └── teams.yaml
│               └── users-napac-prd
│                   ├── kustomization.yaml
│                   ├── namespace.yaml
│                   └── users.yaml
├── clusters
│   ├── bsp-bservices-sag01-prod
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── bsp-devex-sag01-prod
│   │   └── devex-prod-napac
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── bsp-sretools
│   │   └── bsp-sretools-cluster
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── bsp-sretools-cug01-stg
│   │   └── bsp-sretools-stg-cluster
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── bsp-technicalsrvc-sag01-prod
│   │   └── technical-services
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           ├── external-secret-operator-sa
│   │           └── github-notifier
│   ├── business-services-platform-dev
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── business-services-platform-prd
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── business-services-platform-stg
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── business-services-prd-apac
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── business-services-prd-emea
│   │   ├── bsp-messaging-asm
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── business-services-platform
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   └── business-services-platform-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-metrics
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-dev
│   │   └── devex-dev-apigee
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-nonprod
│   │   └── devex-staging
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-nonprod-fedramp
│   │   └── devex-staging-fedramp
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-prod
│   │   └── devex-prod
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-prod-apac
│   │   └── devex-prod-apac
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-prod-emea
│   │   └── devex-prod-emea
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── devex-prod-fedramp
│   │   └── devex-prod-fedramp
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           └── external-secret-operator-sa
│   ├── technical-services-dev
│   │   ├── messaging-test
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-secret-operator-css
│   │   │       └── external-secret-operator-sa
│   │   ├── technical-services
│   │   │   ├── base
│   │   │   ├── flux-system
│   │   │   └── overlays
│   │   │       ├── external-metrics
│   │   │       ├── external-secret-operator-css
│   │   │       ├── external-secret-operator-sa
│   │   │       └── github-notifier
│   │   └── technical-services-asm
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           ├── external-secret-operator-sa
│   │           └── github-notifier
│   ├── technical-services-prd
│   │   └── technical-services
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           ├── external-secret-operator-sa
│   │           └── github-notifier
│   ├── technical-services-prd-apac
│   │   └── technical-services
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           ├── external-secret-operator-sa
│   │           └── github-notifier
│   ├── technical-services-prd-emea
│   │   └── technical-services
│   │       ├── base
│   │       ├── flux-system
│   │       └── overlays
│   │           ├── external-secret-operator-css
│   │           ├── external-secret-operator-sa
│   │           └── github-notifier
│   └── technical-services-stg
│       ├── technical-services
│       │   ├── base
│       │   ├── flux-system
│       │   └── overlays
│       │       ├── external-metrics
│       │       ├── external-secret-operator-css
│       │       ├── external-secret-operator-sa
│       │       └── github-notifier
│       └── technical-services-asm
│           ├── base
│           ├── flux-system
│           └── overlays
│               ├── external-secret-operator-css
│               ├── external-secret-operator-sa
│               └── github-notifier
├── CODEOWNERS
├── common-resources
│   ├── default
│   │   ├── asm
│   │   │   └── mtls-strict
│   │   ├── certs
│   │   │   ├── developer-cert
│   │   │   ├── developer-voyix-cert
│   │   │   ├── ncrcloud
│   │   │   └── notifications-api-ncr
│   │   ├── gateway
│   │   ├── github
│   │   └── slack
│   └── gke-management
│       ├── backend-config
│       ├── default-service-account
│       │   ├── cluster-role
│       │   └── secrets-management
│       └── frontend-config
├── infrastructure
│   ├── carbon-black-cloud
│   │   ├── agent
│   │   └── operator
│   ├── clamav
│   ├── core
│   ├── crowdstrike
│   ├── dynatrace
│   │   ├── agent
│   │   └── operator
│   ├── external-metrics
│   ├── external-secret-operator
│   │   ├── crd
│   │   ├── css
│   │   └── serviceAccount
│   ├── externalSecrets
│   ├── flagger
│   ├── flux-dashboard
│   ├── github-action-runner
│   │   ├── gha-runner-scale-set
│   │   └── openebs
│   ├── github-notifier
│   ├── github-notifier-emu
│   └── istio-ingress-gateway
│       ├── certs
│       └── envoy-jwt-extraction
└── renovate.json
'''
