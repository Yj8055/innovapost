# innovapost

apiVersion: operators.coreos.com/v1alpha1
kind: CatalogSource
metadata:
  name: ibm-integration-platform-navigator-catalog
  namespace: openshift-marketplace
spec:
  displayName: ibm-integration-platform-navigator-7.3.1
  publisher: IBM
  image: icr.io/cpopen/ibm-integration-platform-navigator-catalog@sha256:378dab19dd98753b37b450cbbc14cc9494f88d4ad8b0b790126066051845bd7a
  sourceType: grpc
  updateStrategy:
    registryPoll:
      interval: 30m0s


apiVersion: operators.coreos.com/v1alpha1
kind: CatalogSource
metadata:
  name: opencloud-operators
  namespace: openshift-marketplace
spec:
  displayName: ibm-cp-common-services-4.6.4
  publisher: IBM
  image: icr.io/cpopen/ibm-common-service-catalog@sha256:9d00de6ec33a429cf9eb621461b9fd428522d626905658d32e294e031990aa9b
  sourceType: grpc
  updateStrategy:
    registryPoll:
      interval: 30m0s


apiVersion: operators.coreos.com/v1alpha1
kind: CatalogSource
metadata:
  name: appconnect-operator-catalogsource
  namespace: openshift-marketplace
spec:
  displayName: ibm-appconnect-12.0.2
  publisher: IBM
  image: icr.io/cpopen/appconnect-operator-catalog@sha256:ea636e5466f10b3dfb1585190a75fd0995961c7482db8e6a1aad8cbfaf09cecb
  sourceType: grpc
  updateStrategy:
    registryPoll:
      interval: 30m0s
