# Plan and implement security for public access to Azure resources

👉 https://blog.azinsider.net/56a7b72025ce?source=friends_link&sk=cf85213a66dae0e202491717f51a9c6f

### Use case

You have been asked to install Azure Firewall. This will help your organization control inbound and outbound network access which is an important part of an overall network security plan. Specifically, you would like to create and test the following infrastructure components:

A virtual network with a workload subnet and a jump host subnet.
A virtual machine is each subnet.
A custom route that ensures all outbound workload traffic from the workload subnet must use the firewall.
Firewall Application rules that only allow outbound traffic to www.bing.com.
Firewall Network rules that allow external DNS server lookups.

## Solution Overview 

This scenario is based on and aligned with the Microsoft Certification: AZ-500: Microsoft Azure Security Technologies.

This scenario creates the following infrastructure components:

 - A virtual network with a workload subnet and a jump host subnet.
 - A virtual machine is each subnet.
 - A custom route that ensures all outbound workload traffic from the workload subnet must use the firewall.
 - Firewall Application rules that only allow outbound traffic to www.bing.com.
 - Firewall Network rules that allow external DNS server lookups.

![Azure Firewall Architecture](az-fw.png)
