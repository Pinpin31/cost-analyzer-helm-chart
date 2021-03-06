# cost-analyzer helm chart
Helm chart for the Kubecost project, which is created to monitor and manage Kubernetes resource spend. Please contact team@kubecost.com or visit [kubecost.com](http://kubecost.com) for more info.


Parameter | Description | Default
--------- | ----------- | -------
`global.prometheus.enabled` | If true, use an existing Prometheus install. More info [here](http://docs.kubecost.com/custom-prom). | `false`
`prometheus.server.persistentVolume.size` | Prometheus server data Persistent Volume size | `8Gi`
`prometheus.server.resources.limits.memory` | Set a memory limit on Prometheus server container | `not set`
`prometheus.server.resources.limits.cpu` | Set a CPU limit on Prometheus server container | `not set`
`prometheus.nodeExporter.enabled` `prometheus.serviceAccounts.nodeExporter.create` | If false, do not crate NodeExporter daemonset  | `true`
`networkPolicy.enabled` | If true, create a NetworkPolicy to deny egress  | `false`
