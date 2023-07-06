# FluxCD Deploy Feeder

This repository contains the manifests for the FluxCD Deploy Feeder, a component designed to feed deployment events to FluxCD via [fluxcd2-bootstrap](https://github.com/yashwanth-l/fluxcd2-bootstrap) Repo

## Directory Structure

The directory structure of this repository is as follows:

- **`deploy-helm/flux-kind-k8s`**: This directory contains the applications of `kind: HelmRelease` organized by namespace, considering the HelmRepo is added to the [fluxcd2-bootstrap](https://github.com/yashwanth-l/fluxcd2-bootstrap) repo.

- **`deploy-kustomize/base`**: This directory holds the configuration bases for various tools that can be deployed to the cluster via _kustomize_.

- **`deploy-kustomize/flux-kind-k8s`**: This directory contains the application's `kustomization.yaml` structured in `<namespace>/<application>`

## Prerequisites

Before using the FluxCD Deploy Feeder, ensure that you have the following prerequisites in place:

- [fluxcd2-bootstrap](https://github.com/yashwanth-l/fluxcd2-bootstrap) has this repo as `kind: GitRepository` defined, with credentials if a private repo.

## Support

If you have any questions or need assistance, please open an [issue](https://github.com/yashwanth-l/fluxcd-deploy-feeder/issues).
