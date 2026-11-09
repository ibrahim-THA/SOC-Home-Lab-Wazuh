
# Exercise 02 – Brute Force Detection

## Objective
Detect multiple failed Windows login attempts using Wazuh SIEM.

## Environment
- Ubuntu 26.04 – Wazuh Manager
- Windows 11 – Wazuh Agent
- VMware Workstation

## Configuration
Created a custom Wazuh detection rule:

- Rule ID: 100100
- Level: 10
- Frequency: 5
- Timeframe: 60 seconds
- Matched Rule: 60122

## Testing
Generated multiple failed login attempts on Windows 11.

## Results
Wazuh successfully detected the activity and generated the alert:

Possible Brute Force Attack

## Conclusion
Successfully configured and tested a custom Wazuh rule
to detect repeated failed Windows login attempts.

## Evidence

<img width="1207" height="682" alt="Screenshot 2026-11-09 144409" src="https://github.com/user-attachments/assets/99a2c673-7a52-44c5-b38e-73cdea736e61" />
