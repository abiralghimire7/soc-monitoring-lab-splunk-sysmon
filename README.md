# SOC Monitoring Lab – Splunk & Sysmon

This project demonstrates a small Security Operations Center (SOC) monitoring lab built using Sysmon and Splunk.

## Tools Used
- Splunk Enterprise
- Sysmon
- Splunk Universal Forwarder
- Windows 10 Virtual Machine

## Objectives
- Collect endpoint telemetry using Sysmon
- Send Windows event logs to Splunk
- Analyze logs using Splunk Processing Language (SPL)
- Detect suspicious command execution and authentication events

## Example Detection Query

index=main EventCode=1
| search CommandLine="*whoami*" OR CommandLine="*ipconfig*" OR CommandLine="*systeminfo*"

## Project Files
The full project documentation and screenshots are included in the repository.
## Full Project Documentation

You can view the full lab report here:

[Windows Endpoint Monitoring Lab](./Windows%20Endpoint%20Monitoring%20Lab.pdf)
