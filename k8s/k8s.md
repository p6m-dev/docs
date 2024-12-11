# Kubernetes (k8s)

## `kubectl`
The Kubernetes command-line tool, kubectl, allows you to run commands against Kubernetes clusters. You can use kubectl to deploy applications, inspect and manage cluster resources, and view logs.
### Install `kubectl`
[https://kubernetes.io/docs/tasks/tools/](https://kubernetes.io/docs/tasks/tools/)

## `k9s`
K9s is a terminal based UI to interact with your Kubernetes clusters. The aim of this project is to make it easier to navigate, observe and manage your deployed applications in the wild. K9s continually watches Kubernetes for changes and offers subsequent commands to interact with your observed resources.


### Install `k9s`
[https://k9scli.io/topics/install/](https://k9scli.io/topics/install/)

## `kubectx`
`kubectx` is a tool to switch between contexts (clusters) on kubectl faster.
### Insall `kubectx`
[https://github.com/ahmetb/kubectx?tab=readme-ov-file#installation](https://github.com/ahmetb/kubectx?tab=readme-ov-file#installation)

### Usage
Show all k8s contexts
```sh
kubectx
```
Switch k8s 
```sh 
kubectx {context_name}
```
