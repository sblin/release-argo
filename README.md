# Release Integration sample with Argo CD

## argocd directory
The directory contains a sample app to demonstrate integration between Digital.ai Release and Argo CD.

- `apps` directory: contains the definition of the argo CD apps in single manifest files.
The `helloworld-apps.yaml` file is the definition for the pattern 'App of Apps': see the [Argo CD documentation](https://argo-cd.readthedocs.io/en/stable/operator-manual/declarative-setup/#app-of-apps) for more info.
- `helloworld-src` directory: contains the source of the application.
- `templates` directory: contains the Release templates definition; use the xl cli to import `xl apply xl-release -f templates.yaml`; you'll have to change the connection for the Argo CD server.
- `root-app.yaml` file: it's the definition of the root app for the 'App in Apps' pattern (see before)

## helloworld-chart directory
Helm chart version. *** BROKEN, DO NOT USE ***

