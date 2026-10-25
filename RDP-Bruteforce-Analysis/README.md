
SOC Tier 1 — Incident Ticket

Incident ID: SOC-2026-001
Alert: Multiple Failed Logons
Severity: Medium
Status: Escalated for Review

1. Summary

Multiple failed login attempts were detected against the account drip on host DESKTOP-VFPAAJN.

2. Evidence

Source IP: 192.168.178.153

Target Host: DESKTOP-VFPAAJN

Event ID: 4625

Logon Type: 3 (Network)

Failed Attempts: Multiple attempts, including 136 in one configured time bucket.

3. Investigation

Reviewed Windows authentication logs in Splunk and searched for successful login events between 21:10 and 22:51. No successful authentication was identified in the reviewed period.

4. Verdict

True Positive — Suspicious Brute-Force Activity

Repeated failed logins indicate suspicious password-guessing activity. Account compromise was not confirmed.

5. Actions Taken

Reviewed failed authentication events in Splunk.

Checked for successful authentication during the investigated period.

Documented the source IP, target host, and relevant event details.

6. Next Steps

Recommend further investigation according to SOC procedures. Review related authentication activity and determine whether additional containment actions are required.
