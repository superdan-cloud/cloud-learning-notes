# Week 1 – Azure Fundamentals (AZ-900)

## Day 1 – Cloud Concepts
- Cloud computing (my definition): 
    on-demand delivery of resources, compute, storage, networking over the internet
- Key benefits (scalability, elasticity, high availability, global reach, cost):
    Scalability is the ability to increase/decrease resources
    Elasticity automatically scale up/down resources in response to changing demand
    High Avilability is having system resources available when needed regardless of disruptions
    Predictability able to forcase performance and therfore costs
    Goverance are the policies you put in place that say this is how we use the cloud
- CapEx vs OpEx summary:
    CapEx large upfront spending on physical assets
    OpEx ongoing pay as you go spending on services
- Shared responsibility model summary:
    Azure is responsible for the infrastructure and customer is responsible for what goes in the cloud (data, accounts access)
## Day 2 – Cloud Benefits & Economics
- Cloud benefits I remember (with 1 real-world example each):
    Cloud lets you avoid big upfront costs of data center and equipment
- Consumption-based pricing (how I’d explain it):
    You pay for what resources you use

## Day 3 – Architecture Basics
- IaaS: Infrastructure as a Service - Cloud provider is responsible for physical infrastructure, customer manages OS, apps, data
- PaaS: Platform as a Service - Fully managed platform for building and running apps.  Cloud provider responsible for infrastructure, OS, updates.  Customer manages apps, data
- SaaS: Software as a Service - Fully functioning applications.  CLoud provider responsible for almost everything.  Customer manages users and dta
- Who manages what in each model:
- Regions vs Availability Zones vs Region Pairs (my one-liner for each):
    Regions - Geographically located data centers, usually 3, connected together with low-latency networks
    Availability Zones - physcially seperated data centers inside a region for redundancy
    Region Pairs - region paired with another region at least 300 miles away to be isolated from regional disasters
    Sovereign regions - Government 

## Day 4 – Core Azure Services Overview
### Compute
- Virtual Machines – when I’d use them:
    When I need full control over the OS and runtime or lifiting existing app into cloud
- Scale Sets / Availability Sets – what they’re for:
    Scale Sets - VMSS (VM Scale Set) group of VMs that can increase/decrease based on predefined rules.  For load balancing
    Availability Sets - multiple VMs that have identical function but are seperated for fault isolation
- App Service – when I’d choose it over a VM:
    When I want to host we apps or APIs without managing hardware or OS
- Containers (AKS/ACI) – what problems they solve:
    Virtualized environment.  everything the app need to run image
    AKS (Azure Kubernetes Service) - for complex production grade applications
    ACI (Azure Container Service) - for simple, short-lived tasks
- Functions – when “serverless” makes sense:
    good for small event-driven tasks and only pay when its running
- Azure Virtual Desktop – when it’s useful:
    When need windows desktop and applications

### Networking
- Virtual Network (VNet) – my definition:
    logical private network in Azure that lets resournces like VMs and services securely communicate with each other, the Internet, and on-prem networks
- Subnets:
    smaller networks
- VPN Gateway vs ExpressRoute:
    VPN Gateway - used to send encrypted traffic between networks across the public internet
    ExpressRoute - used to send encryped traffic between networks using private connection from ISP to Azure bypassing pubilic Internet
- Public vs private endpoints:
- Anything that still feels a bit fuzzy:

### Databases / Storage (high-level only for now)
- Azure SQL vs Cosmos DB (one sentence each, if mentioned today):
    Azure SQL
    Cosmos DB
- Azure Storage types I’ve seen so far:
    Blobs - text and binary data
    Files - managed file shares
    Queues - messaging store for reliable messaging btw application components
    Disks - Block-level storage volumes for VMs
    Tables - NoSQL table option
