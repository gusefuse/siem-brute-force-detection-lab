# SIEM-Based Brute Force Attack Detection Lab

## Overview
This project simulates a brute-force attack in a controlled lab environment and analyzes the generated logs using Splunk SIEM to detect and investigate suspicious authentication activity.

## Tools and Technologies
- Splunk SIEM
- Windows Virtual Machine (Target)
- Kali Linux (Attacker)
- VirtualBox

## Lab Setup
- Configured a Windows VM as the target system
- Used Kali Linux as the attacker machine
- Enabled Windows Security logging
- Ingested logs into Splunk for analysis

## Attack Simulation
- Performed brute-force login attempts from Kali Linux to the Windows machine
- Generated multiple failed login events (Event ID 4625)
- Observed authentication behavior and login patterns

## Log Analysis
- Identified repeated failed login attempts from a single IP
- Extracted attacker IP using Splunk queries (rex)
- Correlated failed and successful login events (Event ID 4624)
- Detected successful RDP login (Logon Type 10)

## Dashboard
Created dashboards to visualize:
- Failed login attempts over time
- Attacker IP distribution
- Successful RDP logins
- Targeted user accounts

## Key Findings
- Detected brute-force attack patterns based on high-frequency login attempts
- Differentiated between normal user behavior and automated attack activity
- Identified successful compromise through RDP login
- Demonstrated log correlation and SIEM-based threat detection

## Screenshots
### Failed Login Attempts Over Time
<img width="1855" height="312" alt="image" src="https://github.com/user-attachments/assets/84fa0498-4cd5-45e5-8839-cce5debadcd2" />

### Attacker IP Distribution
<img width="1849" height="330" alt="image" src="https://github.com/user-attachments/assets/4e53ae7d-fbe3-4129-8d3f-03f5fe78b992" />

### Successful RDP Logins
<img width="1850" height="339" alt="image" src="https://github.com/user-attachments/assets/0fbf3d87-2a28-4320-9fef-a131cf555e47" />

### Targeted User Accounts
<img width="1855" height="328" alt="image" src="https://github.com/user-attachments/assets/4650114f-4917-444c-ab5b-fb7a60afa507" />

## Conclusion
This project demonstrates practical experience in detecting and analyzing brute-force attacks using SIEM tools, along with understanding authentication logs and security monitoring workflows.
