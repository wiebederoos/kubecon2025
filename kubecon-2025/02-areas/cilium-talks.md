# Scalability & security
* Identity relevant labels -> reduce amount of security identities
* Granular filtering -> precise filters to reduce capturing unneeded data
* Optimize network traffic based on packet size, protocol, request/response or streaming traffic, encryption
	* Minimize processing by only letting the traffic pass through the network once instead of twice
	* Reduce TCP back pressure
	* Use eBPF host routing to optimize network traffic



[[cilium]]

#cilium #security #ebpf