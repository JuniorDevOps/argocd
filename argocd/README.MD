# Create namespace and install core Argo CD components only:
```
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/core-install.yaml
```
# Install ARGOCD CLI:
```
brew install argocd
```
# Port-forwarding:
```
kubectl port-forward svc/argocd-server -n argocd 8080:443
```
# The API server can then be accessed using:
```
 https://localhost:8080
```
# You can simply retrieve this password using the argocd CLI:
```
argocd admin initial-password
```

No, I would like to add some changes.