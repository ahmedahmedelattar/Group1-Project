# Group1-Project
#Must have packet tracer to test and view the topology.
#read the attached report to view the configuration and uderstand the purpose of the project

Network Development Summary
In this project, we designed and implemented a secure and redundant network infrastructure for a company with two floors, each housing different departments, including HR, Finance, Marketing, Sales, Customer Service, and IT. To ensure seamless wireless connectivity, access points were deployed on each floor.
The network includes a web server and an FTP server, accessible from the external network, and an internal server, which is restricted to internal access only. To achieve high security and redundancy, the following key components were implemented:
•	Inter-VLAN Routing: Used to enable communication between different departments.
•	Redundancy: Implemented using two routers with HSRP, ensuring load balancing by prioritizing certain VLANs on Router 1 and others on Router 2. Additionally, EtherChannel was configured between the two switches for high-speed connectivity and fault tolerance.
•	Firewall Security: A firewall was configured with three security zones: 
o	DMZ (for public-facing services like web and FTP servers)
o	Internal Network (for company resources)
o	Internet (external access)
o	ACLs were used to control access between zones and restrict unwanted services in the DMZ.
•	Routing: Implemented OSPF for efficient dynamic routing.
•	NAT: 
o	Dynamic NAT enabled internal devices to access the internet securely.
o	Static NAT ensured public accessibility for the web and FTP servers.
•	DHCP: Used for automatic IP assignment to internal clients.
•	Layer 2 Security Enhancements: 
o	Port Security to prevent unauthorized device connections.
o	DTP (switchport nonegotiate) to disable unnecessary trunking.
o	DHCP Snooping to prevent rogue DHCP servers.
o	Dynamic ARP Inspection (DAI) to block ARP spoofing attacks.
o	PortFast & BPDU Guard to protect against spanning tree attacks.
This network design ensures high availability, performance, and security, meeting the company’s operational requirements while protecting against potential threats.
