# Lab05 - Creating a LAN

## Objectives
- Connect hosts and network devices
- Configure devices with IPv4 addressing
- Verify end device configuration and connectivity
- Use network commands to display host information

## Scenario
A new branch office is being opened, and you were asked to set up the LAN. The network devices are preconfigured, but you need to connect them to the hosts. You also need to assign IPv4 addresses to the end devices and verify that they can reach local and remote resources.

## Step 1 – Connect Network Devices and Hosts
1. Power on all devices, including the Office Router.
2. Use the **Physical** tab in each device to turn them on (look for the green LED).
3. Connect devices according to the table below:

| Device        | Interface/Port | Connected to Device | Connection Interface/Port |
|---------------|----------------|-------------------|--------------------------|
| Office Router | G0/0           | ISP1              | G0/0                     |
| Office Router | G0/1           | Switch            | G0/1                     |
| Admin PC      | NIC (F0)       | Switch            | F0/1                     |
| Manager PC    | NIC (F0)       | Switch            | F0/2                     |
| Printer       | NIC (F0)       | Switch            | F0/24                    |

> Note: G = GigabitEthernet, F = FastEthernet. Use copper straight-through cables.

## Step 2 – Configure IPv4 Addressing
- **Admin PC and Manager PC**: Configure to receive IP via DHCP from the Office Router.
- **Printer**: Configure static IP according to the addressing table below:

| Device | IPv4 Address      | Subnet Mask      | Default Gateway / Server |
|--------|-----------------|----------------|-------------------------|
| Printer| 192.168.1.100    | 255.255.255.0  | www.cisco.pt            |
| Server | 209.165.200.225  | N/A            | N/A                     |

### Questions
- Why are the IPv4 addresses different, but the subnet masks and default gateways the same?  
*Answer here*

- If the printer needed a default gateway, what would it be? How could you determine it from other devices?  
*Answer here*

## Step 3 – Verify Connectivity
1. Check IP configuration on the PCs (`ipconfig`).
2. Ping the printer from both PCs to verify connectivity.
3. Test connectivity to the internet using the IP and URL of the server.

### Questions
- If you can connect via IP but not via URL, what could be the cause?  
*Answer here*

## Step 4 – Use Network Commands
- `ipconfig`: Display host addressing.
- `ipconfig /all`: Display additional host information.
- `tracert [URL]`: Trace route to remote server.

### Questions
- How many routers are crossed to reach the destination? How are they identified?  
*Answer here*

- Where is the second router located?  
*Answer here*

## 💡 Reflection
- Consider a small office with a LAN similar to this one. What is the biggest challenge when setting up the network at a new location?  
*Answer here*
