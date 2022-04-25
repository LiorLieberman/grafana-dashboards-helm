# grafana-dashboards

This charts will take dashboards represented as json files from dashboards directory and provision them as a ConfigMap in Kubernetes. 
Those ConfigMaps are consumed automatically by the Grafana dashboards import sidecar.

See: <https://github.com/helm/charts/tree/master/stable/grafana#sidecar-for-dashboards>

| Parameter                  | Description                                                          | Default |
|----------------------------|----------------------------------------------------------------------|---------|
| `labels.grafana_dashboard` | set grafana_dashboard label                                          | `"1"`   |
| `importFromValue`          | import dashboard form value string instead from dashboards directory | `{}`    |
