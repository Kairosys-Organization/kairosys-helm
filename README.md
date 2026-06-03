# Kairosys Helm Chart Repository

Add the repo:

```sh
helm repo add kairosys https://kairosys-organization.github.io/kairosys-helm
helm repo update
```

Search available charts:

```sh
helm search repo kairosys
```

Install (supply your own values file with image registry, ACM cert, integration URLs, and secrets):

```sh
helm install kairosys kairosys/kairosys \
  --namespace pathfinder --create-namespace \
  -f your-values.yaml
```

See the chart README on the `main` branch for the full list of required values.
