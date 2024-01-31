<!-- markdownlint-disable-next-line -->


# The Codilar Library for Kubernetes

Popular applications, provided by [Codilar](https://www.codilar.com), ready to launch on Kubernetes using [Kubernetes Helm](https://github.com/helm/helm).






## Before you begin
Add the repo

```bash
$ helm repo add codilar https://helm.codilar.dev/
$ helm repo update
$ helm search repo codilar  ----> To get the required charts
```

### Prerequisites

- Kubernetes 1.23+
- Helm 3.8.0+


### Install Helm

Helm is a tool for managing Kubernetes charts. Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://github.com/helm/helm#install) and ensure that the `helm` binary is in the `PATH` of your shell.

### Using Helm

Once you have installed the Helm client, you can deploy a Bitnami Helm Chart into a Kubernetes cluster.

Please refer to the [Quick Start guide](https://helm.sh/docs/intro/quickstart/) if you wish to get running in just a few commands, otherwise, the [Using Helm Guide](https://helm.sh/docs/intro/using_helm/) provides detailed instructions on how to use the Helm client to manage packages on your Kubernetes cluster.
