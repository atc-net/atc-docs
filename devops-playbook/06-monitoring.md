# Monitoring

`TEXT-IS -MISSING`

Monitoring is the act of collecting and analyzing data to determine the performance, health, and availability of your business application and the resources that it depends on. An effective monitoring strategy helps you understand the detailed operation of the components of your application. It also helps increasing application uptime by proactively notifying about critical issues so that they can be resolved, before becoming bigger problems.

## Application Monitoring

`TEXT-IS -MISSING`

- **Do** instrument your cloud application to emit telemetry, using e.g. Application Insights on Azure
- **Do** provide availability health check endpoints
    > *Several cloud systems, e.g. Application Insights on Azure can monitor availability through http endpoint probing.*

## Platform Monitoring

`TEXT-IS -MISSING`

- **Do** use diagnostics tracing / monitoring
    > *Use it to get notified about issues early and to take automated actions to resolve them quickly.*
- **Consider** have alerts on CPU and RAM usage
- **Consider** monitor scale set / autoscaling