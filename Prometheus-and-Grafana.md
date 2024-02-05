# What is Prometheus 

Prometheus is an open source Linux Server Monitoring tool mainly used for metrics monitoring, event monitoring, alert management, etc.

Prometheus has changed the way of monitoring systems and that is why it has become the top-level project of CNCF

Prometheus uses a powerful query language i.e. "PromQL"

In Prometheus tabs handles hundreds of services and microservices.

Prometheus use multiple modes used for graphing and dashboarding support.

Prometheus Configuration file and Components 

prometheus.yml _ it is the configuration file for prometheus where we can do all changes regarding configuration of Prometheus.

Promtool - It is command-line utility tool is used to verify the configuration of Prometheus.

PromQL - Prometheus uses its own query language i.e. PromQL which is very powerful querying language.
PromQL allows the user to select and aggregate the data.

# What is Grafana 

Grafana is a free and open source visualization tool mostly used with Prometheus to which monitor metrics.

Grafana provides various dashboards, charts, graphs, alerts for the particular data source.

Grafana allows us to query, visualize, explore metrics and set alerts for the data source which can be a system, server, nodes, cluster, etc.

We can save the dashboard and can even share with our team member which is one of the main advantage of Grafana.

# What is Node Exporter 

Node exporter is one of the Prometheus exporters which used to expose servers or system OS metrics.

With the help of Node exporter we can expose various resources of the system like RAM, CPU utilization, Memory Utilization, disk space.

Node exporter runs as a system service which gathers the metrics of your system and that gathered metrics is displayed with the help of Grafana visualizatioin tool.
