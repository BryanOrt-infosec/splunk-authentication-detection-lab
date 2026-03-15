\# Splunk Detection Queries



This file contains the SPL queries used in the authentication detection lab.



\---



\## 1. Search Failed Login Attempts



```spl

index=main EventCode=4625

