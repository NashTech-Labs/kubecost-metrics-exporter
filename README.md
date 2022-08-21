# Kubecost Metrics Expoter 

## Prerequisites

* Kubernetes Cluster
* Helm v3

## Usage

### 1. clone repo 

```
git clone https://github.com/knoldus/kubecost-metrics-exporter.git
cd kubecost-metrics-exporter
```

### 2. Deploy prometheus operator

```
helm upgrade --install prometheus-operator prometheus -f prometheus/custom-values.yaml --namespace prometheus-operator --create-namespace
```

### 3. Deploy the exporter

```
kubectl apply -f kubecost-exporter/
```