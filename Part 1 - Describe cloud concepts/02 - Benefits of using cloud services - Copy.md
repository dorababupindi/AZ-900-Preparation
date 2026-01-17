# Describe the Benefits of Using Cloud Services

## Two Important Considerations for Any Cloud Application
1. **Uptime (Availability)**
2. **Ability to Handle Demand (Scale)**

---

## High Availability

Azure provides **Service Level Agreements (SLA)**, represented in percentages.

### SLA Examples

- **SLA = 100%**
  - No downtime at all
  - Ideally **not achievable**

- **SLA = 99%**
  - Unavailable for **1.68 hours per week**
  - Or **7.2 hours per month**

- **SLA = 99.9%**
  - Unavailable for **10 minutes per week**
  - Or **43.2 minutes per month**

---

## Scalability

Ability to adjust resources to meet demand.

### Types of Scaling

#### 1. Vertical Scaling (Scale Up / Scale Down)
- **Meaning**: Increase or decrease power of a single resource
- **What changes**: CPU, RAM size
- **Azure term**: Scale up / Scale down
- **Speed**: Slower (may require restart)
- **Downtime risk**: Possible downtime
- **Limit**: Has maximum hardware limit
- **Cost**: Increases sharply
- **Best for**: Small apps, legacy systems
- **High availability**: Not very ideal

#### 2. Horizontal Scaling (Scale Out / Scale In)
- **Meaning**: Increase or decrease number of resources
- **What changes**: Number of VMs / instances / containers
- **Azure term**: Scale out / Scale in
- **Speed**: Faster
- **Downtime risk**: Usually no downtime
- **Limit**: Virtually unlimited
- **Traffic handling**: Increases gradually
- **Best for**: High traffic, cloud-native apps
- **High availability**: Very good

---

## Reliability

- System should **not fall apart when something breaks**
- Azure regions have **Availability Zones**
- If **Zone A fails**, traffic shifts to **Zone B**
- Azure handles this **automatically**

---

## Predictability

### 1. Performance Predictability
- App should not slow down when users increase
- Example: Sudden API spikes
- Cloud automatically adds instances
- Load balancer distributes traffic
- When traffic drops, instances are removed

### 2. Cost Predictability
- Identify:
  - Idle VMs
  - Oversized SQL Databases
  - Unused storage
- Adjust resources **before billing explodes**

### Azure Tools for Predictability
- Pricing Calculator
- TCO Calculator
- Monitoring and Analytics

---