# Lab 04 - Examining NAT on a Wireless Router

## Objectives
- Examine the NAT configuration on a wireless router  
- Connect four PCs to a wireless router using DHCP  
- Observe network traffic and understand how NAT translates private addresses  

## Scenario
A small home network needs to connect multiple PCs to the Internet through a wireless router.  
The router uses NAT (Network Address Translation) to allow private IP addresses to communicate with external networks.  
The goal is to observe NAT behavior and the flow of traffic between internal hosts and external servers.  

## Steps I Followed
1. Added one PC and connected it to the wireless router using a straight-through cable.  
2. Configured the PC to receive an IP address via DHCP and noted the default gateway.  
3. Accessed the router’s web GUI (username: `admin`, password: `admin`) to examine:  
   - Internet connection IP (public or private)  
   - Local network IP (private)  
   - DHCP range for internal clients  
4. Added three more PCs and connected them to the router.  
5. Configured each PC to use DHCP and verified IP addresses using `ipconfig /all`.  
   - Noted that these devices received private IP addresses, which require NAT to communicate externally.  
6. Entered **Simulation Mode** in Packet Tracer to observe network traffic:  
   - Applied filters for TCP and HTTP traffic  
   - Created a complex PDU from one PC to `ciscolearn.nat.com` (HTTP, source port 1000, periodic interval 120s)  
   - Observed packet flow using the Simulation Panel  
7. Examined packet headers:  
   - Checked source (SRC) and destination (DST) IP addresses for inbound and outbound traffic  
   - Observed NAT translation of source IPs as packets crossed the router  

## Results
- All PCs received private IP addresses via DHCP  
- NAT translation successfully allowed communication between private IPs and the external server  
- Simulation confirmed proper flow of TCP/HTTP traffic and address translation  

## 💡 What I Learned
- How NAT works to allow private IP addresses to access external networks  
- How to configure DHCP for multiple clients on a wireless router  
- How to use Packet Tracer Simulation Mode to inspect packet headers and network traffic
