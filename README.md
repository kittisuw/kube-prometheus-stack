# How to Install the Prometheus Monitoring Stack
## Prerequisites
1. A [Git](https://git-scm.com/downloads) client, to clone the `Starter Kit` repository.
2. [Helm](https://www.helms.sh), for managing `Promtheus` stack releases and upgrades.
3. [Kubectl](https://kubernetes.io/docs/tasks/tools), for `Kubernetes` interaction.
4. [Curl](https://curl.se/download.html), for testing the examples (backend applications).

## Step 1 - Installing the Prometheus Stack
1. Clone project
```shell
git clone https://github.com/kittisuw/kube-prometheus-stack.git
```
2. เพิ่ม helm repository สำหรับ chart kube-prometheus-stack
```shell
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
helm search repo prometheus-community
```