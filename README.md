# Project Outline

## Project Goals

1. Provide a scalable instance of the Linkerd service architecture on a Kubernetes cluster.
2. Teach the author about Linkerd, tracing and ingress

## Similar Work

https://github.com/kubernetes/charts/tree/master/stable/linkerd

## Justification

This chart is meant as a littleman.co implementation, similar to the above chart. Ideally, it will replace the above
as this is more recent, and designed to be more configurable. However, that is an optimistic goal, and whether it is
accomplished will depend on time.

## Limitations

This is not used in production anywhere, it's just a learning experience.

## Alerting Policies

Note: These have yet to be tested.

| Policy                  | Description |
|-------------------------|-------------|
|                         |             |

## Security Alerts

See SECURITY.md

## Summary

| License       | Code Style   | Locale        |
|---------------|--------------|---------------|
| MIT           | Zend         | en-AU [lang]_ |

## Compatibility

### Kubernetes

| 1.5 | 1.4 | 1.3 | 1.2 | 1.1 | 1.0
|-----|-----|-----|-----|-----|----
|  Y  |  ?  |  ?  |  ?  |  ?  |  ?

### Linkerd

This is tested on whatever version is in values.yaml; nothing more.

## Installation


Install it with Helm:

    helm upgrade --install linkerd path/to/chart

## Usage

Better check linkerd.io out for that. I am learning myself; I plan to use it as a service mesh so I can track
application calls between applications that do not support tracing well.

## Thanks

- Helm (https://github.com/kubernetes/helm)
- @migmarti (https://github.com/migmartri)
- Boyant

## Contributing

Contributions are always welcome! Nothing is too small, and the best place to start is to open an issue.

## References

- A Service Mesh for Kubernetes, Part I: Top-line service metrics, from https://blog.buoyant.io/2016/10/04/a-service-mesh-for-kubernetes-part-i-top-line-service-metrics/
- Lingoes.net,. (2015). Language Code Table. Retrieved 4 June 2015, from http://www.lingoes.net/en/translator/langcode.htm
- GitHub, (2015). Proposed: security disclosure publication. Retrieved 15 May 2016, from https://github.com/php-fig/fig-standards/blob/master/proposed/security-disclosure-publication.md
