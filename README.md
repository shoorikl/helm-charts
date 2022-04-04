# helm-charts

Cluster-issuer is a simplistic helm chart that deployes a ClusterIssuer and an Issuer CRDs to work together with the cert-manager; particularly useful in terraform contexts. To deploy by hand, follow these steps.

* Install helm: `brew install helm`.
* Add a repo: `helm repo add shoorikl https://shoorikl.github.io/helm-charts/`
* Refresh all repos: `helm repo update`
* Look for available versions: `helm search repo cluster-issuer --versions`
* Create a values file `myvalues.yaml`
* Pick a version, and install: `helm install cluster-issuer shoorikl/cluster-issuer --create-namespace -n NAMESPACE --version VERSION -f myvalues.yaml`

