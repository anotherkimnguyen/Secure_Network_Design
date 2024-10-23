## Part 2 - IP Addressing Table and VLANs

### 1. Introduction
The IP addressing schema is divided by sector, keeping network organization clean and efficient. Each sector is assigned a specific subnet, ensuring easy management and troubleshooting.

### 2. Detailed Reasoning
- **Subnetting**: Subnetting allows each VLAN to operate on its own distinct IP range, controlling access between sectors and simplifying network traffic management.

- **DHCP for Dynamic Address Allocation**: A DHCP server dynamically assigns IPs to devices within each sector, reducing manual configuration effort and ensuring efficient use of IP addresses.

### 3. Key Considerations
- Efficient IP allocation through subnetting ensures no overlap between sectors.
- DHCP reduces IP configuration errors and manual overhead.
