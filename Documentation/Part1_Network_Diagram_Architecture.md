## Part 1 - Network Diagram and Architecture

### 1. Introduction
The network architecture is structured into five distinct sectors: Management, Study, Production, Support 1, and Support 2. Each department is allocated its own VLAN to ensure traffic segmentation, preventing unauthorized lateral movement between departments and reducing the attack surface in case of a breach.

### 2. Key architectural components
- **Management VLAN**: Responsible for administrative operations, housing 4 computers, a printer, and IP phone.
- **Study VLAN**: Contains 8 computers and a printer, supporting research and study operations.
- **Production VLAN**: Consists of 10 workstations and handles the core production tasks.
- **Support 1 and Support 2 VLANs**: Each support sector contains 9 and 10 computers respectively, supporting technical and customer service operations.
- **Server Room**: Centralized servers (DNS, DHCP, RADIUS) and routers reside here, handling inter-VLAN communication, DHCP IP assignment, and centralized user authentication.

By strategically placing switches and routing traffic via Layer 3 switches, we’ve ensured that the network is both scalable and efficient without requiring additional routing hardware.
