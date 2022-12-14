+++
title = "Changelog"
description = "Kubeflow on GCP Changelog"
weight = 300
+++

## 1.6.1

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.6.1)

### Changes:

- ๐ผ Upgraded upstream Manifests to v1.6.1.
- ๐ผ Upgraded pipelines to v 2.0.0-alpha.6 (fixes #392).
- ๐ผ Updated MySQL to 8.0 (#391).
- ๐จ Fixed ASM deployment issue (#389)
- ๐จ Minor improvements of deployment process.
- ๐งช Validated deployment using GKE 1.22.

## 1.6.0:

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.6.0)

### Changes:

- ๐ผ Upgraded upstream Manifests to v1.6.0
- ๐ผ Upgraded ASM to v 1.14 (#385).
- ๐ผ Upgraded Knative to v 1.2 (#373).
- ๐ผ Upgraded cert-manager to v 1.5 (#372).
- ๐ผ Upgraded pipelines to v 2.0.0-alpha.4.
- ๐ผ Upgraded APIs to support GKE 1.22 (#349).
- ๐จ Improved deployment stability (#371, #376, #384, #386).
- ๐ Removed deprecated kfserving, cloud-endpoints, and application manifests (#375, #377).
- ๐งช Validated deployment using GKE 1.21 and GKE 1.22.

## 1.5.1

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.5.1)

### Changes:

- ๐ผ Upgraded ASM to v 1.13.
- ๐จ Fixed KServe issues with dashboard (#362) and directory(#361).
- ๐ Increased the maximum length of Kubeflow cluster name (#359).
- ๐ Moved RequestAuthentication policy creation to iap-enabler to improve GitOps friendliness (#364).
- ๐งช Validated deployment using GKE 1.21.11.

## 1.5.0:

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.5.0)

### Changes:

- ๐ผ Upgrade Kubeflow components versions as listed in [components versions table](https://github.com/kubeflow/manifests/tree/v1.5.0#kubeflow-components-versions)
- ๐ Integrated with Config Controller, simplified management cluster maintenance cost, there is no need to manually upgrade Config Connector CRD.
- ๐ Switch from kfserving to KServe as default serving component, you can switch back to kfserving in `config.yaml`.
- ๐จ Fixed cloudsqlproxy issue with livenessProbe configuration.
- ๐งช Validated deployment using GKE 1.20.12.

## 1.4.1

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.4.1)

### Changes:

Changes on top of v1.4.0:

- ๐ผ Upgrade: Integrate with Kubeflow 1.4.1 manifests (kubeflow/manifests#2084)
- ๐จ Fix: Change cloud endpoint images destination (#343)
- ๐จ Fix: Use yq4 in iap-ingress Makefile.

## 1.4.0:

[Release notes](https://github.com/GoogleCloudPlatform/kubeflow-distribution/releases/tag/v1.4.0)

### Changes:

- ๐ผ Upgrade Kubeflow components versions as listed in components versions table
- ๐ข Removed GKE 1.18 image version and k8s runtime pin, now GKE version is default to Stable channel.
- ๐ Set Emissary Executor as default Argo Workflow executor for Kubeflow Pipelines.
- ๐ผ Upgraded kpt versions from 0.X.X to 1.0.0-beta.6.
- ๐ผ Upgraded yq from v3 to v4.
- ๐ผ Upgraded ASM(Anthos Service Mesh) to 1.10.4-asm.6.
- ๐ Unblocked KFSserving usage by removing commonLabels from kustomization patch #298 #324.
- ๐ Integrated with KFServing Web App UI.
- ๐ Integrated with unified operator: training-operator.
- ๐ช Simplified deployment: Removed requirement for independent installation of yq, jq, kustomize, kpt.
