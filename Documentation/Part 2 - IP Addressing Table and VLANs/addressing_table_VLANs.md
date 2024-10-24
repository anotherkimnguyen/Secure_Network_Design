## Part 2 - IP Addressing Table and VLANs

The network uses a structured IP addressing schema to assign specific subnets to each department, ensuring efficient traffic management and reducing the risk of IP conflicts. Dynamic IP assignment is managed by a centralized DHCP server, which is configured with different scopes for each VLAN. This dynamic assignment simplifies network expansion and reduces manual configuration errors.

- **Management VLAN**: Assigned to subnet ...
- **Study VLAN**:
- **Production VLAN**:
- **Support 1 VLAN**:
- **Support 2 VLAN**:

Inter-VLAN routing is handled by Layer 3 switches, ensuring seamless communication between departments while still maintaining traffic segmentation. Specific Access Control Lists (ACLs) further restrict unnecessary communication between certain VLANs, protecting sensitive resources like Management’s assets from being accessed by Production or Support sectors.

