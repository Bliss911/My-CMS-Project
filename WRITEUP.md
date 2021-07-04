# Write-up
## Analysis between Azure VM and Azure App service

**Azure Virtual Machine** is Microsoft's IaaS (Infrastructure-as-a-Service) cloud offering. An Azure VM gives you the flexibility of virtualization without having to buy and maintain the physical hardware that runs it. However, you still need to maintain the VM by performing tasks, such as configuring, patching, and installing the software that runs on it.
Azure VMs offer developer more control over the environment ranging from OS to the running application deployed.

**App Service** is Azure App Service is Microsoft's PaaS (Platform-as-a-Service) cloud service by Microsoft. Azure App Service is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. This service takes away some of the additional responsibilities of customer, and gives it back to cloud provider. The developer only needs to deploy the code, and focus only on the development part of project. This is very useful for teams with less manpower, and less experience with managing such hardware.

| Factor |  VM   |  App service  |
|:-------|:-----:|--------------:|
|**1. Cost**| Azure VMs are more expensive to run. | App services are cheaper to run|
|**2. Scalability**| Azure VMs are preferred for apps, which have scope to expand for future.| Vertical or Horizontal scaling|
|**3. Availability**|Multiple VMs can be grouped to provide high availability| High availability, auto-scaling and support of both Linux and Windows environments.|
|**4. Work flow** | Multiple types to choose from, such as compute or memory-optimized VMs, along with varying amounts of CPU, RAM and storage | Developer spends time writing great apps and let Azure worry about the platform.| 

### Choice of deployment
My choice of deployment is the Microsoft **Azure App service**

### Justification of choice of deployment
The following are the reasons for choosing App service deployment
- Easy to deploy
- No cost beyond App Service Plan costs
- Easy way to setup scheduled tasks

### App changes that would change my decision
The major changes that would change my decision would be:
- if the requirements of the app needs more control over the application Infrastructure and OS
- If there is forseeable spike in app traffic which would cause overload in the app deployment. This would require the deployment on Azure VM as azure VMs are best suited for scalability.
- Lastly, if the finance needed to deploy the app are available, then I will opt for the Azure VM.