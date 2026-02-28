# 🕵 Investigation Process

## Step 1: Alert Triggered
Detected multiple failed login attempts from a single IP address.

## Step 2: Log Correlation
Reviewed:
- Windows Security Event ID 4625
- Sysmon Event ID 1 (Process Creation)
- Sysmon Event ID 3 (Network Connection)

## Step 3: Root Cause Analysis
Identified suspicious process execution followed by outbound network connection consistent with reverse shell behavior.

## Step 4: Conclusion
Attack successfully simulated and detected using SIEM queries and log correlation techniques.
