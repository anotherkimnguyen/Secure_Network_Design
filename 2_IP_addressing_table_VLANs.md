**2. IP Addressing Table and VLANs**

- **Introduction**  
  The IP addressing schema is divided by sector to keep network organization clean and efficient. Each sector is assigned a specific subnet, ensuring easy management and troubleshooting.

- **Detailed Reasoning**
  - **Subnetting:** Subnetting allows each VLAN to operate on its own distinct IP range. This segmentation is vital for security (controlling access between sectors) and simplifies the management of network traffic. For instance, management devices are isolated from production, limiting exposure to sensitive resources.
  - **DHCP for Dynamic Address Allocation:** The DHCP server dynamically assigns IPs to devices within each sector. This reduces manual configuration effort and ensures efficient use of IP addresses. By configuring the DHCP server per VLAN, the network can scale up seamlessly.
  
- **Key Considerations**
  - Efficient IP allocation through subnetting ensures there’s no overlap between sectors.
  - The use of DHCP reduces IP configuration errors and manual overhead.
