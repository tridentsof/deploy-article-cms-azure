# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

-----------------------
**My Answer:**

*1. Analyze costs, scalability, availability, and workflow:*

||Virtual Machine|App Service|
|-----------|-----------|-----------|
|**Cost Analysis**|Pay-as-you-go based on usage, more expensive than App Service|Pay-as-you-go based on usage, generally more cost-effective than VMs for hosting web applications and APIs|
|**Scalability**|Scalable through vertical and horizontal scaling, can be customized to meet specific needs|Scalable through vertical and horizontal scaling, limited customization options|
|**Availability**|High availability through availability sets and virtual machine scale sets|High availability through regional distribution, automatic load balancing, and automatic scaling|
|**Workflow**|Provides full control and flexibility, requires more management and maintenance|Provides a managed platform, requires less management and maintenance|


*2. Choose the solution: According to me, I would choose the Azure App Service for this application's deployment for the following reasons:*
1. This application has only a few basic functions, and we don't have a need for a high-performance compute service, so we can consider it a light-weight app. In this situation, we can choose the App Service.
2. This application is small, so we head to setup this as fast as we can. At this point, App Service is still faster than Virtual Machine because we don't need to take time to first setup Virtual Machine.

*3. Detail how the app and any other needs would have to change for you to change your decision in the last section:*
- Performance: If my application requires high performance or any specific resource requirements that cannot provide by Azure App Service then I need to switch to using VM to scale vertically with larger VM sizes or orizontally with more VMs.
- Licensing: If my application requires specific software licenses that not including in Azure App Service.
- Customization: If my application requires specific configurations that Azure App Service can not provide, I will switch to using VM to have more control over underlying infrastructure.

