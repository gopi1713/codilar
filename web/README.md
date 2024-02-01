<!--- app-name: web -->

# web packaged by Codilar

web is an open source, community-developed SQL database server that is widely in use around the world due to its enterprise features, flexibility, and collaboration with leading tech firms.

[Overview of web](https://www.nginx.com/)

Trademarks: This software listing is packaged by Codilar. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.
                           
## TL;DR

```bash
$ helm repo add codilar https://helm.codilar.dev/
$ helm install my-release codilar/web
```

## Introduction

nginx has one master process and several worker processes. The main purpose of the master process is to read and evaluate configuration, and maintain worker processes.

Codilar charts can be used with [Kubeapps](https://kubeapps.dev/) for deployment and management of Helm Charts in clusters.

## Prerequisites

- Kubernetes 1.19+
- Helm 3.2.0+
- PV provisioner support in the underlying infrastructure

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ helm install my-release codilar/rabbitmq
```

The command deploys web on the Kubernetes cluster in the default configuration. The [Parameters](#parameters) section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```bash
$ helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Parameters
