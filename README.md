# GitOps Repository

With this project, n environment/kubernetes clusters are configured using ArgoCD and managed with GitOps.

## Initialize Repository
````
k apply -k bootstrap/initial/00-namespace/
k apply -k bootstrap/initial/01-argocd
k apply -k bootstrap/initial/02-cluster-core
k apply -k bootstrap/initial/03-cluster-repo-creds

````
## Bootstrap Everything
````
k apply -k bootstrap/initial/04-app-of-apps
````
