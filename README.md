# fluxing
flux cd playground while watching https://youtu.be/X5W_706-jSY

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
kubectl -n flux-syste get GitRepository
kubectl -n flux-system get Kustomization
```