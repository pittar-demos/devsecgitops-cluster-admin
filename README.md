# DevSecOps with OpenShift Pipelines, OpenShift GitOps, and Quay!

1. Install OpenShift GitOps:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/openshift-gitops-operator/overlays/gitops-1.10
```

2. Configure OpenShift GitOps with OpenShift GitOps :)

```
oc apply -k https://github.com/pittar-demos/demo-catalog/openshift-gitops-instances/argocd/openshift-gitops
```

3. Deploy another instance of OpenShift GitOps for Developers to use:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/openshift-gitops-instances/argocd/gitops
```

4. Install OpenShift Pipelines:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/openshift-pipelines-operator/argocd
```
