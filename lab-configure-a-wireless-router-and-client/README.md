# Lab 01 - Configure a Wireless Router and Clients

## Objectives
- Connect devices correctly (cable modem, TV, PCs, and router)  
- Configure the home wireless router (basic setup, DHCP, password, SSID)  
- Set up IP addressing and test connectivity for both wired and wireless clients  

## Scenario
My friend Natsumi just moved into a new house and asked me to help set up her home network.  
The tasks included:  
- Connecting the cable service to both Internet and TV  
- Configuring a home wireless router to provide IP addresses  
- Creating a secure Wi-Fi network  
- Making sure all devices (wired PCs and a laptop) could access the Internet  

## Steps I Followed
1. Connected the coaxial cable from the provider to the cable modem and the TV through a splitter.  
2. Connected the cable modem to the **Home Wireless Router** (Internet port).  
3. Connected the **Office PC** and **Bedroom PC** to the router via Ethernet.  
4. Accessed the router’s GUI from the Office PC and:  
   - Enabled DHCP (limited to 10 users).  
   - Changed the admin password to `MyPassword1!`.  
   - Created a Wi-Fi network (SSID: `MyHome`, Security: WPA2, Passphrase: `MyPassPhrase1!`).  
5. Connected the **Laptop** to the Wi-Fi and tested Internet access.  
6. Verified Internet connectivity on the Office PC and Bedroom PC using the web browser.  

## Results
- All devices (TV, PCs, Laptop) were successfully connected.  
- Wired and wireless devices received IP addresses starting with `192.`  
- I was able to browse to `skillsforall.srv` from every client, confirming Internet access.  

## 💡 What I Learned
- How to connect and configure a basic home network with both wired and wireless devices.  
- The importance of securing the wireless router (changing default admin password, using WPA2).  
- How DHCP automatically assigns IP addresses and makes network setup easier.  
- How to test connectivity using simple tools (web browser, IP configuration).  
