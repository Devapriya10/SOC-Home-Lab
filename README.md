# Home SOC Lab using Splunk Enterprise & Kali Linux

## Overview
This project demonstrates a Home SOC Lab built using Splunk Enterprise and Kali Linux for centralized log monitoring and security analysis.

## Features
- Log forwarding using Splunk Universal Forwarder
- Authentication log monitoring
- Brute-force attack simulation
- SPL query analysis
- Security event investigation

## Technologies Used
- Splunk Enterprise
- Splunk Universal Forwarder
- Kali Linux
- Windows
- SPL (Search Processing Language)

## Project Workflow
1. Installed Splunk Enterprise on Windows
2. Configured receiving port 9997
3. Installed Splunk Universal Forwarder on Kali Linux
4. Forwarded `/var/log/auth.log`
5. Simulated SSH brute-force attempts
6. Analyzed logs using SPL queries

## Sample SPL Query

```spl
host=kali "Failed password" source="/var/log/auth.log"
