<h1>Describe cloud concepts (25–30%)</h1>

__Describe cloud computing__

>__Define cloud computing__

- Cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale. You typically pay only for cloud services you use, helping you lower your operating costs, run your infrastructure more efficiently, and scale as your business needs change

>__Describe the shared responsibility model__

- The workload responsibilities vary depending on whether the workload is hosted on Software as a Service (SaaS), Platform as a Service (PaaS), Infrastructure as a Service (IaaS), or in an on-premises datacenter ***[Microsoft Learn](https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility)***

  - Software as a service
   
    - Identity and directory infrastructure
     
  - Platform as a service
   
    - Identity and directory infrastructure
     
    - Applications
     
    - Network controls

>__Define cloud models, including public, private, and hybrid__

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

>__Identify appropriate use cases for each cloud model__
  
- Public cloud
 
  - Web-based email, online office applications, storage, and testing and development environments
    
- Private cloud
 
  - Government agencies, financial institutions, any other mid- to large-sized organications with business-critical operations seeking enhanced control over their environment
 
- Hybrid cloud
 
  - Companies which seek the best of both worlds, with a demand for scalability, flexibility, and security in mind

>__Describe the consumption-based model__

- The consumption-based model is a pricing model used in the cloud so that customers are only charged based on their usage

>__***[Compare cloud pricing models](https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/operating-model/compare)***__

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

>__Describe serverless__

- Consumption based/pay-as-you-go meaning it is entirely event driven
 
  - An action must occur to have the serverless technology to be used. Such as writing to a storage account
   
- Azure Functions
 
  - __Coded__ - running code in one of the supported languages
   
  - __Stateless__ - meaning multiple actions will not interact with eachother
   
    - When the action is called, the Azure function begins and by default immediately ends once the task is completed
   
- Durable Azure Functions
 
  - It is possible to create an Azure function that does not immediately end once the task is completed
   
  - The state is maintained between events happening. A scenario would be creating an endpoint that makes an HTTP request and checks in if the action is completed
 
- Azure Logic Apps
 
  - __Low/No code__ - meaning it is connector based (like Power Automate) which calls connections

    - With the Logic Apps Designer, you can build out the process using a GUI
   
  - __Automated__ - automates tasks based on triggers when an event is called

__Describe the benefits of using cloud services__

>__Describe the benefits of high availability and scalability in the cloud__

- High abailability

  - Highly availably cloud environments with uptime guarentees depending on the service
 
    - Guarentees are part of the service-level agreements
   
      - Service-level agreements are a formal agreement that guarentees the customer a stated level of service
     
    - Agreements within Azure are represented as a percentage availability known as up time
   
    - Downtime comes with credits that are due to the customer account
   
    - Each service comes with its own SLA which must be prioritized to make sure it fits your business needs
   
  - Scalability
 
    - The ability to scale means to add more resources to better handle an increase in demand
   
    - __Vertical scaling__ - if you were developing an app and you need more processing power, you could add more CPUs or RAM to the virtual machine
   
      - The ability to add or reduce resources to an existing VM to meet current demands and needs
     
    - __Horizontal scaling__ - if you experience a steep increase in demand, you would be able to either deploy more virtual machines or containers
   
      - The ability to deploy entire VMs or containers which were not previously used in the environment
   
      - Deployed resources couuld be scaled in either automatically or horizontally

>__Describe the benefits of reliability and predictability in the cloud__

- Reliability

  - The ability of a system to recover from failures and continue to function.
 
  - Reliability is a shared responsibility between Microsoft and the end-user
 
  - Azure built-in resilience features
 
    - __Availability zones__ - Run critical workloads across datacenters with independant power, cooling, and networking
     
    - __Availability sets__ - Achieve redundancy within a datacenter by collocating or separating resources
     
    - __Azure traffic manager__ - Implement automatic failover, optimize traffic, and combine on-premises and cloud systems
     
    - __Azure site recovery__ - Replicate on-premises and Azure workloads from a primary site to a secondary location
     
    - __Azure backup__ - Back up data with a simple, secure, and cost-effective recovery and restoration solution
     
    - __Azure storage__ - Create and store multiple copies of your data with redundancy options for any scenario
     
  - Cloud monitoring tools
 
    - __Azure chaos studio__ - Systematically improve resillience with chaos engineering and testing by deliberately introducing faults that simulate real-world outages
     
    - __Azure service health__ - Identify resource issues and resolve them through a customizable dashboard
     
    - __Azure monitor__ - Collect, analyze, and act on telemetry data from Azure and on-premises environments
     
    - __Azure application insights__ - An extensible analytics service that helps you understand the performance and usage of your live web applications
     
    - __Network watcher__ - Monitor, diagnose, and gain insights into your networks performance and health
     
    - __Azure advisor__ - Offers actionable recommendations to help you optimize your Azure resources for reliability, security, operational excellence, performance, and cost

- Predictability

  - Focused on performance predictability or cost predictability
 
  - __Performance__ - predict resources that needed to deliver a positive experience to your customers.
 
    - Autoscaling allows you to deploy additional resources to meet demands, and then scale back when demand drops
   
    - Load balancing allows you to redirect overloaded servers to less stressed areas to allow for more efficient use of resources
   
  - __Cost__ - predict or forcast the cost of your cloud spending through real time tracking of resources, and monitoring of resources to ensure you are using them in the most efficient way
 
    - Data analytics to predict patterns and trends that help better plan resource deployments
   
    - Total Cost of Ownership (TCO) or Pricing Calculator to estimate potential cloud spending

