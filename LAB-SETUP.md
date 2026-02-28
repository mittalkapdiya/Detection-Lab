# 🏗 Lab Setup

## Environment

- VirtualBox
- Windows 10 (Target Machine)
- Kali Linux (Attacker Machine)
- Internal Isolated Network

## Configuration Steps

1. Installed VirtualBox and created two virtual machines.
2. Configured Internal Network mode for safe attack simulation.
3. Installed Sysmon on Windows 10.
4. Installed and configured Splunk for log ingestion.
5. Forwarded Windows and Sysmon logs to Splunk.

This setup ensures safe malware execution without impacting the host system.
