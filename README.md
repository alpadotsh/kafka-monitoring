# Kafka Monitoring

_This document describes a general approach to Kafka monitoring._

Kafka can be monitored from at least a few places:

- broker
	- metrics
	- logs
- clients
	- synthetic clients
	- real clients
- infrastructure that sits in between, e.g. load balancers

## SLIs, SLOs or SLTs and SLAs

- SLI (service-level indicator) – a metric that describes one aspect of service reliability. It should be closely
  aligned with user's experience. Good SLI is usually somethig external to the broker to reflect customer experience
  better
- SLO (service-level objective) or SLT (service-level threshold) – is an SLI combined with a target value
- SLA (service-level agreement) is a legal agreement between a service provider and a client. It usually includes
  several of SLOs.

### Client SLIs

- latency – how long it takes for a message to be produced or consumed
- throughput – how many messages can be produced or consumed per second
- error rate – how many messages are lost or fail to be produced or consumed
- correctness – how many messages are produced or consumed correctly


## References

1. Kafka: The Definitive Guide: Real-Time Data and Stream Processing at Scale 2nd Edition by Gwen Shapira (Author), Todd
   Palino (Author), Rajini Sivaram (Author), Krit Petty (Author)
