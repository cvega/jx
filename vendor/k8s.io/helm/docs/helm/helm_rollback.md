## helm rollback

roll back a release to a previous revision

### Synopsis



This command rolls back a release to a previous revision.

The first argument of the rollback command is the name of a release, and the
second is a revision (version) number. To see revision numbers, run
'helm history RELEASE'.


```
helm rollback [flags] [RELEASE] [REVISION]
```

### Options

```
      --dry-run              simulate a rollback
      --force                force resource update through delete/recreate if needed
      --no-hooks             prevent hooks from running during rollback
      --recreate-pods        performs pods restart for the resource if applicable
      --timeout int          time in seconds to wait for any individual Kubernetes operation (like Jobs for hooks) (default 300)
      --tls                  enable TLS for request
      --tls-ca-cert string   path to TLS CA certificate file (default "$HELM_HOME/ca.pem")
      --tls-cert string      path to TLS certificate file (default "$HELM_HOME/cert.pem")
      --tls-key string       path to TLS key file (default "$HELM_HOME/key.pem")
      --tls-verify           enable TLS for request and verify remote
      --wait                 if set, will wait until all Pods, PVCs, Services, and minimum number of Pods of a Deployment are in a ready state before marking the release as successful. It will wait for as long as --timeout
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string               address of Tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of Tiller (default "kube-system")
```

### SEE ALSO
* [helm](helm.md)	 - The Helm package manager for Kubernetes.

###### Auto generated by spf13/cobra on 25-Jan-2018