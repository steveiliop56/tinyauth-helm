# Tinyauth helm

A helm chart for running Tinyauth in a Kubernetes cluster.

## Development

Documentation and values schema generation is powered by:

- [helm-docs](https://github.com/norwoodj/helm-docs) for generating chart documentation
- [helm-values-schema-json](https://github.com/losisin/helm-values-schema-json) for JSON schema validation

### Generating Chart READMEs

Install tools:

```bash
go install github.com/norwoodj/helm-docs/cmd/helm-docs@latest
```

Generate README:

```bash
cd charts/tinyauth && helm-docs
```

### Generating JSON Schema

Install tools:

```bash
helm plugin install https://github.com/losisin/helm-values-schema-json.git
```

Generate schema:

```bash
cd charts/tinyauth && helm schema
```

### CI Testing

CI uses [chart-testing-action](https://github.com/helm/chart-testing-action) to lint charts and test deployment. Creates a kind cluster and installs tinyauth to verify everything works. Configuration is in `ct.yaml`.

### Releasing

To release a new chart version, create and push a git tag. The release workflow uses [chart-releaser-action](https://github.com/helm/chart-releaser-action) to package and publish charts to GitHub Pages.
