# Ingress

# Service vs Ingress

## Scaling

### Kubernetes Autoscaling

Autoscaling is one of the most compelling features of the Kubernetes platform. Once configured correctly, it saves administrators time, prevents performance bottlenecks, and helps avoid financial waste. However, setting up autoscaling requires knowledge of numerous configuration parameters that can confuse even experienced Kubernetes administrators—that’s why created this guide explaining autoscaling in detail.

### The three dimensions of Kubernetes autoscaling

1. ####  Horizontal Autoscaling(HPA)
2. #### Vertical Autoscaling(VPA)
3. #### Cluster Autoscaling(CA)

Autoscaling eliminates the need for constant manual reconfiguration to match changing application workload levels. Kubernetes can autoscale by adjusting the capacity (vertical autoscaling) and number (horizontal autoscaling) of pods, and/or by adding or removing nodes in a cluster (cluster autoscaling).

There are two types of pod autoscalers: Vertical Pod Autoscaler (VPA) can either increase or decrease the CPU and memory allocated to each pod, while the Horizontal Pod Autoscaler (HPA) can replicate or terminate pods, thus affecting the total pod count. Affecting the cluster capacity as a whole, the Cluster Autoscaler (CA) adds or removes nodes dedicated to the cluster to provide the appropriate amount of computing resources needed to host the desired workloads. In combination, the three dimensions of autoscaling help strike—in near-real-time—the delicate balance between preventing performance bottlenecks or outages and avoiding overprovisioning.

![image](https://github.com/Aryan8912/Kubernetes-zero-to-hero/assets/92007507/adad64c0-4a3b-4a95-8392-1eabf836eeba) Source-Kubecast

#### How does HPA work?

![image](https://github.com/Aryan8912/Kubernetes-zero-to-hero/assets/92007507/80c80fae-bca0-418a-b6d6-284ebd7ba957)
In simple terms, HPA works in a “check, update, check again” style loop. Here’s how each of the steps in that loop work.

1. HPA continuously monitors the metrics server for resource usage.
2. Based on the collected resource usage, HPA will calculate the desired number of replicas required.
3. Then, HPA decides to scale up the application to the desired number of replicas.
4. Finally, HPA changes the desired number of replicas.
5. Since HPA is continuously monitoring, the process repeats from Step 1.

### 1. Metrics server
### 2. Horizontal Pod Autoscaler(HPA)
### 3. Cluster Autoscaler(CA)
### 4. Vertical Pod Autoscaler(VPA)
### 5. Overprovisioner
### 6. Custom metrics(Keda)


## What Is Kubernetes Observability? 

Kubernetes observability is the process of gaining insight into the behavior and performance of applications running on Kubernetes, as well as the underlying infrastructure and components, in order to identify and resolve issues more effectively. It can help ensure the stability and performance of Kubernetes workloads, reduce downtime and outages, and improve efficiency.

### The Pillars of Kubernetes Observability 

The pillars of Kubernetes observability are:

1. **Metrics**: Metrics provide a quantitative measurement of various aspects of the system, such as resource utilization, system performance, and application behavior. Metrics are often collected using monitoring tools like Prometheus or InfluxDB.

2. **Logs**: Logs provide a record of events and activities within the system, such as application logs, system logs, and network logs. Logs can be collected and analyzed using tools like Fluentd or ELK.

3. **Tracing**: Tracing provides visibility into the flow of requests and the dependencies between different components in a system. Tracing helps to identify performance bottlenecks and diagnose issues. Tracing can be performed using tools like Jaeger or Zipkin.

4. **Visualization**: Visualization provides a way to represent the data collected from metrics, logs, and tracing in a way
that is easy to understand and navigate. Visualization can be performed using tools like Grafana or Kibana.

## Availability
### 1. Taints and tolerations 
### 2. Liveness, readiness, and startup probes

## Cost optimization
### kubecost

## Statefulsets 
### AWS(EKS)
### Managed node group 
### Fargate
### Karpenter
