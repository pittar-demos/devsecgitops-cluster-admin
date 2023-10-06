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

5. Install and configure Tekton Chains:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/tekton-chains/argocd
```

6. Install Advanced Cluster Security Operator:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/advanced-cluster-security-operator/argocd
```

7. And then an ACS instance and Secured Cluster:

```
oc apply -k https://github.com/pittar-demos/demo-catalog/advanced-cluster-security-instances/argocd
```

## Applications!

### Admins: Create Namespaces

```
oc apply -k https://github.com/pittar-demos/devsecops-minimal/admins/cicd-tools/argocd

oc apply -k https://github.com/pittar-demos/devsecops-minimal/admins/petclinic/argocd/dev

oc apply -k https://github.com/pittar-demos/devsecops-minimal/admins/petclinic/argocd/test

oc apply -k https://github.com/pittar-demos/devsecops-minimal/admins/petclinic/argocd/cicd
```

### Developers: Create Apps and Pipelines

```
oc apply -k https://github.com/pittar-demos/devsecops-minimal/devs/petclinic/argocd/dev

oc apply -k https://github.com/pittar-demos/devsecops-minimal/devs/petclinic/argocd/test

oc apply -k https://github.com/pittar-demos/devsecops-minimal/devs/petclinic/argocd/cicd

oc apply -k https://github.com/pittar-demos/devsecops-minimal/devs/cicd-tools/argocd
```