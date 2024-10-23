## Part 3 - Device Configuration

### 1. Introduction
Key devices like switches, routers, and servers are configured with security in mind, adhering to best practices such as strong passwords, encryption, and remote authentication via RADIUS.

### 2. Detailed Reasoning
- **Layer 3 Switches for Inter-VLAN Routing**: Instead of traditional routers, Layer 3 switches handle inter-VLAN routing, providing faster performance and reducing the number of devices needed.
  
- **DHCP Server**: Configured with scopes for each VLAN, the DHCP server simplifies device configuration and network management.

- **DNS Server**: Configuring a DNS server ensures name resolution for internal resources, simplifying network navigation for users.

### 3. Security Focus
- **ACL Implementation**: Access Control Lists (ACLs) restrict traffic between VLANs based on predefined policies.
  
- **RADIUS Authentication**: Centralized authentication using RADIUS ensures secure user access before they can interact with network devices.
