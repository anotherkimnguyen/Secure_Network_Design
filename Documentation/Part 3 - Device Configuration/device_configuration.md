## Part 3 - Device Configuration

Key network devices were configured with security and performance in mind, following best practices for a secure and maintainable network infrastructure:

- **Layer 3 Switches**: These were configured to handle inter-VLAN routing. By routing traffic locally within the switches, we reduced the need for additional routers and improved traffic flow efficiency.
- **DHCP Server**: Configured with multiple scopes, one per VLAN, the DHCP server dynamically assigns IP addresses to client machines, streamlining device configuration across the network.
- **DNS Server**: Provides internal name resolution for resources, simplifying navigation for users by translating domain names to IP addresses within the private network.
- **RADIUS Authentication**: Centralized authentication through the RADIUS server enforces strong user authentication policies for network device access, ensuring only authorized personnel can access critical systems like switches, routers, and servers.

**Documentation**
Configuration Summary for SW-Management<br>
Device Overview:<br>
<br>
Hostname: SW-Management<br>
IOS Version: 15.0<br>
Configuration Size: 2733 bytes<br>
Security Features:<br>
Service Password Encryption:<br>
<br>
Passwords are encrypted for added security.<br>
Enable Secret:<br>
<br>
An encrypted secret password is configured.<br>
Port Security:<br>
<br>
Enabled on all access ports to prevent unauthorized devices from connecting.<br>
Configured on interfaces FastEthernet0/1 to FastEthernet0/6 and FastEthernet0/24.<br>
Spanning Tree Protocol (STP):<br>
<br>
Mode: PVST (Per VLAN Spanning Tree).<br>
System ID extension is enabled.<br>
BPDU Guard is enabled on all access ports to protect against bridging loops.<br>
Storm Control:<br>
<br>
Broadcast storm control set to 5% on all access ports to limit broadcast traffic.<br>
VLAN Configuration:<br>
VLANs Enabled:<br>
VLANs: 10 (Management), 20 (Production), 30 (Study), 40 (Support), 50 (Voice), 99 (Management/Trunk).<br>
Interface Configuration:<br>
Access Ports:<br>
FastEthernet0/1 to FastEthernet0/6:<br>
All configured to access VLAN 10 with port security.<br>
FastEthernet0/24:<br>
Configured for Voice VLAN 50.<br>
Trunk Ports:<br>
GigabitEthernet0/1:<br>
Configured as a trunk port for VLANs 10, 20, 30, 40, 50, and 99.<br>
Native VLAN is set to 99.<br>
GigabitEthernet0/2:<br>
Allowed VLANs: 10, 20, 30, 40, 50, 99, but currently shut down.<br>
Interface States:<br>
All unused interfaces (FastEthernet0/7 to FastEthernet0/23) are administratively shut down.<br>
Line Configuration:<br>
Console Access:<br>
Password secured.<br>
VTY Lines:<br>
Password secured with SSH transport enabled for secure remote access.<br>
