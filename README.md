# **Vic modern hotel network**

## Overview

This project focuses on designing and implementing a secure, scalable, and structured network for Vic Modern Hotel,
a three-floor hotel with multiple departments. The network ensures reliable communication between departments and stable internet access for staff and guests.

## Network Design

![all](https://github.com/sadeem058/Network_project_tasks/blob/main/all.png)


3 Routers located in the IT department

3 Switches, one for each floor

VLAN segmentation for each department

Wi-Fi connectivity for wireless devices

Dedicated printers for departments

**Technologies Used**

VLANs for traffic segmentation and security

OSPF as a dynamic routing protocol

DHCP for automatic IP address assignment

SSH for secure remote router access

Port Security to prevent unauthorized device connections

VLAN & IP Addressing

**First Floor**

- Reception → VLAN 80 → 192.168.8.0/24

- Store → VLAN 70 → 192.168.7.0/24

- Logistics → VLAN 60 → 192.168.6.0/24

**Second Floor**

- Restaurant → VLAN 50 → 192.168.5.0/24

- HR → VLAN 40 → 192.168.4.0/24

- Sales/Finance → VLAN 30 → 192.168.3.0/24

**Third Floor**

- Admin → VLAN 20 → 192.168.2.0/24

- IT → VLAN 10 → 192.168.1.0/24

**Routing & Security**

OSPF configured between routers using /30 subnets

DHCP enabled for all VLANs

SSH enabled on all routers

Port security applied on IT switch using sticky MAC and shutdown violation mode

## Results

Successful communication between all VLANs

![ping first floor](https://github.com/sadeem058/Network_project_tasks/blob/main/ping%20first%20floor.png)
![ping second floor](https://github.com/sadeem058/Network_project_tasks/blob/main/ping%20second%20floor.png)
![sender](https://github.com/sadeem058/Network_project_tasks/blob/main/sender.png)
![recever](https://github.com/sadeem058/Network_project_tasks/blob/main/recever.png)

Stable and efficient routing between floors

Automatic IP assignment via DHCP

Secure remote access using SSH

Unauthorized device access successfully blocked

## Conclusion

The Vic Modern Hotel network was successfully implemented using modern networking techniques.
The design ensures high performance, scalability, and strong security, making it suitable for real-world hotel environments.
