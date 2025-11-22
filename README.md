# hello-world Config - PROD

Helm chart for PROD environment.

## Configuration

- **Environment**: PROD
- **Auto-Deploy**: Yes (typically by Release Engineer decision via essesseff)
- **Namespace**: `essesseff-hello-world-go-template` (set in the app-of-apps/argocd/hello-world-prod-application.yaml)
- **Ingress**: `example.com/hello-world-prod`

## Updates

This repository in combination with the app-of-apps environment-specific deployment config determine when/if/how deployments occur via Argo CD.  This repository is updated by essesseff platform when PROD deployments are to occur as per Release Engineer manual decision.

Typically, only the values.yaml file should be manually altered, while any/all other changes in the repository are made via essesseff deployment orchestration.
