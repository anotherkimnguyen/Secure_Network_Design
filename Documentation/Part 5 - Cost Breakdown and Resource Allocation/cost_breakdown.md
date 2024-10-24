## Part 5 - Cost Breakdown and Resource Allocation

### 1. Introduction
We selected hardware components that strike a balance between performance, scalability, and cost-efficiency. The goal was to ensure the network infrastructure is robust enough to meet the client’s needs without over-investing in unnecessarily high-end equipment. For example, we chose mid-range €600 PCs that are capable of handling day-to-day business tasks without being overly specialized. Similarly, the selection of network switches, routers, and servers reflects a thoughtful approach to balancing functionality and budget.

The following is a detailed breakdown of the costs per sector.

### 2. Assumptions for Unit Costs:
- PC: €600 each
- Printer: €300 each
- IP Phone: €100 each
- Switch: €400 each
- Server: €2000
- Router: €800
- Multilayer Switch: €1500
- Firewall/ACLs (optional): €1200 per unit or configuration

### Management
- 5 PCs (instead of 5): 5 × €600 = €3000
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400  
**Total for Management**: €3800

### Study
- 8 PCs: 8 × €600 = €4800
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400  
**Total for Study**: €5600

### Server Room
- 3 Servers: 3 x €2000 = €6000
- 1 Router: €800
- 1 Multilayer Switch: €1500  
**Total for Server Room**: €8300

### Production
- 10 PCs: 10 × €600 = €6000
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400  
**Total for Production**: €6800

### Support 1
- 10 PCs: 10 × €600 = €6000
- 5 IP Phones: 5 × €100 = €500
- 1 Printer: €300
- 1 Switch: €400  
**Total for Support 1**: €7200

### Support 2
- 10 PCs: 10 × €600 = €6000
- 5 IP Phones: 5 × €100 = €500
- 1 Printer: €300
- 1 Switch: €400  
**Total for Support 2**: €7200

### Overall Cost Breakdown
**Grand Total (without firewall/ACLs)**: €38,900

### Adding firewall/ACL costs:
- **Physical Firewalls**: €44,900
- **Virtual ACL configuration**: €38,900 + €1200 = €40,100

Deploying physical firewalls at the perimeter of the network provides crucial protection against external threats such as denial-of-service (DoS) attacks. By inspecting and filtering incoming and outgoing traffic, these firewalls prevent malicious traffic from reaching the internal network, safeguarding critical infrastructure from external attacks. The cost of €1,200 per unit is justified by the enhanced security and peace of mind they offer, especially for sensitive operations conducted within the Management and Server Room VLANs.

