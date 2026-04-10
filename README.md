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

### Azure Virtual Machine – Configuration Details ( azure-virtual-machine-overview.PNG )

Detailed view of the deployed virtual machine within Microsoft Azure.

Key details:
- Virtual Machine: vm-network-lan  
- Operating System: Windows Server 2022 Datacenter (Azure Edition)  
- Public and private IP addresses assigned  
- Connected to a virtual network (VNet) and subnet  
- VM size and resource allocation displayed

This confirms successful deployment and configuration of cloud infrastructure used for the Active Directory environment.

### Windows Server Initial Login ( windows-server-first-login.PNG )

Initial login to the Windows Server virtual machine after deployment.

Details:
- First access to the server via remote connection  
- Default desktop environment before configuration  
- Network discovery prompt indicating fresh system setup  

This represents the starting point before configuring server roles, Active Directory, and system policies.

### Windows Server – Initial Configuration State ( windows-server-manager-initial.PNG )

Initial view of Windows Server Manager before full configuration.

Details:
- Server Manager dashboard prior to full role configuration  
- Indicators showing services and roles not fully configured  
- Starting point before Active Directory Domain Services deployment  

This represents the baseline system state before configuring roles, services, and domain infrastructure.

### Virtual Machine System Verification ( azure-vm-system--verification.PNG )

Verified system configuration and environment details within the virtual machine.

Details:
- Confirmed operating system and system specifications  
- Validated server environment readiness  
- Ensured proper setup before installing server roles  

This step ensures the virtual machine is properly configured before proceeding with Active Directory deployment.

### Active Directory Domain Services (AD DS) Installation (active-directory-role-installation.PNG)

Installed the Active Directory Domain Services role on the Windows Server.

Details:
- Used Server Manager → Add Roles and Features Wizard  
- Selected Active Directory Domain Services (AD DS)  
- Included required management tools (Group Policy Management, AD tools)  
- Prepared server for domain controller promotion  

This step establishes the foundation for centralized identity and access management within the environment.

### Active Directory Domain Deployment (active-directory-domain-deployment.PNG)

Configured the server as a domain controller and created a new Active Directory forest.

Details:
- Promoted server to domain controller  
- Created new forest (e.g., lab.local)  
- Configured domain services and DNS integration  

This step establishes centralized authentication and directory services within the environment.

### Active Directory Organizational Unit Structure (active-directory-ou-structure-initial.PNG)

Created and organized Organizational Units (OUs) to reflect a structured business environment.

Details:
- Created OUs such as HR, IT, Sales, Support, and Workstations  
- Established logical separation of departments  
- Prepared structure for user and policy management  

This enables efficient administration and targeted policy application across the organization.

### Active Directory – Users, Groups, and Organizational Units (active-directory-users-groups-full-view.PNG)

Configured and organized Active Directory with users, groups, and OUs to simulate a real business environment.

Details:
- Created multiple Organizational Units (HR, IT, Sales, Support, Workstations)  
- Added user accounts within respective departments  
- Created security groups for role-based access control  
- Organized resources following a structured hierarchy  

This setup reflects real-world Active Directory administration practices, including user management and access control.

### Group Policy Management – OU Level (

Configured Group Policy Objects (GPOs) and linked them to specific Organizational Units.

Details:
- Created a GPO for workstation management  
- Linked policy to the Workstations OU  
- Enabled centralized policy application  

This allows administrators to enforce configurations and security settings across targeted systems.
---

## Outcome
Built and validated a cloud-based virtual machine environment that mirrors real-world infrastructure, demonstrating the ability to deploy, secure, and manage systems in Microsoft Azure
