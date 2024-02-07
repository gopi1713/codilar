<!--- app-name: Analytics -->

# Analytics packaged by Codilar

Analytics is an open source for cWarmer, cWarmer is a product built by Codilar, an award-winning Magento (Adobe) Solution Partner and a leader in performance-driven ecommerce solutions.


[Overview of cWarmer](https://cwarmer.io/) 

## cWarmer, a Software as a Service (SAAS) solution designed for Magento which guarantees that visitors consistently experience cached versions of pages within a Magento store which is 100X faster.

Trademarks: This software listing is packaged by Codilar. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.
                           
## TL;DR

```bash
$ helm repo add codilar https://helm.codilar.dev/
$ helm install my-release codilar/Analytics
```

## Introduction

This chart bootstraps a [Analytics]( https://gitlab.codilar.in/api/v4/projects/703/packages/helm/stable) replication cluster deployment on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.



Codilar charts can be used with [Kubeapps](https://kubeapps.dev/) for deployment and management of Helm Charts in clusters.

## Prerequisites

- Kubernetes 1.19+
- Helm 3.2.0+
- PV provisioner support in the underlying infrastructure

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ helm install my-release codilar/Analytics
```

The command deploys Analytics on the Kubernetes cluster in the default configuration. The [Parameters](#parameters) section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```bash
$ helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.


