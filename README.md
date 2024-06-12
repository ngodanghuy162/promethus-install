Các bước cài:
- Clone folder.
- cd promethus-install/manifest
- kubectl apply -f prometheus-operator/namespace.yaml
- kubectl apply --server-side -f prometheus-operator/crds
- kubectl apply -f prometheus-operator/rbac
- kubectl apply -f prometheus-operator/deployment
- kubectl apply -f prometheus
- Sau đó, ta sẽ truy cập được vào dạng serive dạng nodeport theo e dể file service (port 30900). / có thể chạy: kubectl port-foward svc/prometheus-operated 9090 -n monitoring (port 9090)
