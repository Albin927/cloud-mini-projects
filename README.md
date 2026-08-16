# Azure Cloud Mini Projects

This repository contains 14 Azure and cloud mini projects completed as hands-on practice to build practical skills in Azure networking, virtual machines, storage, security, monitoring, and load balancing.

## Projects

### Project 1 – Azure Virtual Network (VNet)

- Created an Azure VNet with address space `10.0.0.0/16`
- Created frontend and backend subnets
- Practiced Azure VNet and subnet configuration

### Project 2 – Network Security Group (NSG)

- Created separate NSGs for frontend and backend resources
- Associated NSGs with subnets
- Configured inbound rules for RDP (3389) and HTTP (80)

### Project 3 – Application Security Group (ASG)

- Created an Application Security Group for web servers
- Added virtual machines to the ASG
- Configured NSG rules using the ASG for HTTP traffic

### Project 4 – Azure Storage Account and File Share

- Created an Azure Storage Account
- Created an Azure File Share
- Uploaded files and tested file access
- Mounted the Azure File Share on a Windows VM

### Project 5 – Azure Virtual Machine

- Created a Windows virtual machine
- Connected to the VM using RDP
- Installed IIS
- Hosted and tested a basic webpage

### Project 6 – Azure RBAC

- Worked with Azure Role-Based Access Control
- Explored role assignments and resource permissions
- Practiced access management in Azure

### Project 7 – Azure Log Analytics and Monitoring

- Created a Log Analytics workspace
- Explored centralized monitoring and log collection
- Practiced querying monitoring data

### Project 8 – VM to Log Analytics Integration

- Connected an Azure virtual machine to Log Analytics
- Configured monitoring for VM activity
- Explored collected VM logs

### Project 9 – Cross-VNet Connectivity with VNet Peering

- Connected my Azure VNet with a friend's Azure VNet
- Configured VNet peering between the two VNets
- Verified private network connectivity using VM-to-VM communication
- Tested connectivity using private IP addresses

### Project 10 – Azure Internal Load Balancer

- Created an Azure Internal Load Balancer
- Configured a backend pool with multiple virtual machines
- Configured a health probe and load-balancing rule
- Tested internal HTTP traffic distribution using a private frontend IP

### Project 11 – Azure Public Load Balancer

- Created an Azure Public Load Balancer
- Configured a public frontend IP
- Added multiple backend virtual machines
- Configured a TCP health probe on port 80
- Configured an HTTP load-balancing rule
- Tested access through the Load Balancer frontend

### Project 12 – Azure Log Analytics Workspace

- Created and configured a Log Analytics workspace
- Explored Azure Monitor Logs
- Used Kusto Query Language (KQL) to query collected data
- Practiced analyzing events and monitoring information

### Project 13 – VM Security Log Monitoring

- Configured monitoring for Windows VM security logs
- Collected and analyzed Windows security events
- Queried failed login events using KQL
- Used Event ID `4625` to identify failed logon attempts

### Project 14 – Azure Data Collection Rule

- Created an Azure Monitor Data Collection Rule (DCR)
- Configured a Windows data source
- Connected monitoring data collection to the Log Analytics environment
- Practiced collecting and routing VM monitoring data

## Skills Learned

### Azure Networking
- Azure Virtual Network (VNet)
- Subnets
- Network Security Groups (NSGs)
- Application Security Groups (ASGs)
- VNet Peering
- Internal Load Balancer
- Public Load Balancer
- Health Probes
- Load-Balancing Rules

### Azure Compute
- Azure Virtual Machines
- Windows VM administration
- IIS web server
- VM connectivity and testing

### Azure Storage
- Storage Accounts
- Azure File Shares
- File Share mounting

### Azure Security
- Azure RBAC
- NSG security rules
- Windows Security Event Logs
- Failed login monitoring

### Azure Monitoring
- Azure Monitor
- Log Analytics
- Kusto Query Language (KQL)
- Data Collection Rules (DCR)
- VM log collection and analysis

## Repository Structure

Each project is maintained in its own folder with relevant documentation, configuration details, commands, and screenshots where applicable.

```text
azure-cloud-mini-projects/
├── project-1-azure-vnet/
├── project-2-network-security-group/
├── project-3-application-security-group/
├── project-4-azure-storage-file-share/
├── project-5-azure-virtual-machine/
├── project-6-azure-rbac/
├── project-7-azure-log-analytics/
├── project-8-vm-log-analytics-integration/
├── project-9-vnet-peering/
├── project-10-azure-internal-load-balancer/
├── project-11-azure-public-load-balancer/
├── project-12-azure-log-analytics-workspace/
├── project-13-vm-security-log-monitoring/
├── project-14-azure-data-collection-rule/
└── README.md
```

## Conclusion

These projects provide hands-on experience with core Azure services and demonstrate practical understanding of cloud networking, compute, storage, security, monitoring, and traffic management.
