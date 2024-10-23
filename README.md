## Network Design and Architecture - Summary

This project outlines the design and implementation of a secure, efficient, and scalable network for a client relocating to a new office space. The goal was to create a structured, robust, and cost-effective network infrastructure that caters to the unique needs of various sectors, including Management, Study, Production, and Support. The project was simulated using Cisco Packet Tracer and involved the following key elements:

### 1. VLAN Segmentation:
The network is divided into multiple VLANs, each assigned to a specific sector. This segmentation reduces broadcast traffic, improves performance, and enhances security by isolating sensitive data between departments.

### 2. Inter-VLAN Routing:
Layer 3 switches were used to enable communication between VLANs while keeping traffic flows under control. This allows efficient routing without needing additional hardware, reducing overall costs.

### 3. IP Addressing & Subnetting:
The IP addressing scheme is designed with subnetting principles in mind, assigning distinct ranges for each VLAN to facilitate better organization and reduce management complexity. Dynamic addressing is handled via a centralized DHCP server.

### 4. Security Measures:
The network architecture implements strict security protocols, including Access Control Lists (ACLs) and RADIUS-based centralized authentication to ensure sensitive areas of the network are protected. Additional measures, such as strong password policies and encryption, further secure the infrastructure.

### 5. Cost Efficiency:
The overall cost of the network, amounting to $10,500, was kept within budget without sacrificing performance or security. Key components, such as Layer 3 switches and virtualized servers for DNS and DHCP, were chosen based on their ability to balance cost-effectiveness with high functionality.

### 6. Scalability and Flexibility:
The architecture is designed to be scalable, allowing new departments or sectors to be added with minimal reconfiguration. The modular use of VLANs and Layer 3 routing ensures future growth can be supported without major overhauls.

This repository contains all the documentation and simulation files needed to replicate or modify the network. The presentation included in the repository outlines the design process, key decisions made, and the trade-offs considered for security, efficiency, and budget adherence.
