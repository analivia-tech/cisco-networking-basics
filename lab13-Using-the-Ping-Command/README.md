# Lab 13 - Using the Ping Command

## Objective
This lab focuses on using the `ping` command to diagnose connectivity issues and identify misconfigurations in DNS settings on client PCs. The goal is to determine why certain users are unable to access a website and apply corrective actions.

## Scenario
A small business owner reports that some users cannot access a website. All PCs are configured with static IP addresses. The task is to use the `ping` command to identify which PCs are experiencing connectivity issues and determine whether the problem is related to IP configuration or DNS resolution.

## Steps Performed
1. Attempted to access the website `www.cisco.pka` from each PC using the web browser.
2. Identified which PCs failed to connect to the web server.
3. Used the `ping www.cisco.pka` command from problematic PCs to test name resolution and connectivity.
4. Used the same `ping` command from correctly configured PCs to compare results.
5. Pinged the web server's IP address directly from the problematic PCs to verify connectivity.
6. Used `ipconfig /all` to inspect DNS server settings on both working and non-working PCs.
7. Identified mismatched or incorrect DNS configurations on the PCs with connectivity issues.
8. Corrected the DNS settings using the IP Configuration tool in the Desktop tab.
9. Retested access to `www.cisco.pka` using the web browser to confirm the issue was resolved.

## Summary of Learnings
Through this lab, I learned how to:
- Use the `ping` command to test connectivity and diagnose network issues.
- Understand the role of DNS in resolving domain names to IP addresses.
- Compare network configurations across devices to identify inconsistencies.
- Apply configuration changes to resolve connectivity problems.

This exercise reinforced the importance of DNS settings in network communication and demonstrated how basic troubleshooting tools like `ping` and `ipconfig` can be used to resolve real-world issues.
