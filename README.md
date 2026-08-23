# Monitoring Kubernetes system stack for Wodby

Monitoring supplies node, workload, and Kubernetes object telemetry for Wodby
cluster observability.

This repository defines the Wodby stack manifests and default service
composition for Monitoring.

<!-- wodby:generated:start -->

## Stack contract

- [Monitoring stack on Wodby](https://wodby.com/stacks/monitoring)
- [Wodby Kubernetes platform](https://wodby.com)
- [Wodby stack documentation](https://wodby.com/docs/2.0/stacks/)
- [Stack manifest reference](https://wodby.com/docs/2.0/stacks/template/)

## System service definitions

- [Monitoring system service](https://github.com/wodby/service-monitoring)
- [Node exporter system service](https://github.com/wodby/service-node-exporter)
- [Kube state metrics system service](https://github.com/wodby/service-kube-state-metrics)

## What's included

| Component / service | Default configuration |
| --- | --- |
| Monitoring<br>`monitoring` | optional; enabled by default |
| Node exporter<br>`node-exporter` | optional; enabled by default |
| Kubernetes state metrics<br>`kube-state-metrics` | optional; enabled by default |

System services are enabled or disabled according to the cluster provider and
infrastructure configuration.

## Validate the stack manifest

```bash
wodby stack validate-manifest stack.yml --org <org-id>
```

<!-- wodby:generated:end -->
