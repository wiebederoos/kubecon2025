# Speakers
* Luigi Zhou

# Context
* Run millions on jobs for ML based topics
* Scale from 100 nodes to 1000 to support upcoming demand
## Why Cilium
* High performance networking
* Enhanced observability -> rich pod identity
* Granular policies -> fine tuned network control
* Future proof since using eBPF

# 3 stories
## Environment setup
* On prem / air gapped
* Bare metal
* Custom build# 3 stories
## 1 - Map pressure
* See screenshot -> what's a Map
* Explanation Policy Maps wrt identity, direction, protocol, port and verdict
	* Instruct Armada to use only relevant labels (namespace as security boundary is not sufficient here)
## 2 - Conntrac
* See screenshot -> what's Conntract (Connection Tracking)
* CNI related errors
	* Unable to remove proxy redirects -> context cancelled before proxy updates
	* Improper garbage collection since by default its dynamic, based on how many entries are removed in the last interval
		* This results in incorrect GC intervals so old connections are not cleaned up in time
		* Set Max interval to 10 min instead of several hours (default, when not setting it and getting CNI related errors)
## 3 - Bonus (make Cilium to use 1TB of memory)
* Never switch off GOC (the load will slowly build up)
# Comments

[[cilium]]
#cilium #security #ebpf #networking


