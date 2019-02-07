# Installing the Client Tools

In this lab you will install the command line utilities required to complete this tutorial: [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl)

## Install kubectl

The `kubectl` command line utility is used to interact with the Kubernetes API Server. Download and install `kubectl` from the official release binaries:

### OS X

```
curl -o kubectl https://storage.googleapis.com/kubernetes-release/release/v1.12.0/bin/darwin/amd64/kubectl
```

```
chmod +x kubectl
```

```
sudo mv kubectl /usr/local/bin/
```

### Linux

```
wget https://storage.googleapis.com/kubernetes-release/release/v1.12.0/bin/linux/amd64/kubectl
```

```
chmod +x kubectl
```

```
sudo mv kubectl /usr/local/bin/
```

### Verification

Verify `kubectl` version 1.12.0 or higher is installed:

```
kubectl version --client
```

> output

```
Client Version: version.Info{Major:"1", Minor:"12", GitVersion:"v1.12.0", GitCommit:"0ed33881dc4355495f623c6f22e7dd0b7632b7c0", GitTreeState:"clean", BuildDate:"2018-09-27T17:05:32Z", GoVersion:"go1.10.4", Compiler:"gc", Platform:"linux/amd64"}
```

Next: [Provisioning The Cluster](03-create-cluster.md)
