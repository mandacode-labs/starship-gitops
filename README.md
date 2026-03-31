# starship-gitops

ArgoCD-based Kubernetes GitOps repository.

## Structure

- `apps/` - Applications (gitea, harbor, keycloak, cert-manager, cnpg, external-secrets, infisical, openebs, etc.)
- `infra/` - Infrastructure (argocd, cilium, envoy-gateway, storage)
- `tls/` - TLS certificate secrets
- `serengeti/`, `starfrag/` - Cluster-specific configurations

## Deployment

ArgoCD ApplicationSet automatically syncs `apps/*` paths. Pushes to main branch trigger automatic deployment.