# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

App service is easier and faster than vm because App service(PaaS) don't need much effort managing the underlying operating system such as runtime, middleware and OS. Therefore, deploying my application in App Service would be easier and faster than deploying
it in VM. As I analyze below the costs, scalability, availability and workflow, you will see why choosing App service over VM would be the perfect choice for deploying CMS app in App service.

Costs: App service is less expensive than VM since in app service it has a free plans to deploy and test your app and also has a built-in load balancer which will help you save infrasturcture costs.
For example, VM costs costs $8.45 monthly for 20 hours while in App service it costs $2.00 monthly for 20 hours with even more RAM memory and more storage than VM.

Scalability:
	-Autoscaling: App service come with a built-in service where the VM come with scale sets which need more configurations to set and more time to deploy the application.
	-Load balancer:App service come with an integrated load balancer where in VM need an azure load balancer which need configuration to set.
	-Scale limit:App service can host up to 100 apps where VM support 1000 nodes for single scale set. However, the CMS application that I deploy does not need much scale at this time. So, it would be a good choice to choose app service considering the other advantages that App service provide.   

Availability: App service and VM both provide a SLA and they both available in mutiple regions. 

workflow: App service can be integrated easily with GitHub which people can create a workflow in GitHub repo to build the application and deploy it to azure.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If the application was build in a language other than the ones supported by App Service I dafenately go with VMs. Also, if the application is going to get larger in the future i would 
be choosing VMs over App Services becaue of the limitation of the hardware such memory and CPU. Also, App Service has limit access to underlying OS, so if I my application need for OS to be 
minipulated I have to choose VMs over App Service. 