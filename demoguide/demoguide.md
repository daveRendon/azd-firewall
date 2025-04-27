[comment]: <> (please keep all comment items at the top of the markdown file)
[comment]: <> (please do not change the ***, as well as <div> placeholders for Note and Tip layout)
[comment]: <> (please keep the ### 1. and 2. titles as is for consistency across all demoguides)
[comment]: <> (section 1 provides a bullet list of resources + clarifying screenshots of the key resources details)
[comment]: <> (section 2 provides summarized step-by-step instructions on what to demo)


[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
### Plan and implement security for public access to Azure resources

<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** Below demo steps should be used **as a guideline** for doing your own demos. Please consider contributing to add additional demo steps.
</div>

[comment]: <> (this is the section for the Tip: item; consider adding a Tip, or remove the section between <div> and </div> if there is no tip)

***
### 1. What Resources are getting deployed
<add a one-paragraph lengthy description of what the scenario is about, and what is getting deployed>

Use case: You have been asked to install Azure Firewall. This will help your organization control inbound and outbound network access which is an important part of an overall network security plan. Specifically, you would like to create and test the following infrastructure components:

A virtual network with a workload subnet and a jump host subnet.
A virtual machine is each subnet.
A custom route that ensures all outbound workload traffic from the workload subnet must use the firewall.
Firewall Application rules that only allow outbound traffic to www.bing.com.
Firewall Network rules that allow external DNS server lookups.

Resource Group and all deployed resources with name and brief functionality within the scenario:

* shutdown-computevm-srv-jump – autoshutdown configuration

* Test-FW01 – Azure Firewall

* shutdown-computevm-srv-work – autoshutdown configuration

* Test-FW01-firewallPolicy/DefaultApp – firewall policies

* Srv-Jump – Virtual Machines

* srv-jump121 – network interface

* Test-FW01- firewall policies

* Srv-Work – Virtual Machine

* srv-work267 – Network Interfaces

* Test-FW-VN/AzureFirewallSubnet – Azure Firewall subnet

* Test-FW-VN/Jump-SN – Virtual Networks

* Test-FW-VN/Workload-SN – Virtual Networks

* Test-FW01-firewallPolicy – Firewall Policies

* Srv-Jump-nsg/RDP – Network Security Group

* eastus-workload-ipgroup-ombqymk – ipGroups

* eastus-infra-ipgroup-ombqymkr3dz – ipGroups

* Test-FW-VN – VirtualNetworks

* Srv-Work-nsg – Network Security Group

* PIP1 – Public IP Address

* Srv-Jump-nsg – Network Security Group

* Firewall-route – Route Table

* PIP2 – Public IP Address

* Srv-Jump-PIP – Public IP Address

<add a screenshot of the deployed Resource Group with resources>

<img src="https://raw.githubusercontent.com/daverendon/azd-tdd-starter/refs/heads/main/demoguide/azd-fw-rg.png" alt="Resource Group" style="width:70%;">
<br></br>

<br></br>

### 2. What can I demo from this scenario after deployment

This scenario is based on and aligned with the Microsoft Certification: AZ-500: Microsoft Azure Security Technologies.

This scenario creates the following infrastructure components:

 - A virtual network with a workload subnet and a jump host subnet.
 - A virtual machine is each subnet.
 - A custom route that ensures all outbound workload traffic from the workload subnet must use the firewall.
 - Firewall Application rules that only allow outbound traffic to www.bing.com.
 - Firewall Network rules that allow external DNS server lookups.

![Azure Firewall Architecture](az-fw.png)

[comment]: <> (this is the closing section of the demo steps. Please do not change anything here to keep the layout consistant with the other demoguides.)
<br></br>
***
<div style="background: lightgray; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** This is the end of the current demo guide instructions.
</div>



