# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

Currently the CMS app is running on an App Service Plan with F1 Free tier. 
This means that the app can run for 60 min/day free of charge, which is sufficient for developing the application. 
The App Service Plan can easily be scaled up to a B1 with 100 ACU which costs €10.47/month. 
100 ACU is approximately the computational power fo an A1 virtual machine, which costs €22.16/month. 
VM's are generally more expensive than App Service Plans. 
Also with the ASP you don't have to manage the OS and configure the VM so it can run the application. 
The Deployment Center of the App Service takes care of the continuous deployment of the application.  
ASP's provides high availability and auto-scaling.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

The ASP has some hardware limits that could influence my choice. The ASP has a maximum of 14GB memory and 4vCPU's. 
When the application and/or the user-base would grow and one of these limits would impose performance limitations,
hosting the application on a VM would be the better option. 
Another reason to switch would be when the application would require more control over the operating system or additional software to be installed. 


