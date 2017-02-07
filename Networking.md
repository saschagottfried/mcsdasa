# Networking
Networking is one of the primary building blocks of Microsoft Azure (Azure)

Objectives

After completing this module, you will be able to:

- Plan virtual networks in Azure.
- Implement and manage virtual networks.
- Configure intersite connectivity with virtual networks in Azure.
- Configure networking components.
- Plan virtual networks in infrastructure as a service (IaaS) version 1 (v1).


## Overview

Network Security Groups
- feature for ARM based resources

user defined routes
- default gateway is set by Azure

regional VNets


cross-premise/cross-site network connectivity
- point-to-site VPN
- site-to-site VPN
- ExpressRoute
  - provide a private connection from your datacenter to an Azure virtual network, through a connection service provider. This can improve security and achieve higher bandwidth, lower latency, and better reliability.
  
  
reserved IP
- statische Public IP des IAAS Cloud Service - opposed to virtual IP (VIP)

IP addressing in virtual networks

For VMs that need direct access from the Internet, you can configure public IP addresses. Public IP addresses are allocated dynamically when you create a VM, and are bound to the NICs. You also can configure static public IP addresses and associate them to a load balancer, application gateway or a network interface card of the VM


Subnets

Within each subnet, the first three IP addresses and the last IP address are reserved, and you cannot use them for VMs or cloud services. The smallest subnets that are supported use a 29-bit subnet mask.

DNS

- ARM: resources created in the same virtual network and deployed with Azure Resource Manager (ARM) share the same DNS suffix;therefore, in most cases name resolution by using FQDN is not required. 
- ASM: For virtual networks that are deployed by using the Azure classic deployment model, the DNS suffix is shared among VMs that belong to the same cloud service. Therefore, name resolution between VMs that belong to different cloud services in the same virtual network require the use of FQDN.


## Selecting private address spaces

These three address spaces are commonly used in the Azure VNets.

- 10.0.0.0/8. Includes all addresses from 10.0.0.1 to 10.0.0.255
- 172.16.0.0/12. Includes all addresses from 172.16.0.1 to 172.31.255.255
- 192.168.0.0/16. Includes all addresses from 192.168.0.1 to 192.168.255.255

CIDR notation

| CIDR notation | Range                 | Potential Addresses | Avail. in Azure |

| 10.0.0.0/24 | 10.0.0.0 to 10.0.0.255  | 256                 | 251   |


## Azure DNS



# Lesson 3


## Intersite connectivity options

- VNet-to-VNet (connect VNets in multiple regions or subscriptions) - as opposed to VNet peering
- Site-to-site (cloud <--> on-premise)


Virtual gateways
- prefer dynamic gateways (route-based)
- older static gateways use IKE1 protocol
  - no VNet
  - only a single connection


