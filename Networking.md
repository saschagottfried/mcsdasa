# Networking
Networking is one of the primary building blocks of Microsoft Azure (Azure)

Objectives

After completing this module, you will be able to:

- Plan virtual networks in Azure.
- Implement and manage virtual networks.
- Configure intersite connectivity with virtual networks in Azure.
- Configure networking components.
- Plan virtual networks in infrastructure as a service (IaaS) version 1 (v1).


Network Security Groups
- feature for ARM based resources

user defined routes
- default gateway is set by Azure

regional VNets


cross-premise network connectivity
- point-to-site VPN
- site-to-site VPN
- ExpressRoute

reserved IP
- statische Public IP des IAAS Cloud Service - opposed to virtual IP (VIP)

IP addressing in virtual networks

For VMs that need direct access from the Internet, you can configure public IP addresses. Public IP addresses are allocated dynamically when you create a VM, and are bound to the NICs. You also can configure static public IP addresses and associate them to a load balancer, application gateway or a network interface card of the VM


Subnets

Within each subnet, the first three IP addresses and the last IP address are reserved, and you cannot use them for VMs or cloud services. The smallest subnets that are supported use a 29-bit subnet mask.

DNS


- ARM: resources created in the same virtual network and deployed with Azure Resource Manager (ARM) share the same DNS suffix;therefore, in most cases name resolution by using FQDN is not required. 
- ASM: For virtual networks that are deployed by using the Azure classic deployment model, the DNS suffix is shared among VMs that belong to the same cloud service. Therefore, name resolution between VMs that belong to different cloud services in the same virtual network require the use of FQDN.






