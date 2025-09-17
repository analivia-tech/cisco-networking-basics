# Lab 06 - Observing Traffic Flow in a Routed Network

## Objectives
- Part 1: Observe traffic flow in an unrouted LAN  
- Part 2: Reconfigure the network for inter-LAN routing  
- Part 3: Observe traffic flow in the routed network  

## Scenario
The company XYZ LLC is expanding and its network must grow accordingly.  
Currently, all departments share a single IPv4 network, which is inefficient and causes delays.  
This lab demonstrates how routing between multiple LANs improves network efficiency.  

## Steps I Followed

### Part 1: Traffic Flow in an Unrouted LAN
1. Cleared the ARP cache on `Sales 1`.  
2. Noted the IP address of `Sales 1`.  
3. Opened the Command Prompt on `Sales 1` and ran `arp -a` to check the cache.  
4. Switched to Simulation Mode and pinged `Sales 1` from `Sales 2`.  
5. Observed the PDUs moving through the network and recorded:  
   - Source and destination MAC addresses  
   - Source and destination IP addresses  
6. Noted that destination MAC was a broadcast address.  
7. Observed which devices processed ARP request packets and considered the impact on network efficiency.  
8. Inspected the new PDU created in `Sales 2` and identified its type.  

### Part 2: Reconfiguring the Network for Inter-LAN Routing
1. Connected each departmental switch directly to a router interface (Edge Router) using straight-through cables.  
2. Configured hosts to receive IP addresses from the router’s DHCP in new subnets:  
   - `Accounting` remains in `192.168.1.0/24`  
   - `Finance` and `Sales` receive new subnets  
3. Renewed IP addresses on hosts using `ipconfig /renew` to receive updated addresses.  
4. Noted the new subnets:  
   - Finance subnet: _______  
   - Sales subnet: _______  

### Part 3: Traffic Flow in the Routed Network
1. Cleared the ARP cache on `Sales 2`.  
2. Switched to Simulation Mode and pinged `Sales 1`.  
3. Observed how ARP requests now flow through the routed network.  
4. Repeated pings to other hosts and the Internet server.  
5. Observed the benefit of using multiple subnets in improving network efficiency.  

## 💡 What I Learned
- How traffic behaves differently in a single LAN versus multiple routed LANs  
- The role of routers in separating broadcast domains  
- How subnetting improves network performance  
- How to use Packet Tracer Simulation Mode to visualize PDU flow and ARP behavior
