**5. Cost Breakdown and Resource Allocation**

- **Introduction**  

  The network was designed to be cost-effective without sacrificing functionality or security. This section breaks down the costs of key components and justifies their inclusion based on performance and budget constraints.

- **Detailed Cost Justification**
  
  - **Core Network Devices:** These devices manage inter-segment traffic and routing, which are essential for efficient communication between different parts of the network (like management, production, and support). While core devices are more expensive, their scalability and efficiency make them a cost-effective choice, avoiding the need for additional routing equipment.  
    - **Cost**: $2,500.

  - **Access Network Devices:** Cost-efficient options were chosen for areas like the study and production sectors, where performance requirements are not as critical. These access devices provide essential connectivity without the high price tag of high-performance models.  
    - **Cost**: $8,000.

  - **Servers (for DHCP and DNS):** Virtualized servers are employed to minimize the number of physical devices needed. Running multiple services (such as DHCP and DNS) on virtual machines reduces hardware costs while maintaining network efficiency.  
    - **Cost**: $1,000.

  - **Security and Access Control:** The network security relies on ACLs (Access Control Lists) and centralized authentication instead of expensive firewalls. ACLs limit unauthorized access between network segments, while centralized authentication ensures secure access to critical devices.  
    - **Cost**: $300.

  - **Cabling and Infrastructure:** The physical network infrastructure, such as cabling, contributes to the overall connectivity of devices. These are relatively minor but essential costs in any network setup.  
    - **Cost**: $300.

---

- **Total Cost**  
  - Core Network Devices: $2,500  
  - Access Network Devices: $8,000  
  - Servers (for DHCP and DNS): $1,000  
  - Security and Access Control: $300  
  - Cabling and Infrastructure: $300  

**Total Cost: $12,100**
