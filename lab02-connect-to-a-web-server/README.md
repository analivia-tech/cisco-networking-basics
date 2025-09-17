# Lab 02 - Connect to a Web Server

## Objectives
- Observe how packets travel across the Internet using IP addresses.  
- Verify connectivity between a client and a web server.  
- Access a web page hosted on a server using its IP address.  

## Scenario
In this lab, I used a client computer (PC0) to check connectivity with a web server and then opened the server’s web page using its IP address. This simulates how real devices communicate across the Internet.  

## Steps I Followed
1. Opened the **Command Prompt** on PC0.  
2. Sent a ping to the server’s IP address `172.33.100.50`.  
   - The server replied, confirming connectivity (some replies timed out at first due to ARP resolution, which is normal).  
3. Opened the **Web Browser** on PC0.  
4. Typed `172.33.100.50` in the URL field and clicked **Go**.  
5. The client successfully connected to the server and displayed the web page.  

## Results
- Ping confirmed that PC0 could reach the server.  
- The web page loaded successfully from the server.  

## 💡 What I Learned
- Ping is a useful tool to verify if devices can communicate on a network.  
- Sometimes the first ping may fail due to ARP, but subsequent replies show successful connectivity.  
- A client can connect directly to a server using its IP address in a web browser.
