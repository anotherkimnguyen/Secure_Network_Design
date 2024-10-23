## Part 5 - Cost Breakdown and Resource Allocation

### 1. Introduction
The network infrastructure focuses on selecting equipment that balances functionality, cost-effectiveness, and scalability.

### 2. Assumptions for Unit Costs:
- PC: €600 each
- Printer: €300 each
- IP Phone: €100 each
- Switch: €400 each
- Server: €2000
- Router: €800
- Multilayer Switch: €1500
- Firewall/ACLs (optional): €1200 per unit or configuration

### 3. Management
- 5 PCs: 5 × €600 = €3000
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400
- **Total for Management**: €3800

### 4. Study
- 8 PCs: 8 × €600 = €4800
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400
- **Total for Study**: €5600

### 5. Server Room
- 1 Server: €2000
- 1 Router: €800
- 1 Multilayer Switch: €1500
- **Total for Server Room**: €4300

### 6. Production
- 10 PCs: 10 × €600 = €6000
- 1 Printer: €300
- 1 IP Phone: €100
- 1 Switch: €400
- **Total for Production**: €6800

### 7. Support 1
- 10 PCs: 10 × €600 = €6000
- 5 IP Phones: 5 × €100 = €500
- 1 Printer: €300
- 1 Switch: €400
- **Total for Support 1**: €7200

### 8. Support 2
- 10 PCs: 10 × €600 = €6000
- 5 IP Phones: 5 × €100 = €500
- 1 Printer: €300
- 1 Switch: €400
- **Total for Support 2**: €7200

### 9. Total Costs Per Department:
- **Management**: €3800
- **Study**: €5600
- **Server Room**: €4300
- **Production**: €6800
- **Support 1**: €7200
- **Support 2**: €7200

### 10. Overall Cost Breakdown (without firewall/ACLs):
- Total PCs (43 PCs): 43 × €600 = €25,800
- Total Printers (5 Printers): 5 × €300 = €1500
- Total IP Phones (13 IP Phones): 13 × €100 = €1300
- Total Switches (6 Switches): 6 × €400 = €2400

- **Server Room Equipment**:
  - Server: €2000
  - Router: €800
  - Multilayer Switch: €1500
  - **Total for Server Room**: €4300

### 11. Grand Total (without firewall/ACLs):
€25,800 (PCs) + €1500 (Printers) + €1300 (IP Phones) + €2400 (Switches) + €4300 (Server Room) = €35,300

### 12. Adding Firewall/ACL Costs:
- **Option 1**: Physical Firewalls: Deploying 6 firewalls (one per section/department) at €1200 each:  
  - 6 × €1200 = €7200  
  - **Total with Physical Firewalls**: €35,300 + €7200 = €42,500

- **Option 2**: ACL/Virtual Firewalls: Configure virtual firewalls or ACLs on the router/s
