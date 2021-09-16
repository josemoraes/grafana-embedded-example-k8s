# Grafana embedded: an example using Kubernetes
An implementation of grafana embedded in an app and authenticated by a proxy.
I developed this example, just to present a way to solve this demand, although, this opens a lot of vulnerabilities if you use it in an environment that needs to be restricted.
You can solve this using an authentication even with this proxy (using nginx basic auth) or using another method, see [Grafana docs](https://grafana.com/docs/grafana/latest/auth/).
This implementation is a bootstrap to help you if you have a scenario where you need to embed Grafana on a page.
To run this example, use:

```bash
kubectl apply -k ./envs/local
```