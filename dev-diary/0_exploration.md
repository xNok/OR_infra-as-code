Exploration
---

## links

* (Kubernetes)[https://kubernetes.io/docs/tutorials/kubernetes-basics/]
    * (Install Docker)[https://kubernetes.io/docs/setup/production-environment/container-runtimes/#docker]
    * (Install Kubelet/kubeadm/kubectl)[https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/install-kubeadm/]
* (Data Science: Kubeflow)[https://www.kubeflow.org]
* (Iot: KubeEdge)[https://kubeedge.io/en/]

## Setup

### 1.1
```bash
make install-docker
```
### 1.2
```bash
make check-docker
```
### 2.1
```bash
make install-kube
```
### 2.2
```bash
kubeadm init
```

```bash
vi /etc/kubernetes/manifests/kube-apiserver.yaml
# Add the following flags in spec: containers: -command section
- --insecure-port=8080
- --insecure-bind-address=0.0.0.0
```

