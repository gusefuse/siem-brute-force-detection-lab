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

## Conclusion
This project demonstrates practical experience in detecting and analyzing brute-force attacks using SIEM tools, along with understanding authentication logs and security monitoring workflows.
