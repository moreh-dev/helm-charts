## Helm Chart

```shell
helm repo add moreh https://moreh-dev.github.io/helm-charts
```

```shell
helm repo update moreh
```

```shell
helm search repo moreh
```

## Register a chart

Get the compressed chart from the repository or chart directory of your choice.

```shell
helm pull <repo>/<chart> --version <version>
```

```shell
helm pull <chart> --repo <repoURL> --version <version>
```

```shell
helm pull <chartURL> --version <version>
```

```shell
helm package <chartDir>
```

Move the compressed chart to the `charts` directory.

```shell
mv <chart>-<version>.tgz ./charts
```

Update the `index.yaml` file.

```shell
make index
```
