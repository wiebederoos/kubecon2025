# Speakers
* Liz Rice
* Nega Aggarwal
# Context
* Security is based on pod labels and namespace labels
* Two pods in the same namespace with the same label -> share identity
* Cluster security based on one identity in every cluster
# Network performance optimization
* Identity relevant labels -> reduce amount of security identities
* Granular filtering -> precise filters to reduce capturing unneeded data
* Optimize network traffic based on packet size, protocol, request/response or streaming traffic, encryption
	* Minimize processing by only letting the traffic pass through the network once instead of twice
	* Reduce TCP back pressure
		* Use eBPF host routing to optimize network traffic
		* TCP streams in a single stream
		* NetKit devices:
			* No queuing for Ingress and Egress
			* No networking overhead
* Configure Cilium to optimal performance instead of maximum compatibility
### Live demo
* Use Cilium connectivity perf to analyze your network performance and validate settings
	* Live demo in the talk itself (status, performance test results)
* Great demo, highly technical but well explained

# Metadata
#cilium #security #ebpf #networking [[cilium]]