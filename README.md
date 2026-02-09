# example-angular

[![view-action-graph](https://img.shields.io/github/actions/workflow/status/actionforge/example-angular/workflow.yml?label=View%20Action%20Graph)](https://app.actionforge.dev/github/actionforge/example-angular/main/.github/workflows/graphs/build.act)

A simple Hello World app in Angular, built using an [Actionforge](https://actionforge.dev) graph as the CI/CD pipeline.

## Build

```bash
npm install
npm run build
```

## Graph

The build pipeline is defined as an Actionforge graph in [`.github/workflows/graphs/build.act`](.github/workflows/graphs/build.act):

```
checkout -> build -> upload-artifact
```

It runs on every push to `main`, on pull requests, and on manual dispatch.
