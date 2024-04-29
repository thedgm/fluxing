# fluxing
flux cd playground

Bootstrapping
```bash
flux bootstrap github \
    --token-auth \
    --owner=thedgm \
    --repository=fluxing \
    --path=kubernetes/fluxcd/repositories/infra-repo/clusters/dev-cluster \
    --personal \
    --branch main
```
flux check
```bash
cubectl -n flux-syste get GitRepository
kubectl -n flux-system get Kustomization
```