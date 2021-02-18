# k8s-datacenter

## Overview

The K8s-datacenter provides a **fully converged**, homogeneous information system orchestrated by Kubernetes.
All storage, network switching/routing, compute operations are performed by kubernetes.


# Provisioning

1. Installer consumes install-config
2. Values are written to ignition file
3. Ignition file embedded into host os iso file
4. iso is written to usb drive
5. First host is booted in-memory from usb drive
6. Adjacent hosts are pxe booted, in-memory, from each other.
7. Services become available as environment builds


# Host

- Fedora CoreOS based 
- In-memory
- Ignition configurable
- cri-o/kubeadm


## Core Services

- Kube-router
- Kea dhcp
- CoreDNS 
- MetalLB
- Rook/ceph
- Gitea
- FluxCD
- httpd