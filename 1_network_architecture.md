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
