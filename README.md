# ccna-vlan-configuration-lab
Cisco Packet Tracer lab demonstrating VLAN creation and basic port assignments. Includes VLANs setup for CCNA practice with step-by-step IOS commands.

# CCNA VLAN Configuration Lab

This repository contains a Cisco Packet Tracer lab for practicing VLAN configuration as part of CCNA preparation.

## Lab Overview
- **Purpose:** Practice creating VLANs and assigning switch ports.
- **Tool:** Cisco Packet Tracer
- **Devices:** 1 Switch, multiple PCs (adjustable as needed)

## VLANs in this Lab
- VLAN 10 – Sales
- VLAN 20 – HR
- VLAN 30 – IT

## Configuration Steps
Example IOS commands used in this lab:
```cisco
configure terminal
!
vlan 10
 name Sales
vlan 20
 name HR
vlan 30
 name IT
!
interface FastEthernet0/1
 switchport mode access
 switchport access vlan 10
!
interface FastEthernet0/2
 switchport mode access
 switchport access vlan 20
!
end
write memory