>__Describe the benefits of security and governance in the cloud__

- Security

  - There are cloud solutions that meet your security needs, depending on the cloud service type
    
    - If you want maximum control of security, infrastructure as a service provides you with physical resources but lets your manage the operating systems and installed software, including patches and maintenance
   
    - If you want patches and maintenance taken care of automatically, platform as a service or software as a service deployments may be the best cloud strategy for you
 
  - __Microsoft Defender for Cloud__ - Enabled by default in each subscription, and its recommended that you enable data collection from virtual machines to allow Defender for Cloud to install its agent and begin gathering data
 
    - Provides unified view of security across your workloads
   
    - Collects, searches, and analyzes security data from various sources, which include firewalls and other partner solutions
   
    - Provides actionable security recommendations to fix issues before they can be exploited
   
    - Applies security policies across your hybrid cloud workloads to ensure compliance with security standards

- Governance

  - Cloud features support governance and compliance with set templates to help ensure all your deployed resources meet corporate standards and government regulatory requirements
 
  - Update all your deployed resources to new standards as standards change
 
  - Cloud-based auditing helps flag any resource that's out of compliance with your corporate standards and provides mitigation strategies
 
  - __Azure policy__ - Tool that helps you create, assign, and manage policies which enforce rules on your resources so those resources stay compliant with your corporate standards and service-level agreements
 
    - Enforce tagging for resources and resource groups
   
    - Restrict regions for deployed resources
   
    - Restrict expensive SKUs for specific resources
   
    - Audit the use of important features like Azure-managed disks

>__Describe the benefits of manageability in the cloud__

- Management __of__ the cloud

  - Management of the cloud speaks to managing your cloud resources.
 
    - Automatically scale resource deployment based on need
   
    - Deploy resources based on a preconfigured template, removing the need for manual configuration
   
    - Monitor the health of resources and automatically replace failing resources
   
    - Receive automatic alerts based on configured metrics, so you are aware of performance in real time
   
  - Management __in__ the cloud
 
    - Management in the cloud speaks to how you are able to manage your cloud environment and resources
   
      - Through a web portal
     
      - Using a command line interface
     
      - Using APIs
     
      - Using PowerShell

__Describe cloud service types__

>__Describe infrastructure as a service (IaaS)__

>__Describe platform as a service (PaaS)__

>__Describe software as a service (SaaS)__

>__Identify appropriate use cases for each cloud service type (IaaS, PaaS, and SaaS)__

<h1>Describe Azure architecture and services (35–40%)</h1>

__Describe the core architectural components of Azure__

>__Describe Azure regions, region pairs, and sovereign regions__

>__Describe availability zones__

>__Describe Azure datacenters__

>__Describe Azure resources and resource groups__

>__Describe subscriptions__

>__Describe management groups__

>__Describe the hierarchy of resource groups, subscriptions, and management groups__

__Describe Azure compute and networking services__

>__Compare compute types, including containers, virtual machines, and functions__

>__Describe virtual machine options, including Azure virtual machines, Azure Virtual Machine Scale Sets, availability sets, and Azure Virtual Desktop__

>__Describe the resources required for virtual machines__

>__Describe application hosting options, including web apps, containers, and virtual machines__

>__Describe virtual networking, including the purpose of Azure virtual networks, Azure virtual subnets, peering, Azure DNS, Azure VPN Gateway, and ExpressRoute__

>__Define public and private endpoints__

__Describe Azure storage services__

>__Compare Azure Storage services__

>__Describe storage tiers__

>__Describe redundancy options__

>__Describe storage account options and storage types__

>__Identify options for moving files, including AzCopy, Azure Storage Explorer, and Azure File Sync__

>__Describe migration options, including Azure Migrate and Azure Data Box__

__Describe Azure identity, access, and security__

>__Describe directory services in Azure, including Microsoft Entra ID and Microsoft Entra Domain Services__

>__Describe authentication methods in Azure, including single sign-on (SSO), multi-factor authentication (MFA), and passwordless__

>__Describe external identities in Azure, including business-to-business (B2B) and business-to-customer (B2C)__

>__Describe Microsoft Entra Conditional Access__

>__Describe Azure role-based access control (RBAC)__

>__Describe the concept of Zero Trust__

>__Describe the purpose of the defense-in-depth model__

>__Describe the purpose of Microsoft Defender for Cloud__

<h1>Describe Azure management and governance (30–35%)</h1>

__Describe cost management in Azure__

>__Describe factors that can affect costs in Azure__

>__Compare the pricing calculator and the Total Cost of Ownership (TCO) Calculator__

>__Describe cost management capabilities in Azure__

>__Describe the purpose of tags__

__Describe features and tools in Azure for governance and compliance__

>__Describe the purpose of Microsoft Purview in Azure__

>__Describe the purpose of Azure Policy__

>__Describe the purpose of resource locks__

__Describe features and tools for managing and deploying Azure resources__

>__Describe the Azure portal__

>__Describe Azure Cloud Shell, including Azure Command-Line Interface (CLI) and Azure PowerShell__

>__Describe the purpose of Azure Arc__

>__Describe infrastructure as code (IaC)__

>__Describe Azure Resource Manager (ARM) and ARM templates__

__Describe monitoring tools in Azure__

>__Describe the purpose of Azure Advisor__

>__Describe Azure Service Health__

>__Describe Azure Monitor, including Log Analytics, Azure Monitor alerts, and Application Insights__
