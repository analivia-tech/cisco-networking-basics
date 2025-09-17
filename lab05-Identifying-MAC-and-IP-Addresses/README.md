# Lab 05 - Identifying MAC and IP Addresses

## Objectives
- Gather PDU information for communication within a Local Network  
- Gather PDU information for communication with a Remote Network  
- Understand how MAC and IP addresses change depending on the destination  

## Scenario
In this lab, I explored how devices communicate over local and remote networks using Packet Tracer Simulation Mode.  
I focused on how MAC addresses (Layer 2) and IPv4 addresses (Layer 3) appear and change as PDUs travel from the source to the destination.  
This lab helps understand network operations, which is essential for careers in network administration or network security.  

## Steps I Followed

### Part 1: Local Network Communication
1. Selected host `172.16.31.3` and opened the Command Prompt.  
2. Sent a ping to `172.16.31.2` to generate ICMP echo requests.  
3. Switched to Simulation Mode and observed PDUs as they traveled:  
   - Recorded MAC and IP addresses for each hop using Outbound PDU Details  
   - Noted that MAC addresses change only when the PDU passes through a device like a switch, but IP addresses remain the same within the LAN  

### Part 2: Remote Network Communication
1. Sent a ping from `172.16.31.3` to `10.10.10.2`.  
2. Observed the first ICMP echo request, noting source and destination MAC and IP addresses.  
3. Captured PDU details at each hop across the router:  
   - Observed NAT behavior and MAC address changes at router interfaces  
4. Repeated the process for the echo reply (pong) from `10.10.10.2` back to `172.16.31.3`  
5. Recorded all MAC and IP address changes in a spreadsheet format  

### Reflection Questions
- What types of cables/media were used to connect devices?  
- Did the cables change how PDUs were processed?  
- Did the Wireless Access Point modify the PDUs it received?  
- How did the MAC addressing change as PDUs passed through the access point?  
- What was the highest OSI layer used by the Access Point?  
- At which OSI layer do cables and access points operate?  
- In the PDU Details, which MAC address appeared first: source or destination?  
- What do red Xs and green checkmarks mean in the simulation?  
- At which point did MAC addresses suddenly change when PDUs moved between networks 10 and 172?  
- Which device uses MAC addresses starting with 00D0:BA?  
- To which devices do the other MAC addresses belong?  
- Were the IPv4 addresses altered in any of the PDUs?  
- What happens to source and destination addresses during a ping reply?  
- Why do router interfaces belong to two different IP networks?  
- Which IP networks are connected by the router?  

## 💡 What I Learned
- How to observe MAC and IP address changes in local and remote communication  
- The role of switches, routers, and access points in forwarding PDUs  
- The importance of understanding OSI layers and NAT for troubleshooting
