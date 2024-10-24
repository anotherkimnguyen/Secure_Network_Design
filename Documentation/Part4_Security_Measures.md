## Part 4 - Security Measures

Security was a primary focus throughout the network design process, with several measures implemented to protect the network from both internal and external threats:

- **VLAN Segmentation**: Each department is separated by VLAN, ensuring that sensitive information from departments like Management cannot be accessed by other departments like Production or Support. This segmentation reduces the attack surface and enhances overall network security.

- **Access Control Lists (ACLs)**: We have implemented strict ACLs on inter-VLAN traffic to control which devices can communicate across VLANs. For instance, Production VLAN traffic is blocked from accessing resources on the Management VLAN except for specific exceptions, such as print services.

- **RADIUS Authentication**: The RADIUS server centralizes authentication, requiring users to authenticate before accessing any critical network device. This minimizes the risk of compromised devices, enforces strong password policies, and provides centralized management of user credentials.

- **Strong Password Policies and Encryption**: We enforce strong password policies across all network devices and enable encryption protocols to secure traffic where possible, especially on the servers handling DNS, DHCP, and user authentication. This ensures that even if credentials are compromised, brute force attacks are less likely to succeed. All sensitive data traffic between servers, such as DNS and DHCP requests, is secured using AES-256 encryption. Additionally, communication between devices and the RADIUS authentication server is secured with TLS/SSL protocols to ensure data privacy and integrity during transmission. This reduces the risk of man-in-the-middle attacks and ensures compliance with best practices for securing sensitive information in transit.
