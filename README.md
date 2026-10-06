# Task 4: Setup and Use a Firewall

## Objective
Configure and test basic firewall rules to allow or block network traffic.

## Environment
- Operating System: macOS
- Firewall: macOS Application Firewall and PF (Packet Filter)
- Test Port: TCP 23 (Telnet)
- Tool: Terminal and Netcat (nc)

## Procedure
1. Checked the macOS Application Firewall status.
2. Listed the configured firewall applications.
3. Checked TCP port 23 for a listening service.
4. Created a temporary PF rule to block TCP port 23.
5. Started a temporary local test service on port 23 using Netcat.
6. Tested the connection before applying the firewall rule.
7. Loaded and enabled the PF firewall rule.
8. Tested the connection again and confirmed that it was blocked.
9. Stopped the temporary test service.
10. Disabled PF and restored the system after testing.
11. Verified that the macOS Application Firewall remained enabled.

## Firewall Rule Tested
block in quick on lo0 proto tcp to port 23

## Result
The TCP connection to port 23 succeeded before the firewall rule was applied. After enabling the PF rule, the connection timed out, demonstrating that the firewall successfully blocked the specified traffic.

## Key Concepts
- Firewall configuration
- Inbound traffic filtering
- TCP ports
- PF (Packet Filter)
- Application Firewall
- Telnet (Port 23)

## Screenshots
All screenshots showing the firewall configuration and testing process are included in the `screenshots` folder.

## Note
The internship task specifies Windows Firewall or UFW on Linux. Since this task was completed on macOS, the built-in macOS Application Firewall and PF were used to demonstrate the equivalent firewall configuration and traffic-filtering concepts.
