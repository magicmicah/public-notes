Purpose is to actively collect system metrics and logs
track errors when they occur
store metrics to observe the system
react to incidents through alerts

## Monitoring Service![[monitoring.png]]

Metric - measurement related to health, capacity or performance of a resource.

Metric namespace - resource, service or app that emits the metric

Service Metrics | Custom Metrics

Filter by dimensions and time period.

## Alarms
Resources are monitored via metrics which are tagged to an alarm. The alarm publishes to a topic which will then be consumed by a notification - email, sms, slack, etc. 

Alarm states - ok, firing, reset, repeat

Suppression - avoid publishing alarm messages. 

## Logging

Highly scalable and fully managed pane of glass for all logs

Built on open standards such as fluentd log ingestion. Compliant CNCF CloudEvents 1.0

Rule-based actions on log events.
searchable, actionable, transportable. create alarms on log data
transport alarms to another service

service connector hub
create alarms on log data
alamrs on sending log data to monitoring service

Logs are always encrypted - in flight, disk-level, archived

A log is a resource that stores and captures log events. 

Object storage logs for buckets - read and write access events

Write event - put, post, delete

read event - get, list, head

Every service can have different log categories. example, functions will have different log categories than object storage service. 

### Log Groups
Logical containers for logs to streamline log management.

Logs and log groups are searchable and transportable

IAM policy can be used to limit access to sensitive logs.


### Types of Logs

Service logs - emitted by OCI services like Object Storage, VCN, etc
Predefined logging categories that can be enabled or disabled on-click.

Custom logs - emitted by custom applications on OCI, other cloud providers, on-premises apps.
Custom applications can ingest logs by using API or unified monitoring agent.

Audit logs - related to audit events emitted by OCI Audit service
Accessed from the console
Every OCI service supports logging by audit

## Events

Enables automation on state changes of resources throughout tenancy. 
services emit events for resources or data
example - object storage emits events such as create, update, delete, etc.

Event types can have rules setup that will emit an action or trigger which can then notify team.

Events will have structured and schematized messages that denote a change in a resource

Rules are the configuration where a user defines events that need to be created and triggers an action if they occur

Actions are the user defined response when an event occurs. Can be notifications, streaming or functions. 

## Oci Events Service in Action
![[events-in-action.png]]
