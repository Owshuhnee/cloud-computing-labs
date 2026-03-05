Module 2 - Compute in the Cloud

Notes: 
Compute refers to the processing power needed to run applications, manage data, and perform calculations.

Amazon Elastic Compute Cloud (Amazon EC2) -
What is an instances - VMs?
Multitenancy - Hypervisor on cloud?
Resizable
Vertical scaling
Networking aspect
COmpute as a service model

on-premises vs cloud resources
Compute time?

Amazon Machine Image (AMI)

What is multi-tenancy in the context of Amazon EC2 instances?

You need to the choose EC2 instance type (how powerful you want it) and the Amazon Machine Image (AMI), which determines the operating system and software for your instance.

Amazon EC2 Instance Types

general purpose
compute optimized
memory optimized
Accelerated computing
storage optimized

# Module 02 — Compute in the Cloud

**Course:** AWS Cloud Practitioner Essentials  
**Focus:** Compute Services  
**Status:** ✅ Ongoing  
**Last Updated:** 2026-03-03  

---

# What is Compute?

**Compute = Processing Power**

Compute refers to the processing power required to:
- Run applications  
- Process data  
- Perform calculations  
- Handle user requests  

---

# Amazon Elastic Compute Cloud (Amazon EC2)

> Amazon EC2 is a cloud service that allows you to rent virtual servers in AWS.

Instead of buying physical hardware, you:
- Launch a virtual server
- Use it
- Pay only for the time it runs

---

## What is an EC2 Instance?

> An **EC2 Instance = A Virtual Machine (VM)**

It behaves like a real computer:
- CPU
- RAM
- Storage
- Operating System
- Networking

But it runs inside AWS data centers.

---

# Multi-Tenancy

> Multiple customers share the same physical hardware securely.

### Apartment Analogy

- One building  
- Many tenants  
- Separate locked apartments  

Everyone shares the structure, but:
- You cannot access your neighbor’s room.

In AWS:
- One physical server  
- Many isolated virtual machines  
- Each belongs to a different customer  

---

# Hypervisor

The **hypervisor** is the technology that makes multi-tenancy possible.

It:
- Divides physical hardware  
- Allocates CPU, RAM, storage  
- Keeps instances isolated  


# Resizable Compute

EC2 instances are **resizable**.

You can:
- Stop an instance  
- Change its size (instance type)  
- Restart it  

You switch based on your needs.

---

# Vertical Scaling

Vertical scaling means:

> Increasing the power of a single instance.

Examples:
- Add more RAM  
- Add more CPU  

---

# Networking in EC2

Each EC2 instance:
- Has a private IP address  
- Can have a public IP  
- Can connect to other instances  
- Can access the internet  

---

# Compute as a Service Model

EC2 follows the **Infrastructure as a Service (IaaS)** model.

You manage:
- Operating system  
- Applications  
- Security inside the instance  

AWS manages:
- Physical hardware  
- Data centers  
- Power and cooling  
- Networking infrastructure  

This follows the **Shared Responsibility Model**.

---

# On-Premises vs Cloud Compute

## On-Premises

You:
- Buy servers  
- Install them  
- Maintain them  
- Replace broken hardware  
- Pay electricity  

Like owning your own factory.

---

## Cloud (AWS)

You:
- Rent servers  
- Launch when needed  
- Stop when done  
- Pay only for usage  

Like renting equipment only when required.

---

# Compute Time

Compute time refers to:

> How long your EC2 instance is running.

AWS charges:
- Per second (in most cases)

---

# Amazon Machine Image (AMI)

An **Amazon Machine Image (AMI)** is a template used to launch an EC2 instance.

It contains:
- Operating system (Linux or Windows)  
- Pre-installed software  
- Configuration settings  

When launching an EC2 instance, you must choose:

1. **Instance Type** → Hardware power  
2. **AMI** → Operating system and software  

3 ways to use AMIs

Create you own
Use available AWS AMIs
Purchase from the marketplace

---

# EC2 Instance Types

Instance types determine how powerful your virtual machine is.

Different families are optimized for different tasks:

- **General Purpose** → Balanced performance  
- **Compute Optimized** → Strong CPU performance  
- **Memory Optimized** → Large RAM capacity  
- **Storage Optimized** → Fast disk performance  
- **Accelerated (GPU)** → Graphics, AI, ML  

### Analogy

Choosing an instance type is like choosing a vehicle:

- Sedan → General use  
- Race car → High CPU performance  
- Truck → Heavy memory workload  
- Delivery van → Storage heavy  

---

# Quick Review (ELI5 Table)

| Term | Simple Meaning |
|------|----------------|
| Compute | Processing power |
| EC2 | Renting a virtual computer |
| Instance | The virtual machine |
| Multi-tenancy | Many customers share hardware securely |
| Hypervisor | Technology that separates VMs |
| Vertical Scaling | Make one machine stronger |
| AMI | OS template |
| Instance Type | How powerful the VM is |
| Compute Time | How long it runs |

---

# Key Exam Reminder

When launching an EC2 instance, you choose:

- **Instance Type** = Hardware power  
- **AMI** = Operating system template  

Think of it like buying a laptop:

- Hardware specs → Instance type  
- Operating system installed → AMI  

---

Application Programming Interface

AWS Management Console
AWS Command Line Interface (CLI)
AWS Software Development Kit (SDK)

Compute and shared responsibility

EC2 Instance types Pricing
- On-demand
- Savings plans
- Reserved Instances
- Spot Instances
- Dedicated Hosts

Scalability refers to the ability of a system to handle an increased load by adding resources

Elasticity is the ability to automatically scale resources up or down in response to real-time demand. 

Amazon EC2 Auto Scaling
Predictive
Dynamic


Elastic Load Balancing (ELB)
Amazon EC2 Auto Scaling

Routing Methods

Round Robin
Distributes traffic evenly across all available servers in a cyclic manner.


Least Connections
Routes traffic to the server with the fewest active connections, maintaining a balanced load.


IP Hash
Uses the client’s IP address to consistently route traffic to the same server.


Least Response Time
Directs traffic to the server with the fastest response time, minimizing latency.

Messaging and Queing