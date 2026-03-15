\# Evidence Summary



\## Evidence Collected



This folder contains supporting evidence related to the Splunk authentication detection lab.



\### Evidence Types

\- Splunk screenshots

\- Authentication event searches

\- Statistical detection results

\- Password spray simulation command execution



\---



\## Screenshots Included



1\. Splunk Search interface

2\. Failed login events (Event ID 4625)

3\. Successful login events (Event ID 4624)

4\. Failed login statistics by account name

5\. Alert view before password spray attack

6\. Password spray results across multiple accounts

7\. Sorted password spray statistics

8\. Host-based password spray analysis

9\. Command Prompt password spray simulation using `runas`



\---



\## Relevant Event IDs



\- \*\*4624\*\* — Successful logon

\- \*\*4625\*\* — Failed logon attempt



\---



\## Summary of Evidence



The evidence collected in this lab demonstrates that:



\- Splunk successfully ingested Windows Security logs

\- Failed authentication attempts were detected and searchable

\- Successful authentication events were also visible

\- Password spray activity could be identified across multiple usernames

\- SPL queries were effective in summarizing suspicious login patterns

