# Speakers
* Joe Stephenson
* Rodney Karemba

# Context / use case
* Greenfield project -> time to learn new tools and tech
* Choice of backend not known yet
	* Choose for OpenTelemetry -> easy to start with
## Setup
* Simple initial deployment pattern
* Switch to Multi Cluster Pattern
	* Kubernetes cluster
	* Separate Observability stack

# Blunders
* Time series explosion: from 2 to 38 million
	* Kubernetes Attribute Processor
	* Associations 
		* Use istio & side car model
		* All IPs are the same (bucketcreator and ratelimiter)
* Overwhelming the olly stack
	* Send too much logging data alongside metrics data to Loki
	* Use Kafka to managed the message stream
* Not ensuring system resilience & performance of OpenTelemetry
	* Load testing and chaos engineering
* Switch everything at once
	* Kubelet stats receiver
	* Kubernetes cluster receiver
	* Host metrics receiver
* Ensure HA for OpenTelemetry Gateways
	* Prevent crashes, downtime and datalosses
	* Switch autoscaling on only if mode is deployment or statefulset, not for others


# Comments
* pre-shared slides: https://static.sched.com/hosted_files/colocatedeventseu2025/ec/Otel-y%20Oops%20-%20Observability%20Day%202025.pptx.pdf
* Check WARP

#observability #failure-stories #crash

[[observability]]