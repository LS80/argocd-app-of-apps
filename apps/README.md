
```
argocd app create ls-sync-wave-issue \
  --repo https://github.com/LS80/argocd-app-of-apps.git \
  --path apps \
  --dest-namespace argocd \
  --dest-server https://kubernetes.default.svc \
  --helm-set namespace=ls-sync-wave-issue \
  --helm-set branch=ls-sync-wave-issue \
  --revision ls-sync-wave-issue \
  --sync-policy auto \
  --project draft
```
