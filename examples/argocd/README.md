# Deploy by Argocd 
## Argo CD
### TLS
`sudo kubectl create secret tls deepin-app-tls \
  --cert=./certs/deepin.app/cert.pem \
  --key=./certs/deepin.app/private-key.pem \
  -n argocd`

## Ingress
- `kubectl apply -f argocd-ingress.yaml`
- `kubectl get ingress -n argocd`