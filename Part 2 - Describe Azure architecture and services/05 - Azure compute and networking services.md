# Azure Virtual Machines (VMs) – Notes

## What is an Azure VM?
- Virtual server hosted in Azure
- Part of IaaS (Infrastructure as a Service)
- Full control over OS and software
- Azure manages hardware, you manage OS & apps

## When to Use VMs
- Need OS-level control
- Custom or legacy software
- Lift-and-shift scenarios
- Disaster recovery

## VM Images
- Templates used to create VMs
- Include OS + optional software
- Marketplace images or custom images

## Scaling VMs

### Virtual Machine Scale Sets (VMSS)
- Group of identical VMs
- Automatic scaling based on demand
- Built-in load balancer
- Centralized configuration and updates

### Use Cases for Scale Sets
- Web servers
- APIs
- Big data
- Container workloads

## High Availability

### Availability Sets
- Prevents downtime from failures
- No additional cost

#### Update Domains
- VMs updated in batches
- One batch at a time
- 30-minute recovery gap

#### Fault Domains
- VMs spread across physical hardware
- Different power and network sources
- Protects against hardware failure

## Common Use Cases
- Testing & development
- Running cloud applications
- Extending on-prem datacenter
- Disaster recovery

## Lift and Shift
- Move physical server to Azure VM
- Minimal changes
- You still manage OS and software

## VM Resources
- Size: CPU, RAM
- Storage: HDD/SSD disks
- Networking: VNet, IPs, ports


---

# Azure Virtual Desktop (AVD) – Notes

## What is Azure Virtual Desktop?
- Desktop and application virtualization service
- Runs Windows desktops in Azure
- Users access remotely from any device
- Desktop & apps run in the cloud

## Key Benefits
- Access from anywhere
- Works across OS and devices
- Centralized management
- High security

## Security Features
- Microsoft Entra ID authentication
- Multi-Factor Authentication (MFA)
- Role-Based Access Control (RBAC)
- Data and apps stay in Azure
- Reduced data leakage risk
- Isolated user sessions

## Multi-Session Windows
- Windows 10/11 Enterprise multi-session
- Multiple users share a single VM
- Lower cost and better resource utilization
- Better app compatibility than Windows Server

## User Experience
- Full desktop or specific apps
- Familiar Windows environment
- No dependency on local device power

## Common Use Cases
- Remote work
- BYOD environments
- Secure access to internal apps
- Temporary or contract workers

## Mental Model
- Azure VM = Server in the cloud
- Azure Virtual Desktop = Desktop in the cloud
- AVD is Desktop as a Service (DaaS)


---


# Azure Containers – Notes

## Why Containers?
- VMs are limited to one OS per machine
- Containers allow multiple apps on one OS
- Lower cost, faster scaling

## What are Containers?
- Lightweight virtualization
- Package app + dependencies
- Share host OS
- No OS management required

## Containers vs Virtual Machines
- VM: Full OS, heavier, slower
- Container: No OS, lightweight, fast
- Containers start/stop in seconds

## Docker
- Popular container engine
- Azure supports Docker containers

## Azure Container Services

### Azure Container Instances (ACI)
- Fastest way to run containers
- No VM or OS management
- PaaS offering
- Best for simple workloads

### Azure Container Apps
- Similar to ACI
- Adds load balancing and scaling
- Elastic and easy to use
- No Kubernetes complexity

### Azure Kubernetes Service (AKS)
- Container orchestration service
- Manages container lifecycle
- Best for large-scale systems
- Used in microservices architecture

## Containers & Microservices
- Apps split into small services
- Each service runs in a container
- Independent scaling and updates

## Mental Model
- VM = Virtual Machine (OS-level)
- Container = Application-level isolation



---

# Azure Functions – Notes

## What is Azure Functions?
- Event-driven, serverless compute service
- Runs code only when triggered
- No VM or container management required

## Serverless Computing
- Servers exist but are fully managed by Azure
- No infrastructure visibility
- No cost when idle

## Triggers
- HTTP requests
- Timers
- Queue messages
- Blob uploads
- Service Bus events

## Key Benefits
- Focus only on code
- Automatic scaling
- Pay-per-execution model
- Ideal for variable demand

## Execution Model
- Short-lived tasks
- Runs in seconds
- Resources deallocated after execution

## Stateless Functions
- Default behavior
- No memory of previous executions

## Stateful Functions (Durable Functions)
- Maintain state across executions
- Used for workflows and long-running processes

## Flexibility
- Can move from serverless to other hosting models
- Supports VNets and isolation when needed

## Common Use Cases
- REST APIs
- Event processing
- Automation
- Background jobs
- Lightweight microservices

## Mental Model
- VM = Machine
- Container = Application
- Function = Code
