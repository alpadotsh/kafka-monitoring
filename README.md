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
  serveral of SLOs.

## References

1. Kafka: The Definitive Guide: Real-Time Data and Stream Processing at Scale 2nd Edition by Gwen Shapira (Author), Todd
   Palino (Author), Rajini Sivaram (Author), Krit Petty (Author)
