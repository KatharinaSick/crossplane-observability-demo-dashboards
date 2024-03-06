# Crossplane Observability Demo Dashboards

This repository contains a Helm chart to create Dynatrace dashboards for
the [crossplane-observability-demo](https://github.com/vfarcic/crossplane-observability-demo).
See [values.yaml](./values.yaml) for all possible values and information about them.

## Usage

[Helm](https://helm.sh) must be installed to use the charts. Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```shell
helm repo add crossplane-observability-demo-dashboards https://katharinasick.github.io/crossplane-observability-demo-dashboards
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages. You can then run `helm search repo crossplane-observability-demo-dashboards` to see
the charts.

To install the dashboards chart:

```shell
helm install dashboards crossplane-observability-demo-dashboards/dashboards
```

To uninstall the chart:

```shell
helm delete dashboards
```
