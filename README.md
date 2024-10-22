## Network Design and Architecture - Summary

This project outlines the design and implementation of a secure, efficient, and scalable network for a client relocating to a new office space. Our goal was to create a structured, robust, and cost-effective network infrastructure that caters to the unique needs of various sectors, including Management, Study, Production, and Support. The project was simulated using **Cisco Packet Tracer** and involved the following key elements:

1. **VLAN Segmentation**:  
   The network is divided into multiple VLANs, each assigned to a specific sector. This segmentation reduces broadcast traffic, improves performance, and enhances security by isolating sensitive data between departments.

2. **Inter-VLAN Routing**:  
   We utilized Layer 3 switches to enable communication between VLANs while keeping traffic flows under control. This solution allows efficient routing without needing additional hardware, reducing overall costs.

3. **IP Addressing & Subnetting**:  
   The IP addressing scheme is designed with subnetting principles in mind, assigning distinct ranges for each VLAN to facilitate better organization and reduce management complexity. Dynamic addressing is handled via a centralized **DHCP server**.

4. **Security Measures**:  
   The network architecture implements strict security protocols, including **Access Control Lists (ACLs)** and **RADIUS-based centralized authentication** to ensure that sensitive areas of the network are protected. Additional measures, such as strong password policies and encryption, further secure the infrastructure.

5. **Cost Efficiency**:  
   The overall cost of the network, amounting to **$10,500**, was kept within budget without sacrificing performance or security. Key components, such as Layer 3 switches and virtualized servers for DNS and DHCP, were chosen based on their ability to balance cost-effectiveness with high functionality.

6. **Scalability and Flexibility**:  
   The architecture is designed to be scalable, with the ability to add new departments or sectors with minimal reconfiguration. The modular use of VLANs and Layer 3 routing ensures that future growth can be supported without major overhauls.

This repository contains all the documentation and simulation files needed to replicate or modify the network. The presentation included in the repository outlines the design process, key decisions made, and the trade-offs considered for security, efficiency, and budget adherence.

---

**1. Network Diagram and Architecture**

- **Introduction**  
  The network design consists of multiple interconnected sectors, each tailored to specific departmental needs (Management, Study, Production, and Support). By leveraging VLANs and ACLs, we ensure traffic segmentation, enhance security, and improve resource allocation.

- **Detailed Reasoning**
  - **VLAN Segmentation:** VLANs allow us to logically segment the network by department (Management, Study, Production, Support). This minimizes broadcast traffic and increases security by limiting network communication to specific segments. Each sector's workstations have specific tasks, and VLANs ensure that unnecessary communication is minimized, reducing the risk of lateral attacks.
  - **Inter-VLAN Routing via Layer 3 Switches:** We use Layer 3 switches to enable communication between VLANs. This is a cost-effective alternative to using dedicated routers for inter-VLAN routing, reducing the number of devices needed while still ensuring traffic can flow efficiently between different sectors.
  - **Design Scalability:** The network's architecture is designed to be scalable, allowing future expansion by simply adding new VLANs or additional sectors without requiring significant changes to the core infrastructure.

- **Key Considerations**
  - Efficient management of broadcast domains.
  - Streamlined communication between departments using inter-VLAN routing.
  - Strong isolation of sensitive data in sectors like Management.

---

**2. IP Addressing Table and VLANs**

- **Introduction**  
  The IP addressing schema is divided by sector to keep network organization clean and efficient. Each sector is assigned a specific subnet, ensuring easy management and troubleshooting.

- **Detailed Reasoning**
  - **Subnetting:** Subnetting allows each VLAN to operate on its own distinct IP range. This segmentation is vital for security (controlling access between sectors) and simplifies the management of network traffic. For instance, management devices are isolated from production, limiting exposure to sensitive resources.
  - **DHCP for Dynamic Address Allocation:** The DHCP server dynamically assigns IPs to devices within each sector. This reduces manual configuration effort and ensures efficient use of IP addresses. By configuring the DHCP server per VLAN, the network can scale up seamlessly.
  
- **Key Considerations**
  - Efficient IP allocation through subnetting ensures there’s no overlap between sectors.
  - The use of DHCP reduces IP configuration errors and manual overhead.
  
---

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
  
---

**4. Security Measures**

- **Introduction**  
  Security was a primary focus during network design, with several key measures implemented to safeguard the network's assets and data.

- **Detailed Reasoning**
  - **VLANs and ACLs:** Segmenting the network with VLANs and using ACLs limits lateral movement in the event of a breach. Unauthorized access from one VLAN to another is tightly controlled.
  - **RADIUS for Centralized Authentication:** Using RADIUS, we enforce strong authentication protocols for anyone trying to access critical network devices. This reduces the risk of compromised credentials.
  - **Password Policies and Encryption:** We enforce strong password policies across all devices and encrypt sensitive traffic, protecting against brute force attacks and ensuring data privacy.

- **Key Considerations**
  - **Minimizing Attack Surface:** By isolating network traffic into sectors and limiting communication via ACLs, the attack surface is significantly reduced.
  - **Centralized Authentication Benefits:** Centralized authentication through RADIUS streamlines user access control and strengthens overall security.
  
---

**5. Cost Breakdown and Resource Allocation**

- **Introduction**  
  The network was designed to be cost-effective without sacrificing functionality or security. This section breaks down the costs of key components and justifies their inclusion based on performance and budget constraints.

- **Detailed Cost Justification**
  - **Layer 3 Switches:** Although Layer 3 switches are more expensive than Layer 2, their ability to perform inter-VLAN routing makes them a cost-effective choice by reducing the need for additional routers.
  - **Switches:** Cost-efficient models were selected for the Study and Production sectors, where high traffic and performance are less of a concern compared to the Management sector.
  - **Servers (DNS, DHCP):** We opted for virtualized servers to save on hardware costs. These virtual machines are run on a single physical server, reducing the total number of devices needed.
  - **Firewalls and RADIUS Authentication:** While Packet Tracer limits firewall configuration, we mitigate this by using ACLs and implementing centralized RADIUS authentication for device access, saving costs on high-end firewall appliances.

- **Total Cost:**
  - Layer 3 Switches: $5,000  
  - Access Switches: $2,000  
  - Servers (Virtualized for DNS, DHCP): $3,500  
  - Total Cost: **$10,500**
  
---

### Presentation Outline (for 10-minute Presentation)

1. **Introduction**
   - Overview of the network design and its goals.
   
2. **Architecture Choices**
   - Explanation of the use of VLANs, inter-VLAN routing, and Layer 3 switches.

3. **IP Addressing and Subnetting**
   - The logic behind IP allocation for each sector and how DHCP is used.

4. **Device Configuration and Security**
   - RADIUS authentication, ACLs, and password policies.

5. **Security Focus**
   - How security was prioritized: from VLANs to centralized authentication.

6. **Cost Justification**
   - Why we made specific choices to balance performance and cost.

7. **Conclusion**
   - Summarize how the design is scalable, secure, and cost-efficient.
