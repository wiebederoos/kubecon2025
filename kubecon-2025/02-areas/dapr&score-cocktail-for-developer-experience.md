# Speakers
* Mathieu Benoit
* Kendall Roden
# Context / use case
* Abstracting away the cognitive load wrt infrastructure for developers to focus on consistency, simplicity, productivity
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
* Overview:
* ![Dapr overview](../attachments/20250402_112300.jpg)
# Challenges
* Containerized workloads run all the time?
* Promote from DEV to PROD?
* Learn Docker Compose or K8S manifests?
# Score (abstraction & standardization)
* Specification: intent how to deploy application 
* Concrete implementation
	* Generate manifests for score files
* For both: see screenshot
	* ![Score overview](../attachments/20250402_113928.jpg)
# Comments
* Great scheme (see screenshot) about internal developer platform enablements
	* Created / uses Internal Platform Maturity Model from CNCF
	* ![Maturity model](../attachments/20250402_112019.jpg)
* Focus on platform interfaces and capabilities
	* DAPr APIs and SDKs + Score Specification
* Need to check out the recording - talk was superfast
* Very useful to lower the stress for developers which should not expand their knowledge even more

# Metadata
#dapr #score #specification #developers


