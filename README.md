# argocd-linuxdays-example
ArgoCD example from LinuxDays


ArgoCD  1.6.2 with k3d working state:

https://github.com/leheckaj/argocd-linuxdays-example/tree/a6b8902596a3e7ed78c33dcbccf2a6468dc14e6e

Folder plan:
```bash
argocd-linuxdays-example
  \apps
    \argocd
      \clusters
      \patches   -- also for service
      \repos
      \projects
      app_of_apps.yml
      ingress.yml
      kustomization.yml
      namespace.yml
  \appsets
  app_of_apps.yaml

Firstly create ArgoCD in k8s (kubectl apply -k . -n argocd   in appropriate folder)
Secondly apply app_of_apps.yaml (kubectl apply -f app.... -n argocd)
```
