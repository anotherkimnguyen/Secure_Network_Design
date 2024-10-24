## Part 3 - Device Configuration

Key network devices were configured with security and performance in mind, following best practices for a secure and maintainable network infrastructure:

- **Layer 3 Switches**: These were configured to handle inter-VLAN routing. By routing traffic locally within the switches, we reduced the need for additional routers and improved traffic flow efficiency.
- **DHCP Server**: Configured with multiple scopes, one per VLAN, the DHCP server dynamically assigns IP addresses to client machines, streamlining device configuration across the network.
- **DNS Server**: Provides internal name resolution for resources, simplifying navigation for users by translating domain names to IP addresses within the private network.
- **RADIUS Authentication**: Centralized authentication through the RADIUS server enforces strong user authentication policies for network device access, ensuring only authorized personnel can access critical systems like switches, routers, and servers.
