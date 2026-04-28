Name: Parnav Kumar
Registration No: 12209660
Roll No: 41
Section: 4OM05
This project demonstrates a complete DevOps lifecycle by deploying a cloud-native application using Kubernetes. The FitMotion website (a React-based fitness platform) is containerized, deployed, monitored, and scaled automatically based on real-time traffic.
Key highlights:
Containerization using Docker
Deployment on Kubernetes (Minikube)
Monitoring using Prometheus & Grafana
Load testing & troubleshooting
Horizontal Pod Autoscaling (HPA
Tech Stack :-
Frontend: React.js
Containerization: Docker
Orchestration: Kubernetes (Minikube)
Monitoring: Prometheus + Grafana
Package Manager: Helm
Web Server: Nginx)
Commands :-
Start Minikube - minikube start
Build Docker Image - docker build -t fitmotion-app.
Deploy to Kubernetes -kubectl apply -f deployment.yaml  kubectl apply -f service.yaml
Access Application - kubectl port-forward service/fitmotion-service 3000:80
Install Prometheus & Grafana using Helm -helm install monitoring prometheus-community/kube-prometheus-stack
Verification Steps
Check running pods :-kubectl get pods
Load Testing & Autoscaling - kubectl autoscale deployment fitmotion-deployment --cpu-percent=50 --min=2 --max=10
Features -:
Real-time cluster monitoring
Metrics collection using Prometheus
Custom dashboards in Grafana
CPU usage tracking with PromQL
Final Outcome
Fully automated scaling system
Real-time monitoring dashboard
Self-healing Kubernetes deployment
