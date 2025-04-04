# Speakers
* Kush Trivedi
* Joe Brinkman
# Context / use case
* Being able to migrate 600+ micro-services to ArgoCD
* LinkerD -> K8S Gateway API -> ArgoCD
## Environment setup
* Heavy focus on ArgoCD / seamless deployments
* Gateway API for East <> West traffic
	* Switching between canary and stable rollouts
* Traffic management to control heavy traffic
* ArgoCD rollouts for blue/green canary deployments
* Architecture picture: see screenshot
## Developer enablements
* Use custom ArgoCD plugin to visualize workflow / canary
* Create deployment templates to hide servicemesh & LinkerD configuration
	* Canary configuration & Deployment status
## Demo
* Custom plugin: gradual tweak weight % for canary & stable deployment to verify the integrity / stability of the deployment
# Comments
* Earn-in offers Earned Wages to 4+ million customers through an app 
* Story difficult to follow

#gateway-api #linkerd #progressive-delivery

[[gateway-api]]