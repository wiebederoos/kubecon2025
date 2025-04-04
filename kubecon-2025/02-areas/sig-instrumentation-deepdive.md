# Speakers
* Pranshu Srivastava
* Damien Grisonnet
* Richa Banker
* Yongrui Lin
# Metrics
* Main projects
	* Stability matrix wrt metrics
	* Calculate SLOs for components (detect stability & availability) -> component Health SLIs
	* Meta Metrics to detect deprecated metrics
	* Auto generated documentation for K8S metrics -> helpful to get insight of the metrics
	* Explore z-pages (debug endpoints) -> only for humans
* Subprojects
	* Prometheus metrics collector to collect kubernetes resource usage and capacity metrics
	* Kube state metrics -> for Custom Resource metrics due to limitations of Custom Resource State
		* Various advantages mentioned, see slides
# Logs
* klog -> convert k8s objects to normal google logger (thus lowering the barrier for developers) to make it more queryable
* Add structure to k8s logging -> no need to use regexes tot analyze
	* In plain text but also in json format
* Introduce contextual logging -> skip boilerplate logging code
##  Tracing
* Simplify  understanding of k8s based infrastructure & workloads
* Focus on API server + kubelet
* Complete Pod traces very helpful to debug issues in workload deployments
## Signal correction
* Introduce the ideal debugging path
	* metrics -> traces -> logs by sharing the context between traces and structured logs
* Examplars (SIG instrumentation)
# Resources
* Link to presentation: https://static.sched.com/hosted_files/kccnceu2025/56/KubeCon%20EU%202025%20-%20SIG%20Instrumentation.pdf

#metrics #sig #instrumentation #observability #signal-correction
[[observability]]