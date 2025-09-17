# Lab 11 - Using Telnet and SSH

## Objective
This lab focuses on establishing remote access to a router using Telnet and SSH protocols. The goal is to understand the difference between secure and insecure remote access methods and how to verify connectivity before initiating a remote session.

## Scenario
A router (HQ) is configured with an IP address of 64.100.1.1 on interface G0/0/1. Two PCs (PC0 and PC1) are configured to obtain IP addresses via DHCP. The task is to verify IP configuration, test connectivity to the router, and attempt remote access using Telnet and SSH.

## Steps Performed
1. Verified that the PC received an IP address via DHCP using the `ipconfig` command.
2. Tested connectivity to the router HQ using the `ping 64.100.1.1` command.
3. Attempted to access the router using Telnet with `telnet 64.100.1.1`, which was unsuccessful due to security restrictions.
4. Successfully accessed the router using SSH with the command `ssh -l admin 64.100.1.1` and password `class`.

## What I learned
Through this lab, I learned how to:
- Verify IP address assignment via DHCP.
- Test network connectivity using ping.
- Understand the security implications of Telnet versus SSH.
- Establish a secure remote connection to a network device using SSH.

This lab reinforced the importance of secure remote access in network management and provided hands-on experience with basic connectivity troubleshooting and remote login protocols.
