# Kubernetes-Monitoring-with-Prometheus-and-Grafana

## Project Purpose and Architecture

This project aims to set up monitoring for a Kubernetes cluster using Prometheus and Grafana. Prometheus is used for collecting metrics from Kubernetes resources, and Grafana is used for visualizing these metrics through dashboards.

The architecture consists of the following components:
- Kubernetes cluster
- Prometheus: Collects metrics from Kubernetes API server and other sources.
- Grafana: Visualizes metrics collected by Prometheus through dashboards.

## Tools and Connections

- **Kubernetes Cluster**: Manages containerized applications and resources.
- **Prometheus**: Scrapes metrics from Kubernetes and stores them in a time-series database.
- **Grafana**: Retrieves metrics from Prometheus and displays them through customizable dashboards.

Prometheus scrapes metrics from Kubernetes API server, kubelet, and other sources, and Grafana queries these metrics from Prometheus to create visualizations.

## Installation Guide

### Docker
1. Install Docker using the official Docker documentation.
2. Verify Docker installation with `docker --version`.

### Minikube
1. Install Minikube using the official Minikube documentation.
2. Start Minikube with `minikube start`.
   
### Helm
1. Install Helm using the official Helm documentation.
2. Verify Helm installation with `helm version`.

### Prometheus
1. Add Prometheus Helm repository: `helm repo add prometheus-community https://prometheus-community.github.io/helm-charts`.
2. Update Helm repositories: `helm repo update`.
3. Install Prometheus: `helm install prometheus prometheus-community/prometheus`.

### Grafana
1. Add Grafana Helm repository: `helm repo add grafana https://grafana.github.io/helm-charts`.
2. Update Helm repositories: `helm repo update`.
3. Install Grafana: `helm install grafana stable/grafana`.


## Project Commands

1. Start Minikube: `minikube start`.
2. Install Prometheus: `helm install prometheus prometheus-community/prometheus`.
3. Install Grafana: `helm install grafana stable/grafana`.
4. Check pod resource consumption: `kubectl top pods`.
5. Visualize CPU and memory metrics in Grafana dashboards.
## Concolusion
The project follows a straightforward installation process, leveraging Helm charts to deploy Prometheus and Grafana onto the Kubernetes cluster. Once deployed, users can use commands like kubectl top to view resource consumption metrics directly from the command line, or they can visualize CPU and memory metrics through Grafana dashboards.

![22222222222222222222](https://github.com/Mohab-Hesham/Kubernetes-Monitoring-with-Prometheus-and-Grafana/assets/161193942/6d6709db-9709-45f9-817d-bff4a16ed4f8)

![555555555555555555555](https://github.com/Mohab-Hesham/Kubernetes-Monitoring-with-Prometheus-and-Grafana/assets/161193942/f29206b0-aa20-4195-a127-6ed95d3903a4)

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License

