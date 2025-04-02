# Speakers
* Mathieu Benoit
* Kendall Roden

# Context / use case
* Abstracting away the cognitive load wrt infrastructure for developes to focus on consitency, simplicity, productivity
* Finding the balance between developer experience and governance

# Practical example/walkthrough
* Call DAPr API to call Docker workflow based on a local application (using Python and Redis DB)
* Using sidecar deployment model that is hosting the runtime environment
* Register a workflow on runtime
* Creating the structure to execute workflows in the correct order/sequence
* Activities:
	* DAPr client to create and publish messages and tell which k8s component to use
	* Message being delivered to the UI based on a subscription
	* Using state API to fetch state(s)
* Deploy application and promote it through Score - transparently for multiple target environments
# Challenges
* Containerized workloads run all the time?
* Promote from DEV to PROD?
* Learn Docker Compose or K8S manifests?

# Score (abstraction & standardization)
* Specification: intent how to deploy application 
* Concrete implementation
	* Generate manifests for score files
* For both: see screenshot
# Comments
* Great scheme (see screenshot) about internal developer platform enablements
	* Created / uses Internal Platform Maturity Model from CNCF
* Focus on platform interfaces and capabilities
	* DAPr APIs and SDKs + Score Specification
* Need to check out the recording - talk was superfast


