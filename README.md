# helm-charts
Helm chart repository

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```bash
  helm repo add payfi https://helm.payfi.ng
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
payfi` to see the charts.

### To install the payfi chart:
```bash
  helm install payfi payfi/payfi
```
### To uninstall the chart:
```bash
  helm uninstall payfi
```

### Local development

```bash
helm template payfi charts/payfi/ --values charts/payfi/values.yaml
```
```bash
helm install payfi charts/payfi/ --values charts/payfi/values.yaml
```