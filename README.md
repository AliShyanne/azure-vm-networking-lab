# Azure Virtual Machine Networking Lab

---

## Overview
Designed and deployed a cloud-based virtual network in Microsoft Azure to simulate a real-world IT environment. This project focuses on virtual machine provisioning, network configuration, secure remote access, and resource management within a live cloud infrastructure.

The environment demonstrates how cloud systems are built and managed, including networking, access control, and connectivity between resources.

---

## Objective
- Understand Azure cloud infrastructure and virtual networking  
- Deploy and configure virtual machines in a secure environment  
- Implement networking rules and access controls  
- Simulate real-world system administration tasks in the cloud  

---

## Azure Environment

### Resources Created:
- Resource Group (logical container for all resources)
- Virtual Network (VNet)
- Subnet configuration
- Network Security Group (NSG)
- Virtual Machine (Windows Server)

---

## Network Architecture

The environment consists of:

- A Virtual Network (VNet) for internal communication  
- A Subnet to segment the network  
- A Virtual Machine hosted inside the subnet  
- A Public IP for remote access  
- A Network Security Group (NSG) to control inbound/outbound traffic  

---

## Implementation Process

### ### 1. Resource Group Creation
- Created a resource group to organize and manage all Azure resources  
- Ensures centralized management and easier cleanup  

---

### ### 2. Virtual Network Setup
- Configured a Virtual Network (VNet)  
- Defined IP address space for internal communication  
- Created subnet for VM placement  

---

### ### 3. Virtual Machine Deployment
- Deployed a Windows Server VM  
- Selected region, size, and OS image  
- Configured admin credentials  

---

### ### 4. Networking Configuration
- Assigned Public IP for remote access  
- Connected VM to the VNet and subnet  
- Attached Network Security Group  

---

### ### 5. Network Security Group (NSG)
Configured inbound rules:

- Allowed RDP (Port 3389) for remote access  
- Controlled traffic flow for security  

---

### ### 6. Remote Access (RDP)
- Connected to VM using Remote Desktop Protocol  
- Verified successful login and system access  

---

### ### 7. System Configuration
Inside the VM:
- Verified network connectivity  
- Explored system settings and server environment  
- Prepared environment for future services (AD, DNS, etc.)

---

## Technologies Used
- Microsoft Azure  
- Virtual Machines (IaaS)  
- Virtual Networking (VNet, Subnets)  
- Network Security Groups (NSG)  
- Remote Desktop Protocol (RDP)  
- Windows Server  

---

## Key Configurations

### ### Virtual Network
- Defined IP address space  
- Created subnet for isolation  

### ### Virtual Machine
- Windows Server deployment  
- Assigned public and private IP  

### ### Security
- NSG rules for controlled access  
- Restricted traffic to required ports only  

---

## Thought Process

This project was designed to replicate how real cloud environments are built:

- Structure first: Resource groups and VNets organize everything logically  
- Security first: NSGs ensure only required access is allowed  
- Connectivity: Ensured proper communication between resources  
- Validation: Tested access through RDP to confirm full functionality  

Instead of just deploying a VM, the focus was on building a functional, secure cloud environment from scratch.

---

## Testing & Verification
- Verified successful VM deployment  
- Confirmed RDP connectivity  
- Validated NSG rules allowed proper access  
- Ensured network communication within the VNet  

---

## Results
Successfully deployed a fully functional Azure virtual environment with secure remote access and properly configured networking.

This setup demonstrates foundational cloud engineering and system administration skills.

---

## Skills Demonstrated
- Cloud infrastructure deployment (Azure)  
- Virtual networking and subnetting  
- Security configuration (NSGs)  
- Remote system access (RDP)  
- Resource organization and management  
- Troubleshooting connectivity issues  

---

## Screenshots

---

## Outcome
Built and validated a cloud-based virtual machine environment that mirrors real-world infrastructure, demonstrating the ability to deploy, secure, and manage systems in Microsoft Azur
