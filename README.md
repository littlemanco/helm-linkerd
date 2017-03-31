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

See MONITORING.md

## Security

See SECURITY.md

## Summary

| License       | Code Style   | Locale        |
|---------------|--------------|---------------|
| MIT           | Zend         | en-AU [lang]_ |

## Compatibility

### Kubernetes

Tested on GKE, with beta APIs enabled

| 1.5 | 1.4 | 1.3 | 1.2 | 1.1 | 1.0 |
|-----|-----|-----|-----|-----|-----|
|  Y  |  ?  |  ?  |  ?  |  ?  |  ?  |

### Linkerd

This is tested on whatever version is in values.yaml; nothing more.

## Installing the Chart

To install the chart with the release name `my-release`:

```console
$ helm install --name my-release path/to/chart/
```

The command deploys linkerd on the Kubernetes cluster in the default configuration. The [configuration](#configuration)
section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Upgrading the CHart

The chart deploys a DaemonSet (DS) object onto the cluster. Unfortunately, there is currently no way to upgrade a DS
(unless you're on Kubernetes 1.6, for which this chart is untested). You will have to delete the DS and reprovision it.


## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

```console
$ helm delete my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration


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

- BuoyantIO/linkerd-examples, from https://github.com/BuoyantIO/linkerd-examples/blob/master/k8s-daemonset/k8s/linkerd.yml
- A Service Mesh for Kubernetes, Part I: Top-line service metrics, from https://blog.buoyant.io/2016/10/04/a-service-mesh-for-kubernetes-part-i-top-line-service-metrics/
- Lingoes.net,. (2015). Language Code Table. Retrieved 4 June 2015, from http://www.lingoes.net/en/translator/langcode.htm
- GitHub, (2015). Proposed: security disclosure publication. Retrieved 15 May 2016, from https://github.com/php-fig/fig-standards/blob/master/proposed/security-disclosure-publication.md
