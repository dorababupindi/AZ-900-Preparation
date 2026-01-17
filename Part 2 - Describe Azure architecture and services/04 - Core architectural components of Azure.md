# What is Microsoft Azure?

![Shared Responsibility Model](../Assets/Azure%20Logo.webp)

## Definition (Exam-Friendly)
**Microsoft Azure** is a growing collection of cloud services that helps businesses build, manage, and deploy applications on a global network.

👉 Azure helps handle **current needs** and **future growth** using familiar tools and frameworks.

---

## What Does Azure Offer?

### 1. Limitless Innovation
- Build intelligent apps and solutions
- Use advanced technologies like:
  - Cloud services
  - AI
  - Analytics
- Helps take businesses to the next level

---

### 2. Bring Ideas to Life
- Build on a **trusted cloud platform**
- Use **industry-leading AI and cloud services**
- Helps organizations grow and modernize

---

### 3. Seamlessly Unify
- Manage everything from one platform:
  - Infrastructure
  - Data
  - Analytics
  - AI solutions
- Simplifies platform management
- Improves efficiency and security

---

### 4. Innovate on Trust
- Built on trusted Microsoft technology
- Strong focus on:
  - Security
  - Compliance
  - Responsible cloud usage

---

## What Can I Do With Azure?

- Azure provides **100+ cloud services**
- You can:
  - Run existing applications
  - Build new modern applications
  - Experiment with advanced technologies

---

## Common Starting Point: Virtual Machines (VMs)

- Many teams start cloud adoption by:
  - Moving existing apps to **Azure Virtual Machines**
- This is called **migration**
- Migration to VMs is a good first step

⚠️ But Azure is **more than just running VMs**

---

## Beyond Virtual Machines

Azure also provides:

### Artificial Intelligence (AI) & Machine Learning (ML)
- Apps can:
  - See (vision)
  - Hear (speech)
  - Talk (language)
- Enables smart and interactive applications

---

### Scalable Storage
- Storage grows automatically
- Can handle **huge amounts of data**
- No need to worry about capacity planning

---

## Why Azure is Powerful
- Enables solutions that are:
  - Difficult
  - Expensive
  - Or impossible without cloud computing

---

## One-Line Exam Summary ⭐
> **Azure is a cloud platform with 100+ services that lets you build, run, and manage applications globally, using scalable, secure, and intelligent cloud technologies.**

---
---


# Get Started with Azure Accounts

## Azure Account & Subscription (Key Concept)

- To use **Azure services**, you need an **Azure subscription**
- When you create an **Azure account**, a subscription is automatically created
- One Azure account can have **multiple subscriptions**

### Example:
- One Azure account
  - Subscription for Development
  - Subscription for Testing team
  - Subscription for Production environments

➡ Subscriptions help **organize resources and billing**

---

## Azure Resources

- After creating a subscription, you can create **Azure resources**
- Examples of resources:
  - Virtual Machines
  - Storage
  - Databases
  - Networks

---

## Important Cost Tip ⚠️

- Always complete the **clean-up step** after exercises
- Prevents **unexpected Azure charges**

---

## One-Line Exam Summary ⭐
> **An Azure account contains one or more subscriptions, and subscriptions are used to create and manage Azure resources with proper billing and access control.**

---
---

# Azure Physical Infrastructure

## Core Azure Architecture
Azure architecture is divided into:
- Physical Infrastructure
- Management Infrastructure


---

## Datacenters

- Datacenters are large buildings with servers
- Include:
  - Power supply
  - Cooling systems
  - Networking
- Not directly accessible by customers
- Datacenters are grouped into regions and availability zones

---

## Regions

- A **Region** is a geographical area
- Contains one or more datacenters
- Datacenters in a region are connected with low-latency networks
- Azure balances workloads within a region

### Key Points:
- You choose a region when deploying resources
- Some services are region-specific
- Some services are global (no region needed)

---

## Availability Zones

- Availability Zones are **physically separate datacenters** within a region
- Each zone has:
  - Independent power
  - Independent cooling
  - Independent networking
- Connected by high-speed private fiber networks
- Minimum of **three zones** in zone-enabled regions

### Purpose:
- Improve availability
- Provide fault isolation

---

## Using Availability Zones

- Used for mission-critical applications
- Resources are duplicated across zones
- Improves high availability
- Additional cost may apply

---

## Availability Zone Service Types

### 1. Zonal Services
- Pinned to a specific zone
- Example:
  - Virtual Machines
  - Managed Disks

### 2. Zone-Redundant Services
- Automatically replicated across zones
- Example:
  - Zone-redundant storage
  - SQL Database

### 3. Non-Regional Services
- Always available globally
- Resilient to zone and region failures
- Example:
  - Azure DNS

---

## Region Pairs

- Two regions paired within the same geography
- Located at least 300 miles apart
- Provide disaster recovery
- Automatic failover in some services

### Benefits:
- One region prioritized during large outages
- Updates rolled out one region at a time
- Data stays within the same geography

### Example Region Pairs:
- East US ↔ West US
- Southeast Asia ↔ East Asia

⚠️ Not all services replicate automatically

---

## Sovereign Regions

- Isolated Azure regions
- Used for legal, compliance, and government needs

### Examples:
- US Government regions
- China regions (operated with local partners)

---

## One-Line Exam Summary ⭐
> **Azure physical infrastructure consists of datacenters grouped into regions, availability zones, and region pairs to provide high availability, fault tolerance, and global resiliency.**
