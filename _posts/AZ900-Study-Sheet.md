<h2>Describe cloud concepts (25–30%)</h2>

__Describe cloud computing__

- Define cloud computing

  - Cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale. You typically pay only for cloud services you use, helping you lower your operating costs, run your infrastructure more efficiently, and scale as your business needs change

- Describe the shared responsibility model

  - The workload responsibilities vary depending on whether the workload is hosted on Software as a Service (SaaS), Platform as a Service (PaaS), Infrastructure as a Service (IaaS), or in an on-premises datacenter ***[Microsoft Learn](https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility)***

    - Software as a service
   
      - Identity and directory infrastructure
     
    - Platform as a service
   
      - Identity and directory infrastructure
     
      - Applications
     
      - Network controls

- Define cloud models, including public, private, and hybrid

  - Public cloud model
    
    - Public clouds are the most common type of cloud computing deployment. The cloud resources (like servers and storage) are owned and operated by a third-party cloud service provider and delivered over the internet. With a public cloud, all hardware, software, and other supporting infrastructure are owned and managed by the cloud provider. Microsoft Azure is an example of a public cloud
      - Advantages of public clouds

        - __Lower costs__ - no need to purchase hardware or software, and you pay only for the service you use
       
        - __No maintenance__ - your service provider provides the maintenance
       
        - __Near-unlimited scalability__ - on-demand resources are available to meet your business needs
       
        - __High reliability__ - a vast network of servers ensure against failure
       
        - __Operational expenditure__ (OpEx) - in a public cloud you pay for the resources that you use
    
  - Private cloud model
    
    - A private cloud consists of cloud computing resources used exclusively by one business or organization. The private cloud can be physically located at your organization’s on-site datacenter, or it can be hosted by a third-party service provider. But in a private cloud, the services and infrastructure are always maintained on a private network and the hardware and software are dedicated solely to your organization. (Financial institutions)
   
      - Advantages of a private cloud
     
        - __More flexibility__ - your organization can customize its cloud environment to meed specific business needs
       
        - __More control__ - resources are not shared with others, so higher levels of control and privacy are possible
       
        - __More scalability__ - private clouds often offer more scalability compared to on-premises infrascructure
       
        - __Captial expenditure__ (CapEx) - in a private cloud you pay up front for your resources
    
  - Hybrid cloud model
    
    - A hybrid cloud is a type of cloud computing that combines on-premises infrastructure—or a private cloud—with a public cloud. Hybrid clouds allow data and apps to move between the two environments.
   
      - Advantages of a hybrid cloud
     
        - __Control__ - your organization can maintain a private infrastructure for sensitive assets or workloads that require low latency
       
        - __Flexibility__ - you can take advantage of additional resources in the public cloud when you need them
       
        - __Cost-effectiveness__ - with the ability to scale to the public cloud, you pay for extra computing power only when needed
       
        - __Ease__ - transitioning to the cloud doesn't have to be overwhelming because you can migrate gradually, phasing in workloads over time

- Identify appropriate use cases for each cloud model
  
  - Public cloud
 
    - Web-based email, online office applications, storage, and testing and development environments
    
  - Private cloud
 
    - Government agencies, financial institutions, any other mid- to large-sized organications with business-critical operations seeking enhanced control over their environment
 
  - Hybrid cloud
 
    - Companies which seek the best of both worlds, with a demand for scalability, flexibility, and security in mind

- Describe the consumption-based model

  - The consumption-based model is a pricing model used in the cloud so that customers are only charged based on their usage

