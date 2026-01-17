# Describe Cloud Computing

## What is Cloud Computing?
Delivery of computing services over the internet, including:
- Virtual Machines
- Storage
- Databases
- Networking

---

## Shared Responsibility Model
(Applies to On-Prem, IaaS, PaaS, SaaS)

![Shared Responsibility Model](../Assets/shared-responsibility-b3829bfe.svg)

### Cloud Provider is Always Responsible For:
1. Physical data center
2. Physical network
3. Physical hosts

### Customer is Always Responsible For:
1. Information and data stored in the cloud
2. Devices allowed to connect to the cloud
3. Accounts and identities of people, services, and devices in your organization

---

## Cloud Models (4 Models)

1. **Private Cloud**
2. **Public Cloud**
3. **Hybrid Cloud**
4. **Multi-Cloud**

**Important AZURE product names**
### ☁️ Azure Arc
* **What it is:** A bridge that connects "outside" resources to Azure.
* **Simple Definition:** It lets you manage resources running on-premises, AWS, or Google Cloud as if they were running inside Azure.
* **Key Benefit:** You get a "single pane of glass" (one screen) to manage everything, no matter where it lives.

### 🖥️ Azure VMware Solution
* **What it is:** A service that runs your VMware environment inside Azure.
* **Simple Definition:** Move your on-premise VMware workloads to the cloud without rewriting them or changing how you manage them.
* **Key Benefit:** "Lift and shift"—keep using the same VMware tools and skills you already have, but get the scalability of the cloud.

---

## When to Use Which Cloud Model

- **Compliance, full control** → Private Cloud  
- **Pay-as-you-go, scale fast** → Public Cloud  
- **Sensitive + scalable workloads** → Hybrid Cloud  
- **Multiple cloud providers** → Multi-Cloud  

---

## Consumption-Based Model (Cloud)

- Pay-as-you-go
- Consumption-based pricing
- No upfront cost
- Scale up / Scale down
- Only pay for what you use

➡ **Operational Expenditure (OpEx)**

---

## Traditional Model (On-Premises)

- Buy servers upfront
- Fixed capacity
- Hardware lifecycle management

➡ **Capital Expenditure (CapEx)**
