# Cluster API deployment on vSPHERE using helm and ArgoCD

<p float="center">
  <img src="./docs/images/git-icon.png" width="160" /> 
  <img src="./docs/images/plus2.png" width="50" /> 
  <img src="./docs/images/argocd.png" width="160" /> 
  <img src="./docs/images/plus2.png" width="50" /> 
  <img src="./docs/images/capi.png" width="160" />
</p>

## Goals

- To simplify kubernetes deployments using using declarative (ClusterAPI)  style code
- Use helm to modify k8 cluster values based on requirement. This helps in code reusability
- Version control
- Using GitOps(ArgoCD) to deploy, scale-in/scale-out your Kubernetes infrastructure

## Prerequisites

- [kind](https://kind.sigs.k8s.io/) - This will act as your management cluster for bootstrapping cluster-api components.
- [clusterctl](https://cluster-api.sigs.k8s.io/user/quick-start.html) - The clusterctl CLI tool handles the lifecycle of a Cluster API management cluster.
- [Govc](https://github.com/vmware/govmomi/tree/master/govc) - Govc will be used to interact with your vSphere environment.
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [helm3](https://github.com/helm/helm)
- vSphere 6.7U3 or above

For more information refer to the cluster-api [quickstart](https://cluster-api.sigs.k8s.io/user/quick-start.html)
