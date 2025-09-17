# Lab 03 - Configure DHCP on a Wireless Router

## Objectives
- Connect three PCs to a wireless router using Ethernet cables  
- Configure the router’s DHCP settings with a custom IP range  
- Set clients to receive IP addresses dynamically via DHCP  
- Test connectivity between the router and the PCs  

## Scenario
A home user wants to connect three PCs to a wireless router. All PCs should automatically receive their IP addresses from the router using DHCP. The router’s default DHCP configuration will be modified to use a specific subnet and address range.  

## Steps I Followed
1. Added three generic PCs and connected them to the wireless router with straight-through cables.  
2. Verified the default DHCP configuration on **PC0** and noted the default gateway (router’s IP).  
3. Logged into the router’s web GUI (default user: `admin`, password: `admin`).  
   - Confirmed that DHCP was enabled with a default IP range.  
4. Changed the router’s IP address to `192.168.5.1` and saved settings.  
   - Renewed the IP configuration on PC0 to receive a new address in the 192.168.5.0/24 network.  
5. Modified DHCP settings:  
   - Start IP Address: `192.168.5.126`  
   - Maximum Number of Users: `75`  
   - Saved the new configuration.  
6. Renewed DHCP leases on all three PCs (PC0, PC1, PC2) and confirmed that they received valid IPs.  
7. Tested connectivity using Command Prompt:  
   - `ping 192.168.5.1` → reached the router  
   - `ping 192.168.5.126` → reached PC0  
   - `ping 192.168.5.127` → reached PC1  

## Results
- All three PCs successfully received IP addresses from the router via DHCP.  
- The router and all PCs were reachable through ping, confirming proper configuration.  

## 💡 What I Learned
- How to configure a router with a custom IP address and DHCP pool.  
- How clients dynamically obtain IP addresses from a DHCP-enabled router.  
- How to verify IP configuration and connectivity using `ipconfig` and `ping`.
