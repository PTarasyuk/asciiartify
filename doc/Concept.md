# Concept

## Intro

- **minikube** - Local deployment of single-node Kubernetes clusters with support for various hypervisors (VirtualBox, KVM, Docker)
- **kind** (Kubernetes IN Docker) - Generates local Kubernetes clusters using Docker containers as nodes
- **k3d** (K3s in Docker) - Creates lightweight local K3s clusters (a lightweight Kubernetes distribution) using Docker containers as nodes

## Features:

|             | **minikube** | **kind**<br>(Kubernetes IN Docker) | **k3d**<br>(K3s in Docker) |
| ----------- | ------------ | ---------------------------------- | -------------------------- |
| Operating system | Linux, Windows, MacOs | Linux, MacOs, Windows | Linux, MacOs, Windows |
| Architecture | x86-84, ARM64, ARMv7, ppc64, S390x | x86-84, ARM64 | x86-84, ARM64, ARMv7 |
| Automation | CLI, predefined profiles | CLI, YAML configuration | CLI, YAML configuration |
| Monitoring | + | - | - |
| Addons | + | - | - |
| Podman | + | + | + |

## Tradeoffs

|             | **minikube** | **kind**<br>(Kubernetes IN Docker) | **k3d**<br>(K3s in Docker) |
| ----------- | ------------ | ---------------------------------- | -------------------------- |
| Last version | v1.32.0 | v0.25.0 | v5.6.0 |
| Documentation     | [minikube.sigs.k8s.io](https://minikube.sigs.k8s.io/docs/) | [kind.sigs.k8s.io](https://kind.sigs.k8s.io/) | [k3d.io](https://k3d.io/) |
| Repository  | <https://github.com/kubernetes/minikube> | <https://github.com/kubernetes-sigs/kind> | <https://github.com/k3d-io/k3d> |
| Popularity<br>(*GitHub Stars*) | 27.6k | 12.3k | 4.8k |
| First commit | April 2016 | September 2018 | April 2019 |
| Releases | 144 | 25 | 139 |
| Contributors | 850 | 295 | 121 |
| Issues | 931 | 172 | 178 |
| Ease of use | beginner friendly | relative simple | simple |
| User friendly | high | medium | medium |
| Speed deployment | medium | high | high |
| Work Stability | high | high | medium (k3s) |

## Conclusion

All three solutions, minikube, k3d and kind are very similar. Each has pros and cons, but none stand out, making them a universal choice. These tools are fast, easy to install, and user-friendly, well-suited to local development needs.

I have a gut feeling that minikube is slightly ahead of all options and the closest to the official Kubernetes development roadmap. It appears to be slightly ahead, providing a robust option, especially for developers who may be relatively new to DevOps practices. Minikube, with its low entry barrier, seems particularly well-suited for individual developers or small teams starting their journey with Kubernetes. In my recommendation, minikube stands out as an excellent choice for those venturing into Kubernetes for the first time.

## Demo

![Demo minikube](./assets/demo.gif)
