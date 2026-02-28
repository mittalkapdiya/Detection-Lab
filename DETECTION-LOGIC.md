# 🔍 Detection Logic

## Brute Force Detection (Failed Logins)

index=wineventlog EventCode=4625
| stats count by Account_Name, Source_Network_Address
| where count > 5

## Suspicious Process Creation (Sysmon Event ID 1)

index=sysmon EventCode=1
| stats count by ParentImage, Image

## Reverse Shell Network Detection (Sysmon Event ID 3)

index=sysmon EventCode=3
| stats count by SourceIp, DestinationIp

Detection focused on identifying:
- Multiple failed logins
- Suspicious parent-child process chains
- Unusual outbound network connections
