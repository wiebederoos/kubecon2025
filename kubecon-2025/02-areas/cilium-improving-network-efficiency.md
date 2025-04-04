# Speakers
* Tamilmani Manoharan
* Will Daly
# Context: integrate Cilium setup with eBPF & Azure Overlays
## Environment setup
* Two nodes: Native Routing & a tunnel based connection between them
* Using Azure Overlay feature

## Use case: Cilicium manages Azure IPAM 
* Challenges:
	* Legacy stack is not scalable for container networking
	* Vendor specific code incorporated in Cillium code-base
	* Cost specific and maintenance responsibilities
	* Various other risks wrt scaling / performance
* Solution:
	* Delegated IPAM with Azure overlays
		* Simple flow: control Plane -> Kubelet -> ContainerD -> CNI plugin -> IPAM plugin
		* azure-ipam -> azure-cns <> nodenetworkconfigs <> delegated network controller
		* Helm chart config:
			* ipam-mode: delegated-plugin (open source)
			* routing-mode: native
			* disable ingress controller
			* disable endpoint health checking
			* CNI custom conf -> true

# Comments
* Very specialized topic, explained well
* Need deeper dive into this and find practical use cases which showcase it

#cilicium #network-traffic #azure #networking #IPAM #CNI
[[cilium]]