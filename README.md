# Incident Investigation Using the Splunk BOTS Dataset

## Project Overview

This project focuses on performing a log-based security investigation using Splunk Enterprise and the Boss of the SOC (BOTS) Version 2 dataset.

The objective was to analyze security events, identify suspicious external IP addresses, investigate unusual request patterns, and understand potential attack activity through log analysis.

## Tools & Technologies

- Splunk Enterprise 10.6
- Boss of the SOC (BOTS) Version 2 Dataset
- Search Processing Language (SPL)
- Security Monitoring
- [SIEM](https://en.wikipedia.org/wiki/Security_information_and_event_management)

## Investigation Findings

During the investigation, the following suspicious activities were identified:

 - **Suspicious IP Address:**"45.77.65.211"
- **Target IP Address:** "172.31.4.249"
- **Request Count:** 8,966 requests from the suspicious IP.
- **User-Agent:**"w3af.org", associated with automated vulnerability scanning.
- **Targeted Pages:** "/member.php" and "/search.php"
- **Activity Period:** Approximately one hour on August 11, 2017, around 14:00.

The suspicious IP generated significantly more requests than other external IP addresses, indicating potentially automated scanning activity.

## Investigation Process

1. Loaded and verified the BOTS Version 2 dataset in Splunk.
2. Analyzed top source IP addresses.
3. Identified normal internal network traffic.
4. Separated internal IP addresses from external IP addresses.
5. Investigated suspicious IP activity and request patterns.
6. Analyzed targeted web pages and user-agent information.
7. Reviewed the event timeline to understand the activity.
8. Created a Splunk dashboard to visualize investigation findings.

## Project Files
```bash
01_Dataset_Loaded.png
```
```bash
02_Top_Source_IPs.png
```
```bash
03_Suspicious_IP_Activity.png
```
```bash
04_External_IPs.png
```
```bash
05_Attack_Pattern.png
```
```bash
06_Attack_Timeline.png
```
```bash
07_Dashboard.png
```

## Key Learnings

Through this project, I gained practical experience in:

- Searching and analyzing security logs using Splunk.
- Writing SPL queries for security investigations.
- Identifying suspicious IP addresses.
- Understanding automated scanning activity.
- Analyzing HTTP requests and user-agent information.
- Building dashboards for security monitoring.
- Investigating suspicious events using log data.

## Conclusion

This project helped me understand how SIEM tools like Splunk are used in Security Operations Centers (SOCs) for [security](https://en.wikipedia.org/wiki/Computer_security) monitoring, suspicious activity detection, and [Incident Investigation](https://en.wikipedia.org/wiki/Incident_management)

It provided hands-on experience with security data and improved my understanding of basic SOC investigation workflows.

## Project Domain

Cybersecurity | SOC Monitoring | SIEM | Incident Investigation

---

**Created by:** Sachin Kumar
