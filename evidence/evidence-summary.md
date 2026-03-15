# Evidence Summary

This document summarizes the supporting evidence collected during the **Splunk Authentication Detection Lab**.

The evidence consists of authentication logs generated from simulated attacks and analyzed using Splunk.

---

# Evidence Collected

The following artifacts were collected during the investigation:

| Evidence Type | Description |
|---------------|-------------|
| Splunk Search Interface | Screenshot of Splunk search dashboard |
| Event ID 4625 Logs | Failed authentication attempts |
| Event ID 4624 Logs | Successful login events |
| Authentication Statistics | Failed login counts grouped by account |
| Alert Status | Splunk alert state before attack simulation |
| Password Spray Results | Authentication failures across multiple accounts |
| Host Analysis | Detection results grouped by account and host |
| Attack Simulation | Password spray attack executed using runas |

---

# Screenshots Included

1. Splunk Search Interface  
2. Failed Login Events (4625)  
3. Successful Login Events (4624)  
4. Failed Login Statistics by Account  
5. Alert Status Before Attack  
6. Password Spray Results Across Accounts  
7. Password Spray Detection Statistics  
8. Host and Account Analysis  
9. Password Spray Command Execution

---

# Purpose of Evidence

The collected evidence demonstrates how authentication attack simulations generate Windows Security logs that can be detected using SIEM monitoring.

These artifacts support the findings documented in the investigation report.
