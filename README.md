# OpenSearch Kubernetes Operator

**This repository is no longer maintained. Please use the [upstream opensearch-k8s-operator](https://github.com/opensearch-project/opensearch-k8s-operator) from the Opensearch organization.**

## Getting started

The Operator can be easily installed using helm on any CNCF-certified Kubernetes cluster. Please refer to the [User Guide](./docs/userguide/main.md) for installation instructions.

## Current feature list

- [x] Deploy a new OS cluster.
- [x] Ability to deploy multiple clusters.
- [x] Spin up OS dashboards.
- [x] Configuration of all node roles (master, data, coordinating..).
- [x] Scale the cluster resources (manually), per nodes' role group.
- [x] Drain strategy for scale down.
- [x] Version updates.
- [x] Change nodes' memory allocation and limits.
- [x] Secured installation features.
- [x] Certificate management.
- [x] Rolling restarts - through API.
- [x] Scaling nodes' disks - increase disk size.
- [x] Cluster configurations and nodes' settings updates.
- [x] Operator Monitoring, with Prometheus and Grafana.

## Installation

The Operator can be easily installed using Helm:

1. Add the helm repo: `helm repo add opensearch-operator https://maibornwolff.github.io/opensearch-operator/`
2. Install the Operator: `helm install opensearch-operator opensearch-operator/opensearch-operator`

## Compatibility

The operator aims to be compatible with all current and supported Opensearch 2.x versions. When a new Opensearch version comes out it might take some time for the operator to support specific features, but in general all 2.x versions should work. Note that the operator will not prevent you from running any version, regardless of if it was tested or not.

## Development

If you want to develop the operator, please see the separate [developer docs](./docs/developing.md).

## Contributions

We welcome contributions! See how you can get involved by reading [CONTRIBUTING.md](./CONTRIBUTING.md).
