# SOC-Home-Lab-Wazuh
SOC Home Lab using Wazuh SIEM, Ubuntu, and Windows 11 for security monitoring and threat detection.
# Exercise 01 – Windows Failed Login Detection

## Objective
Detect failed Windows login attempts using Wazuh SIEM.

## Lab Environment
- Ubuntu Linux – Wazuh Manager
- Windows 11 – Monitored Endpoint
- Kali Linux – Future Attacker Machine
- VMware Workstation

## Implementation
1. Installed Wazuh Manager on Ubuntu.
2. Installed Wazuh Agent on Windows 11.
3. Registered the Windows endpoint using an Authentication Key.
4. Verified that the Wazuh Agent status was Active.
5. Generated a failed login attempt on Windows 11.
6. Detected the event in Wazuh Dashboard.

## Detection Results

- Event: Logon Failure
- Windows Event ID: 4625
- Agent: SOC-Windows11
- Agent ID: 001
- Agent Status: Active

## Security Analysis

Windows Event ID 4625 indicates a failed login attempt.

Repeated failed login attempts may indicate a Brute Force Attack.

A SOC Analyst should investigate the username, source IP address, frequency of attempts, and any subsequent successful logins.

## Conclusion

Successfully connected a Windows 11 endpoint to Wazuh SIEM and detected a failed authentication event.

This exercise provided practical experience with endpoint monitoring and Windows security event analysis.

Status: Completed
## Screenshot – Failed Login Event

![Wazuh Failed Login Event](../Screenshot%202026-11-08%20094322.png)
