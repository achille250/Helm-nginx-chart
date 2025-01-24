# Helm_nginx_chart
 A Helm chart for deploying and managing Nginx on Kubernetes using Minikube.
## Features
- Deploys Nginx using a customizable Helm chart.
- Configurable options for replicas, image version, and service type.
- Supports Ingress for routing traffic to the application.
## Prerequisites
- Kubernetes cluster (Minikube recommended for local development).
- Helm installed on your local machine.
  ## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/achille250/Helm-nginx-chart.git
   cd Helm-nginx-chart
2. Deploy the Helm chart:
   ```bash
   helm install my-nginx ./nginx-chart
3. Verify the deployment:
   ```bash
   kubectl get all
   
5. Accessing the Application
  using Ingress, ensure your DNS is configured to point to the Minikube IP and access the application via http://nginx.local. 
   
## Repository Structure
```bash
Helm-nginx-chart/
├── charts/                # Subcharts (if any)
├── templates/             # Kubernetes resource templates
├── values.yaml            # Default configuration values
├── Chart.yaml             # Chart metadata
└── README.md              # Project documentation
