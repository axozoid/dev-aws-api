## Bootstrap applications deployment in a Kubernetes cluster

Once ArgoCD is installed, run the following command to kick off the deployment of all apps:

```
kubectl -n argocd apply -f https://raw.githubusercontent.com/axozoid/k8s-clusters/dev/dev-aws-api-01/bootstrap/bootstrap.yaml

```

This will install a "root application" that will be deployed as a Helm chart that contains all necessary apps.