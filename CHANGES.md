Changes by Version
==================
Release Notes.

8.6.0
------------------
#### Project


#### Java Agent
* Add `trace_segment_ref_limit_per_span` configuration mechanism to avoid OOM.
* Improve `GlobalIdGenerator` performance.
* Add an agent plugin to support elasticsearch7.
* Add `jsonrpc4j` agent plugin.
* new options to support multi skywalking cluster use same kafka cluster(plugin.kafka.namespace)
* resolve agent has no retries if connect kafka cluster failed when bootstrap
* Add Seata in the component definition. Seata plugin hosts on Seata project.
* Extended Kafka plugin to properly trace consumers that have topic partitions directly assigned.
* Support print SkyWalking context to logs.
* Add `MessageListener` enhancement in pulsar plugin
* Add an optional agent plugin to support mybatis.

#### OAP-Backend
* BugFix: filter invalid Envoy access logs whose socket address is empty.
* Fix K8s monitoring the incorrect metrics calculate. 
* Loop alarm into event system.
* Support alarm tags.
* Support WeLink as a channel of alarm notification.
* Fix: Some defensive codes didn't work in `PercentileFunction combine`.
* CVE: fix Jetty vulnerability. https://nvd.nist.gov/vuln/detail/CVE-2019-17638

#### UI
* Add logo for kong plugin.
* Add apisix logo.
* Refactor js to ts for browser logs and style change.
* When creating service groups in the topology, it is better if the service names are sorted.
* Add tooltip for dashboard component.
* Fix style of endpoint dependency.
* Support search and visualize alarms with tags.

#### Documentation
* Polish k8s monitoring otel-collector configuration example.
* Print SkyWalking context to logs configuration example.

All issues and pull requests are [here](https://github.com/apache/skywalking/milestone/84?closed=1)

------------------
Find change logs of all versions [here](changes).
