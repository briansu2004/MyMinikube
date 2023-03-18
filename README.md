# MyMinikube

My Minikube

## Minikube in Windows 10 (1 CPU)

- Install

- Upgrade kubernetes version

```dos
PS C:\devbox> minikube start --kubernetes-version=v1.25.3
* minikube v1.29.0 on Microsoft Windows 10 Enterprise 10.0.19044.2604 Build 19044.2604

X Exiting due to K8S_DOWNGRADE_UNSUPPORTED: Unable to safely downgrade existing Kubernetes v1.26.1 cluster to v1.25.3
* Suggestion:

    1) Recreate the cluster with Kubernetes 1.25.3, by running:

    minikube delete
    minikube start --kubernetes-version=v1.25.3

    2) Create a second cluster with Kubernetes 1.25.3, by running:

    minikube start -p minikube2 --kubernetes-version=v1.25.3

    3) Use the existing cluster at version Kubernetes 1.26.1, by running:

    minikube start --kubernetes-version=v1.26.1


PS C:\devbox>  minikube delete
* Deleting "minikube" in docker ...
* Deleting container "minikube" ...
* Removing C:\Users\x239757\.minikube\machines\minikube ...
* Removed all traces of the "minikube" cluster.
PS C:\devbox> minikube start --kubernetes-version=v1.26.1
* minikube v1.29.0 on Microsoft Windows 10 Enterprise 10.0.19044.2604 Build 19044.2604
* Automatically selected the docker driver. Other choices: hyperv, virtualbox, ssh
* Using Docker Desktop driver with root privileges
* Starting control plane node minikube in cluster minikube
* Pulling base image ...
    > gcr.io/k8s-minikube/kicbase...:  407.19 MiB / 407.19 MiB  100.00% 6.88 Mi
* Creating docker container (CPUs=2, Memory=8100MB) ...
* Preparing Kubernetes v1.26.1 on Docker 20.10.23 ...
  - Generating certificates and keys ...
  - Booting up control plane ...
  - Configuring RBAC rules ...
* Configuring bridge CNI (Container Networking Interface) ...
* Verifying Kubernetes components...
  - Using image gcr.io/k8s-minikube/storage-provisioner:v5
* Enabled addons: default-storageclass

! C:\ProgramData\chocolatey\bin\kubectl.exe is version 1.22.4, which may have incompatibilities with Kubernetes 1.26.1.
  - Want kubectl v1.26.1? Try 'minikube kubectl -- get pods -A'
* Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default
```

## Minikube in Ubuntu (Windows + VirtualBox + Vagrant)

Not working

## Minikube in Mac (4 cores)