- ***[Compare cloud pricing models](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/operating-model/compare)***

  - Pay-as-you-go
 
    - Allows you to pay for Azure services based on your usage with no upfront commitment
   
    - Allows you to start and stop services whenever you want without changing your business needs
   
    - Variable cost depending on your usage
   
    - Good for development and testing environments, and businesses that prefer operational expenditure
 
  - Spot pricing
 
    - Allows you to take advantage of un-used Azure capacities
   
    - Azure is able to evict your virtual machines at any time
   
    - It is cost effective as you are able to pay what you want (setting an upper limit on what you're willing to pay), but has no guarentees
   
    - Good for things that don't require a constant and reliable instance such as, batch processing, data analysis, and for development testing
 
  - Reserved instances
 
    - Allow users to commit to a specific virtual machine type and size for a fixed term
   
    - Discounted pricing is provided due the the term reservation
   
    - Offers predictable billing, but in turn it is less flexible that pay-as-you-go
   
    - Good for long term projects that require predictable resource requirements

>Describe serverless

__Describe the benefits of using cloud services__

>Describe the benefits of high availability and scalability in the cloud

>Describe the benefits of reliability and predictability in the cloud

>Describe the benefits of security and governance in the cloud

>Describe the benefits of manageability in the cloud

__Describe cloud service types__

>Describe infrastructure as a service (IaaS)

>Describe platform as a service (PaaS)

>Describe software as a service (SaaS)

>Identify appropriate use cases for each cloud service type (IaaS, PaaS, and SaaS)

<h2>Describe Azure architecture and services (35–40%)</h2>

__Describe the core architectural components of Azure__

>Describe Azure regions, region pairs, and sovereign regions

>Describe availability zones

>Describe Azure datacenters

>Describe Azure resources and resource groups

>Describe subscriptions

>Describe management groups

>Describe the hierarchy of resource groups, subscriptions, and management groups

__Describe Azure compute and networking services__

>Compare compute types, including containers, virtual machines, and functions

>Describe virtual machine options, including Azure virtual machines, Azure Virtual Machine Scale Sets, availability sets, and Azure Virtual Desktop

>Describe the resources required for virtual machines

>Describe application hosting options, including web apps, containers, and virtual machines

>Describe virtual networking, including the purpose of Azure virtual networks, Azure virtual subnets, peering, Azure DNS, Azure VPN Gateway, and ExpressRoute

>Define public and private endpoints

__Describe Azure storage services__

>Compare Azure Storage services

>Describe storage tiers

>Describe redundancy options

>Describe storage account options and storage types

>Identify options for moving files, including AzCopy, Azure Storage Explorer, and Azure File Sync

>Describe migration options, including Azure Migrate and Azure Data Box

__Describe Azure identity, access, and security__

>Describe directory services in Azure, including Microsoft Entra ID and Microsoft Entra Domain Services

>Describe authentication methods in Azure, including single sign-on (SSO), multi-factor authentication (MFA), and passwordless

>Describe external identities in Azure, including business-to-business (B2B) and business-to-customer (B2C)

>Describe Microsoft Entra Conditional Access

>Describe Azure role-based access control (RBAC)

>Describe the concept of Zero Trust

>Describe the purpose of the defense-in-depth model

>Describe the purpose of Microsoft Defender for Cloud

<h2>Describe Azure management and governance (30–35%)</h2>

__Describe cost management in Azure__

>Describe factors that can affect costs in Azure

>Compare the pricing calculator and the Total Cost of Ownership (TCO) Calculator

>Describe cost management capabilities in Azure

>Describe the purpose of tags

__Describe features and tools in Azure for governance and compliance__

>Describe the purpose of Microsoft Purview in Azure

>Describe the purpose of Azure Policy

>Describe the purpose of resource locks

__Describe features and tools for managing and deploying Azure resources__

>Describe the Azure portal

>Describe Azure Cloud Shell, including Azure Command-Line Interface (CLI) and Azure PowerShell

>Describe the purpose of Azure Arc

>Describe infrastructure as code (IaC)

>Describe Azure Resource Manager (ARM) and ARM templates

__Describe monitoring tools in Azure__

>Describe the purpose of Azure Advisor

>Describe Azure Service Health

>Describe Azure Monitor, including Log Analytics, Azure Monitor alerts, and Application Insights
