<!--- app-name: TimescaleDB -->

# TimescaleDB packaged by Codilar

TimescaleDB is an open source, community-developed SQL database server that is widely in use around the world due to its enterprise features, flexibility, and collaboration with leading tech firms.

[Overview of TimescaleDB](https://www.timescale.com/)

Trademarks: This software listing is packaged by Codilar. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.
                           
## TL;DR

```bash
$ helm repo add codilar https://helm.codilar.dev/
$ helm install my-release codilar/TimescaleDB
```

## Introduction

This chart bootstraps a [TimescaleDB]( https://gitlab.codilar.in/api/v4/projects/703/packages/helm/stable) replication cluster deployment on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

TimescaleDB is developed as open source software and as a relational database it provides an SQL interface for accessing data. The latest versions of TimescaleDB also include GIS and JSON features.

Codilar charts can be used with [Kubeapps](https://kubeapps.dev/) for deployment and management of Helm Charts in clusters.

## Prerequisites

- Kubernetes 1.19+
- Helm 3.2.0+
- PV provisioner support in the underlying infrastructure

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ helm install my-release codilar/TimescaleDB
```

The command deploys TimescaleDB on the Kubernetes cluster in the default configuration. The [Parameters](#parameters) section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```bash
$ helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Parameters



### TimescaleDB common parameters

| Name                       | Description                                                                                                                                                                                                                                                                   | Value                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| `image.registry`           | TimescaleDB image registry                                                                                                                                                                                                                                                        | `docker.io`           |
| `image.repository`         | TimescaleDB image repository                                                                                                                                                                                                                                                      | `TimescaleDB`     |
| `image.tag`                | TimescaleDB image tag (immutable tags are recommended)                                                                                                                                                                                                                            | `10.10` |
| `image.digest`             | TimescaleDB image digest in the way sha256:aa.... Please note this parameter, if set, will override the tag                                                                                                                                                                       | `""`                  |
| `image.pullPolicy`         | TimescaleDB image pull policy                                                                                                                                                                                                                                                     | `IfNotPresent`        |
| `image.pullSecrets`        | Specify docker-registry secret names as an array                                                                                                                                                                                                                              | `[]`                  |
| `auth.rootPassword`        | Password for the `root` user. Ignored if existing secret is provided.                                                                                                                                                                                                         | `""`                  |
| `auth.database`            | Name for a custom database to create                                                                                                                                                                                                                                          | `my_database`         |
| `auth.username`            | Name for a custom user to create                                                                                                                                                                                                                                              | `""`                  |
| `auth.password`            | Password for the new user. Ignored if existing secret is provided                                                                                                                                                                                                             | `""`                  |