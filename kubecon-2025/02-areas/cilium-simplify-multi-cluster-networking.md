# Speakers
* Arthur Outhenin-Chalandre
* Marco Iorio

# Use case
* Multi cluster networking -> expand services to use multiple clusters instead of just one

## Context
* Make service Endpoint available to all clusters using an API
* Load balance traffic between multiple clusters using annotations
	* shared -> true (local and remove backends)
	* affinity -> control preferred endpoints
* Pros and cons:
	* Straightforward, fully integrated
	* No standard API, services should be available on all nodes
	* No support for headless services
	* Global services are not enough
## Demo 1
* Based on 3 clusters
	* Enable endpoint slides -> see endpoints on all clusters
	* Load gets distributed across all backends
	* Challenges:
		* Split large endpoints
		* Apply changes in batches
		* ...?
## MCS-API
* Merge all clusters
* Use bar.foo.local.svc.clusterset.local (instead of *cluster.local)
	* Use P1 - P4
	* Split clustersets into multiple clusters referencing all by cluster FQDN
* Tight integration with a lot of technologies
* Supported by Cilium 1.17+
	* Requires MCS-API CRDs
	* Install and enable CoreDNS plugin
## Demo 2
* Showcasing multiple clusters and service endpoints
* Show service import
* Show clustermeshes
* Send requests to multiple cluster service via Gateway API -> get answers from all clusters

# Comments


[[cilium]]

#cilium #security #ebpf #networking