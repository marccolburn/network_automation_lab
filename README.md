Network Automation Lab
======================
Create network automation lab in oVirt for testing various playbooks/scenerios.

This lab will provide an environment consisting of a mock service provider, data center, and branch office. The goal is to create scenerios around various automation concepts that apply to this environment.

Playbooks
---------
full_topology_lab.yml - will spin up networking and virtual machines within oVirt based on vars within vars/folder

Requirements
------------
* Ansible 2.9
* RAM ~ 46GB
* vCPUS ~ 29
* Templates for each of the VNF types

Caveats
-------
* ovirt_create_vms will not overwrite NIC profile if already assigned in template, (Recommend removing NICs from template and then assigning at creation)

Diagrams
--------
## Network Automation Lab Physical Overview
![Physical Overview](/images/network_automation_lab_physical_overview.svg)
## Network Automation Lab Logical with Addressing
![Logical Overview](/images/network_automation_lab_logical_with_addressing.svg)
## Network Automation Lab Routing Overview 
![Routing Overview](/images/network_automation_lab_routing_overview.svg)
## Network Automation Lab vSwitch Overview
![vSwitch Overview](/images/network_automation_lab_vswitch_overview.svg)
