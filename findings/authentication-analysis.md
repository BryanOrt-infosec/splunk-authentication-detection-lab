\# Authentication Analysis Findings



\## Summary



This file documents the findings from the Splunk authentication detection lab.



Windows Security logs were ingested into Splunk and analyzed to identify suspicious authentication activity. Two attack simulations were performed:



1\. Manual failed login attempts using the Windows lock screen

2\. Password spray simulation using the `runas` command



\---



\## Attack 1: Manual Failed Logins from Lock Screen



The workstation was locked and multiple incorrect passwords were entered for the local user account.



\### Result

\- Windows generated \*\*Event ID 4625\*\* for each failed login attempt

\- Splunk successfully ingested these logs

\- Failed logins were visible through direct searches and statistical queries



\### Detection Value

This activity simulates a simple brute-force style login attempt against a single account.



\---



\## Attack 2: Password Spray Simulation



A password spray attack was simulated using the Windows `runas` command with multiple usernames and the same password attempt.



Example:



```cmd

runas /user:test1 cmd

