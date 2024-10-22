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
