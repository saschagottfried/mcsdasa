# mcsdasa
azure solution architect

# Day1

## Learning Topics & Partner
- azure pass
- skillpipe 
- measureup (use study mode)


## Azure Powershell
- [Quickstart](https://docs.microsoft.com/en-us/azure/azure-resource-manager/powershell-azure-resource-manager)


## Azure Portals
- classic portal
- current portal
- [preview portal](https://preview.portal.azure.com)

## Azure Resource Manager
- [Resource Explorer](https://resources.azure.com)
- [ARM Template Designer](https://armviz.io)


## IAAS v2 virtual machines

Basic parts
- VM
- storage
- network interface

Premium vs. Standard storage account
- standard: billed by usage
- premium: billed by allocated size
  
Storage accounts services
- blobs (block, page, append)
- queue
- table
- file

OS disks
- page blobs
- max size: 1023GB

Data disks
- VM sizes support number
  - [ARM template example](https://github.com/Azure/azure-quickstart-templates/tree/master/101-vm-multiple-data-disk)
- increase capacity: storage spaces, storage pools


VM Sizing

- Basic vs. Standard
  - Standard: support for load balancing, auto scale
- exam: questions on VM sizes


VM costs
- [The Microsoft Azure (IaaS) Cost Estimator Tool](https://www.microsoft.com/en-us/download/details.aspx?id=43376)


Migration of workloads
- .vhd files
- .vhdx not supported
- [sysprep](http://www.utilizewindows.com/introduction-to-sysprep/) required

# Implementing Virtual Machines

VS2015 Developer Machine - run in the cloud
- use market place image
- run on SSD vm sizes




# Managing Virtual Machines

## Availability Set
In general, you want your Azure virtual machine environment to be resilient to hardware failures and maintenance events that might occur occasionally within the Azure infrastructure
- update domains
- fault domains

Examples
- 4 quickstart templates convering Availability Sets

Advanced examples
- [Automating application deployments to Azure Virtual Machines](https://docs.microsoft.com/en-us/azure/virtual-machines/virtual-machines-windows-dotnet-core-1-landing)

Pitfalls
- Add VMs to same VNET (show lock icon - portal feature)
- Add VMs to same availability set


## Scale Sets
- scaling without preprovisionied VMS like in the classic model (ASM)


## Configuration management



Custom script and DSC extensions
- Custom Script for Linux (OMF based)
- Custom Script for Windows (WMF based)

Desired State Configuration
- DSC Extension for Azure 

DSC Example 
- Add Windows server role


## IAAS v1 Networking

All VMs are in same VNET 
- out-of-the-box

Direct communication
- Instance level Public IP 

Endpoint communications
- Static IP (SIP)
- Private IP (PIP)

A cloud service constitutes a logical boundary for virtual machines it contains, offering a number of additional features, including:

- A public IP address and associated Domain Name System (DNS) name in the cloudapp.net DNS namespace.
- Support for endpoints, which you can use to expose individual ports of VMs within the cloud service for external access (from the Internet or other Azure services).
- Automatic name resolution and direct communication between its VMs without the need to use their fully qualified domain names (FQDNs).
- Automatic assignment of private IP addresses to its VMs.

