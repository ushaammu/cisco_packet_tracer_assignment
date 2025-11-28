# cisco_packet_tracer_assignment
Network Configuration Exercises

This project contains five networking exercises designed to build skills in DHCP, VLANs, routing, DNS, and Layer-3 switch configuration using Cisco Packet Tracer.

1. Exercise 1 – Basic DHCP Configuration

This exercise introduces simple DHCP setup using a router. A basic topology is created with a router, switch, and PCs. The router’s interface is configured with an IP address, and a DHCP pool is created to automatically assign IPs to the PCs. Excluded addresses are added to ensure the router’s own IP and reserved addresses are not leased. PCs are set to DHCP mode to verify automatic IP assignment using ipconfig and show ip dhcp binding.

2. Exercise 2 – DHCP for Multi-VLAN (Router-on-a-Stick)

Here, VLAN segmentation and inter-VLAN communication are implemented using router sub-interfaces. The switch is configured with VLAN 10 and VLAN 20, ports are assigned, and trunking is enabled. The router creates sub-interfaces for each VLAN with dot1Q encapsulation. DHCP pools for both VLANs allow PC-A and PC-B to obtain automatic IPs from different networks.

3. Exercise 3 – DNS + Website Access

This exercise sets up a server providing both DNS and HTTP services. The server receives a static IP, an A-record is created mapping a domain name (example.com) to the server IP, and a simple webpage is added. PCs use static IPs with the DNS server configured, allowing successful pinging and webpage access via the domain.

4. Layer-3 Switch Configuration

A Layer-3 switch (3560/3650) is used to route between VLANs. VLAN interfaces (SVIs) are created with gateway IPs for each VLAN. The command ip routing enables inter-VLAN routing. PCs placed in different VLANs can communicate using these SVIs.

5. VLAN Assignment

Switch ports are configured in access mode and assigned to their respective VLANs. Each PC connects to a dedicated port mapped to VLAN 10, 20, or 30, ensuring proper traffic separation before routing or DHCP services apply.
