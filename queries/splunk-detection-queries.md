# Splunk Detection Queries

This document contains the Splunk SPL queries used to detect authentication activity within the lab environment.

---

# Failed Login Detection

Search for failed authentication attempts.


index=main EventCode=4625


Purpose:

Detect login failures that may indicate brute-force attempts.

---

# Successful Login Detection

Search for successful authentication events.


index=main EventCode=4624


Purpose:

Identify legitimate login activity.

---

# Failed Login Statistics by Account


index=main EventCode=4625
| stats count by Account_Name


Purpose:

Determine which accounts are receiving the highest number of failed login attempts.

---

# Password Spray Detection


index=main EventCode=4625
| stats count by Account_Name
| sort -count


Purpose:

Identify multiple authentication failures across different usernames.

---

# Advanced Authentication Analysis


index=main EventCode=4625
| stats count by Account_Name, host
| sort -count


Purpose:

Detect authentication attack patterns across accounts and systems.
