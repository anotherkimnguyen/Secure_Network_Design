## Part 1 - Network Diagram and Architecture

### 1. Introduction
The network design consists of multiple interconnected sectors, each tailored to specific departmental needs (Management, Study, Production, and Support). By leveraging VLANs and ACLs, we ensure traffic segmentation, enhance security, and improve resource allocation.

### 2. Detailed Reasoning

- **VLAN Segmentation**: VLANs allow us to logically segment the network by department. This minimizes broadcast traffic and increases security by limiting network communication to specific segments.
  
- **Inter-VLAN Routing via Layer 3 Switches**: Layer 3 switches are used for inter-VLAN communication, providing a cost-effective alternative to dedicated routers.

- **Design Scalability**: The architecture is designed to be scalable, allowing future expansion by adding new VLANs or sectors without requiring significant changes to the core infrastructure.

### 3. Key Considerations
- Efficient management of broadcast domains.
- Streamlined communication between departments using inter-VLAN routing.
- Strong isolation of sensitive data in sectors like Management.
