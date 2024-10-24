## Part 2 - IP Addressing Table and VLANs

The network uses a structured IP addressing schema to assign specific subnets to each department, ensuring efficient traffic management and reducing the risk of IP conflicts. Dynamic IP assignment is managed by a centralized DHCP server, which is configured with different scopes for each VLAN. This dynamic assignment simplifies network expansion and reduces manual configuration errors.

- **Management VLAN**: VLAN 10 192.168.10.0/26
- **Study VLAN**: VLAN 20 192.168.10.64/26
- **Production VLAN**: VLAN 30 192.168.10.128/26
- **Support 1 VLAN**: VLAN 40 192.168.10.192/26
- **VOICE VLAN**: VLAN 50 192.168.11.0/26
- **NATIVE VLAN**: VLAN 99
- **DHCP/DNS**: 8.8.8.8/8
- **iSCSI storage server**: 192.168.100.2/30
- **RADIUS SERVER**: 10.0.0.3/29
- **MULTI LAYER SWITCH**:
    Vlan10                 192.168.10.2    
    Vlan20                 192.168.10.66                          
    Vlan30                 192.168.10.130                         
    Vlan40                 192.168.10.194                         
    Vlan50                 192.168.11.2
    G1/0/1:                10.0.0.2/30
    G1/0/2:                8.8.8.1/8
    G1/0/8:                192.100.1.1/30
-**ROUTER**: G0/0/0:  10.0.0.1/30
             G0/0/1:  200.100.0.1/24
   


Inter-VLAN routing is handled by Layer 3 switches, ensuring seamless communication between departments while still maintaining traffic segmentation. Specific Access Control Lists (ACLs) further restrict unnecessary communication between certain VLANs, protecting sensitive resources like Management’s assets from being accessed by Production or Support sectors.

