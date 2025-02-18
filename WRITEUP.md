# Write-up 

###Features of VMs
In terms of costs, there is a benefit of having a lower up front cost compared to having to purchase hardware (IaaS). 
However, in addition to the provisioning and configuration costs, there is an ongoing fee for running and maintaining the VM, as well as, adding more VMs in the case of handling more loads. For scalability of VMs, this is a manual process based on what is needed and scale sets or load balancers can be used. VMs can be set to have high availability by distributing them across multiple fault domains. As far as overall set up, VMs can complex and require more time and expertise of the developer. There is also ongoing maintenance required like security and OS updates.

###Features of App Services
One of the biggest up front benefits of App Services is that is PaaS and fully managed, keeping initial costs low. Overtime, you need to pay for what resources are in use and well as the service plan. There is also auto-scalability which can also help lower costs by scaling resources by demand. The auto-scaling can be either vertical or horizontal. These scaling features can be applied or adjusted easily without having to change code. App Services automatically have availability features like load balancing and failover. You can also configure for zone redundancy. Using an App Service provides you with a fully managed platform, simplifying overall management and deployment. App Services have seamless integration with DevOps tools for CI/CD, can support multiple languages and both Linux or Windows, making this customizable for developers. However, there is limited access to the host server and there are hardware limitations like max memory and vCPU cores per instance.


### Justification
After analysis of both options, for this project, I decided to go with the App Service plan. One factor was that I have little expertise in setting up and VM and would spend less time less time deploying the web app with an App Service (not having to worry about infrastructure). Using App Service allowed for a more straightforward deployment process considering a SQL database, Blob storage needed to be provisioned. I was also able to utilize the integration with GitHub for CI/CD. Overall, for this scenario, App Service provides for a streamlined deployment process and reduces the need for a high level of infrastructure management.


### Considering App Changes
A case where you might need to use a VM over an App Service might be if there is an need for full control of the OS. Maybe there is a need to install custom software or you working with complex legacy apps. Another reason could be the case where there are specific security requirements calling for dedicated hardware. I would use a VM if there were stricter requirements around infrastructure, security, software, and OS configurations.
