# Production-EKS-setup
Setting up a production EKS cluster to deploy multiple microservices

Phase 1
kubectl create namespace ecommerce-prod
kubectl create namespace ecommerce-infra
kubectl create namespace monitoring
kubectl label namespace ecommerce-prod istio-injection=enabled
# Label for easier filtering in kubectl
kubectl label namespace ecommerce-prod env=production team=backend
kubectl label namespace ecommerce-infra env=production team=platform
kubectl label namespace monitoring env=production team=platform
