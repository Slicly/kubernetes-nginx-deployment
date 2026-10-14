\# Kubernetes NGINX Deployment Project



\## Project Overview

Deployed and managed an NGINX web application using a local Kubernetes cluster running in Docker Desktop on Windows with WSL 2.



\## Technologies Used

\- Kubernetes and kubectl

\- Docker Desktop and WSL 2

\- NGINX

\- YAML

\- PowerShell



\## Project Implementation

1\. Configured a local Kubernetes cluster using Docker Desktop.

2\. Deployed an NGINX application using Kubernetes.

3\. Scaled the deployment from one to three replicas.

4\. Tested Kubernetes self-healing by deleting a Pod and verifying its replacement.

5\. Created a ClusterIP Service and accessed the application using port forwarding.

6\. Created declarative YAML configuration files for the Deployment and Service.

7\. Applied the configurations using kubectl and verified resource health.



\## Project Files

\- `deployment.yaml` — NGINX Deployment with three replicas.

\- `service.yaml` — Internal ClusterIP Service.



\## Deployment Commands

```powershell

kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

kubectl get deployments,pods,services

kubectl port-forward service/nginx 8080:80

```



Access the application at http://localhost:8080 while port forwarding is running.



\## Key Skills Demonstrated

Kubernetes deployments, container orchestration, horizontal scaling, self-healing, networking, YAML configuration, and troubleshooting.



\## Future Improvements

\- Configure resource requests and limits.

\- Implement readiness and liveness probes.

\- Explore Kubernetes RBAC and network policies.

\- Add CI/CD automation using GitHub Actions.

