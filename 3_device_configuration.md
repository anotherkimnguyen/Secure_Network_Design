**3. Device Configuration**

- **Introduction**  
  Key devices like switches, routers, and servers are configured with security in mind, adhering to best practices such as strong passwords, encryption, and remote authentication via RADIUS.

- **Detailed Reasoning**
  - **Layer 3 Switches for Inter-VLAN Routing:** Instead of traditional routers, Layer 3 switches handle inter-VLAN routing, providing faster performance and reducing the number of devices needed.
  - **DHCP Server:** The DHCP server is configured with scopes for each VLAN. By assigning IP addresses automatically, the DHCP server simplifies device configuration and makes network management easier.
  - **DNS Server:** Configuring a DNS server ensures name resolution for internal resources, simplifying network navigation for users.
  
- **Security Focus**
  - **ACL Implementation:** Access Control Lists (ACLs) are applied to restrict traffic between VLANs based on predefined policies. For example, Production VLAN traffic is blocked from accessing Management VLAN resources unless explicitly allowed.
  - **RADIUS Authentication:** Centralized authentication using RADIUS ensures that users need to authenticate through a secure server before accessing network devices. This adds an extra layer of security, especially for sensitive sectors.
