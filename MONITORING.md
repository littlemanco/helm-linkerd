# Monitoring

Because linkerd operates as the service mesh, it provides extremely valuable diagnostic data that can be used to
determine which services are slow, or are failing to connect. It exports two sets of diagnostic data (in addition
to logs):

## Prometheus (or other TSDB)

Linkerd exposes metrics in the format expected by Prometheus. These are enabled by default; instructions on how to
disable these are in the README.

### Alerting

Alerting should only be dispatched on things that are affecting the user, or will affect the user in the next 4 -
24 hours[1][2].

## Open Tracing

Todo: Work this out.

## Definitions

| Word   | Definition                                                                                              |
|--------|---------------------------------------------------------------------------------------------------------|
| TSDB   | Time Series Database                                                                                    |
| Alert  | A notification that is intended to generate immediate user action at all times of the day (i.e. wake    |
|        |  someone up)                                                                                            |
| Ticket | A report lodged in a bug tracking or other project management system                                    |

## References

[1] SRE Book (alerting chapter)
[2] Brian Brazil youtube video on "What is monitoring"
