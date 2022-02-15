# How to Install the Prometheus Monitoring Stack
## Prerequisites
1. A [Git](https://git-scm.com/downloads) client, to clone the `Starter Kit` repository.
2. [Helm](https://www.helms.sh), for managing `Promtheus` stack releases and upgrades.
3. [Kubectl](https://kubernetes.io/docs/tasks/tools), for `Kubernetes` interaction.
4. [Curl](https://curl.se/download.html), for testing the examples (backend applications).

## Step 1 - Installing the Prometheus Stack
1. Clone project:
```shell
git clone https://github.com/kittisuw/kube-prometheus-stack.git
```
2. เพิ่ม helm repository และ list chart ที่มีให้ใช้   
```shell
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
helm search repo prometheus-community
```
ผลลัพธ์ที่ได้จะประมาณนี้
```shell
NAME                                                    CHART VERSION   APP VERSION     DESCRIPTION                                       
prometheus-community/alertmanager                       0.15.0          v0.23.0         The Alertmanager handles alerts sent by client ...
prometheus-community/kube-prometheus-stack              32.2.1          0.54.0          kube-prometheus-stack collects Kubernetes manif...
...
```