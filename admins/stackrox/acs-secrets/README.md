# Create "roxsecrets" Secret

This job will create a secret named "roxsecrets" in the namespaces specified in the `postsync-roxsecret-namespaces-cm.yaml` ConfigMap.

Be sure to patch the CM in your own repo to include the namespaces that you require access to the ACS cli (for example, for pipelines).