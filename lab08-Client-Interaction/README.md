# Lab08 - Client Interaction

## Objectives
- Observe client-server interactions between a PC and a server.

## Scenario
Clients, such as desktop PCs, request services from servers. This lab environment supports a variety of services in a simulated network. The Packet Tracer allows adding network servers for DHCP, DNS, HTTP, and TFTP, as well as simulated PCs that can request these services.

In this activity, a simple network is used with one PC connected directly to a server configured to provide DNS services and host a web page via an HTTP server. This lab tracks the traffic flow when a web page is requested, how the page’s IP is resolved, and how the web page is delivered.

## Instructions

### Step 1 – Enter Simulation Mode
1. Open Packet Tracer.
2. Click **Simulation Mode** in the bottom-right corner of the logical workplace.

### Step 2 – Set Event List Filters
1. Click **Show All/None** to deselect all events.
2. Click **Edit Filters**.
3. In the **IPv4** tab, select **DNS**.
4. In the **Misc** tab, select **HTTP**.
5. Close the window. Only DNS and HTTP events will now be visible.

### Step 3 – Request a Web Page
1. Click on the **PC**.
2. Open the **Desktop** tab and select **Web Browser**.
3. Enter `www.example.com` in the URL box and click **Go**.
4. Minimize the PC window.

### Step 4 – Run the Simulation
1. In the **Simulation Panel**, click **Play**.
2. Observe the exchange between the PC and the server in the Event List:
   - DNS resolution of the URL to an IP address
   - Server provides the IP address
   - PC requests the web page
   - Server sends the web page in two segments
   - PC acknowledges receipt
3. Use **View Previous Event** to review events if the buffer fills up.

### Step 5 – Examine a Specific PDU
1. Restore the PC window (web page should be displayed).
2. In the **Simulation Panel Event List**, click the colored box in the last column of the first event to open **PDU Information**.
3. Click **Next Layer >>** repeatedly to inspect inbound and outbound PDU layers.
4. Read the descriptions below each layer for a detailed understanding of the data exchange.

## 💡 Reflection
- Observe how DNS and HTTP requests flow between the PC and server. What differences did you notice in the PDU layers?
*Answer here*
