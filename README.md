# MITRE ATT&CK Data Sources
This repo contains my (Tareq's) work on MITRE ATT&CK data sources. Details about each section are included in the relevant Medium Blog posts.

## Data Sources Ordered By Collection Priority
The aim here is to create a prioritized list of data sources that is based on objective metrics. Full details are at the link below, but the general criteria for ordering are:
1. Prioritize sources that can be collected, for obvious reason.
1. Prioritize sources with lower volume. 
1. Prioritize sources that do not require collection from all hosts.
1. Prioritize sources by the number of subtechniques.
1. Prioritize source by the number of techniques.

https://medium.com/@tareq.alkhatib/are-we-using-mitre-att-ck-data-sources-wrong-13cac16d7531 

| Rank | Data Source | Sub Source | Collectable | Num of Sensors | Volume | Polymorphic | Num of Techniques | Num of Subtechniques | Notes |
|---|-----|-----|-----|-----|-----|-----|-----|-----|-----|
| 1 | Active Directory | Active Directory Object Modification | Yes | Domain Controllers | Low | FALSE | 7 | 13 |  |
| 2 | User Account | User Account Metadata | Yes | Domain Controllers | Low | FALSE | 4 | 8 | Assuming Domain Accounts |
| 3 | Container | Container Creation | Yes | Containers | Low | FALSE | 4 | 6 |  |
| 4 | User Account | User Account Modification | Yes | Domain Controllers | Low | FALSE | 3 | 6 | Assuming Domain Accounts |
| 5 | User Account | User Account Creation | Yes | Domain Controllers | Low | FALSE | 2 | 6 | Assuming Domain Accounts |
| 6 | Web Credentials | Web Credentials Usage | Yes | Domain Controllers | Low | FALSE | 2 | 6 |  |
| 7 | Instance | Instance Creation | Yes | Cloud API | Low | FALSE | 3 | 5 |  |
| 8 | Image | Image Creation | Yes | Cloud API | Low | FALSE | 3 | 4 |  |
| 9 | Active Directory | Active Directory Object Creation | Yes | Domain Controllers | Low | FALSE | 2 | 4 |  |
| 10 | Instance | Instance Start | Yes | Cloud API | Low | FALSE | 2 | 4 |  |
| 11 | Instance | Instance Metadata | Yes | Cloud API | Low | FALSE | 3 | 3 |  |
| 12 | Snapshot | Snapshot Creation | Yes | Cloud API | Low | FALSE | 2 | 3 |  |
| 13 | Active Directory | Active Directory Object Access | Yes | Domain Controllers | Low | FALSE | 2 | 3 |  |
| 14 | Instance | Instance Deletion | Yes | Cloud API | Low | FALSE | 2 | 3 |  |
| 15 | Container | Container Start | Yes | Containers | Low | FALSE | 2 | 3 |  |
| 16 | Web Credentials | Web Credentials Creation | Yes | Domain Controllers | Low | FALSE | 1 | 3 |  |
| 17 | Firewall | Firewall Disable | Yes | Firewalls | Low | FALSE | 1 | 3 | Assuming Network Firewalls |
| 18 | Firewall | Firewall Rule Modification | Yes | Firewalls | Low | FALSE | 1 | 3 |  |
| 19 | Cloud Storage | Cloud Storage Enumeration | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 20 | Cloud Storage | Cloud Storage Metadata | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 21 | Pod | Pod Metadata | Yes | Containers | Low | FALSE | 2 | 2 |  |
| 22 | Snapshot | Snapshot Deletion | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 23 | Snapshot | Snapshot Modification | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 24 | Cloud Service | Cloud Service Enumeration | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 25 | Volume | Volume Deletion | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| 26 | Image | Image Metadata | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| 27 | Cloud Service | Cloud Service Disable | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| 28 | Cloud Service | Cloud Service Modification | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| 29 | Active Directory | Active Directory Object Deletion | Yes | Domain Controllers | Low | FALSE | 1 | 2 |  |
| 30 | Instance | Instance Modification | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| 31 | Instance | Instance Stop | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| 32 | Group | Group Enumeration | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| 33 | Group | Group Metadata | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| 34 | Group | Group Modification | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| 35 | Firewall | Firewall Enumeration | Yes | Firewalls | Low | FALSE | 1 | 2 |  |
| 36 | Firewall | Firewall Metadata | Yes | Firewalls | Low | FALSE | 1 | 2 |  |
| 37 | Image | Image Modification | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 38 | User Account | User Account Deletion | Yes | Domain Controllers | Low | FALSE | 1 | 1 | Assuming Domain Accounts |
| 39 | Image | Image Deletion | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 40 | Cloud Storage | Cloud Storage Creation | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 41 | Cloud Storage | Cloud Storage Deletion | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 42 | Pod | Pod Creation | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 43 | Pod | Pod Enumeration | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 44 | Pod | Pod Modification | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 45 | Snapshot | Snapshot Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 46 | Snapshot | Snapshot Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 47 | Cloud Service | Cloud Service Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 48 | Instance | Instance Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 49 | Cluster | Cluster Metadata | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 50 | Container | Container Enumeration | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 51 | Container | Container Metadata | Yes | Containers | Low | FALSE | 1 | 1 |  |
| 52 | Volume | Volume Creation | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 53 | Volume | Volume Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 54 | Volume | Volume Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 55 | Volume | Volume Modification | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| 56 | Logon Session Creation | Logon Session Creation | Yes | All Hosts | Low | FALSE | 11 | 32 |  |
| 57 | Service | Service Creation | Yes | All Hosts | Low | FALSE | 6 | 15 |  |
| 58 | Sensor Health | Host Status | Yes | All Hosts | Low | FALSE | 5 | 15 |  |
| 59 | Service | Service Metadata | Yes | All Hosts | Low | FALSE | 7 | 12 |  |
| 60 | Driver | Driver Load | Yes | All Hosts | Low | FALSE | 5 | 10 |  |
| 61 | Logon Session Creation | Logon Session Metadata | Yes | All Hosts | Low | FALSE | 4 | 9 |  |
| 62 | Scheduled Job | Scheduled Job Creation | Yes | All Hosts | Low | FALSE | 1 | 7 |  |
| 63 | Drive | Drive Modification | Yes | All Hosts | Low | FALSE | 3 | 6 |  |
| 64 | Network Share | Network Share Access | Yes | All Hosts | Low | FALSE | 4 | 5 |  |
| 65 | Drive | Drive Access | Yes | All Hosts | Low | FALSE | 3 | 5 |  |
| 66 | Service | Service Modification | Yes | All Hosts | Low | FALSE | 1 | 5 |  |
| 67 | Drive | Drive Creation | Yes | All Hosts | Low | FALSE | 3 | 4 |  |
| 68 | Scheduled Job | Scheduled Job Metadata | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| 69 | Scheduled Job | Scheduled Job Modification | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| 70 | Kernel | Kernel Module Load | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| 71 | Driver | Driver Metadata | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| 72 | Network Traffic | Network Traffic Flow | Yes | Network Taps | High | FALSE | 38 | 82 |  |
| 73 | Network Traffic | Network Connection Creation | Yes | Network Taps | High | FALSE | 30 | 58 |  |
| 74 | User Account | User Account Authentication | Yes | Domain Controllers | High | FALSE | 7 | 20 | Assuming Domain Accounts |
| 75 | Active Directory | Active Directory Credential Request | Yes | Domain Controllers | High | FALSE | 2 | 7 |  |
| 76 | Cloud Storage | Cloud Storage Access | Yes | Cloud API | High | FALSE | 2 | 2 |  |
| 77 | Cloud Storage | Cloud Storage Modification | Yes | Cloud API | High | FALSE | 2 | 2 |  |
| 78 | Command | Command Execution | Yes | All Hosts | High | TRUE | 25 | 255 |  |
| 79 | Process | Process Creation | Yes | All Hosts | High | FALSE | 79 | 206 |  |
| 80 | File | File Modification | Yes | All Hosts | High | FALSE | 29 | 98 |  |
| 81 | File | File Creation | Yes | All Hosts | High | FALSE | 30 | 88 |  |
| 82 | Process | OS API Execution | Yes | All Hosts | High | FALSE | 40 | 78 |  |
| 83 | Windows Registry | Windows Registry Key Modification | Yes | All Hosts | High | FALSE | 19 | 58 |  |
| 84 | Module | Module Load | Yes | All Hosts | High | FALSE | 15 | 50 |  |
| 85 | File | File Access | Yes | All Hosts | High | FALSE | 22 | 46 |  |
| 86 | File | File Metadata | Yes | All Hosts | High | FALSE | 13 | 37 |  |
| 87 | Script | Script Execution | Yes | All Hosts | High | TRUE | 15 | 26 |  |
| 88 | Process | Process Access | Yes | All Hosts | High | FALSE | 6 | 18 |  |
| 89 | Windows Registry | Windows Registry Key Creation | Yes | All Hosts | High | FALSE | 8 | 17 |  |
| 90 | Process | Process Metadata | Yes | All Hosts | High | FALSE | 5 | 11 |  |
| 91 | File | File Deletion | Yes | All Hosts | High | FALSE | 5 | 10 |  |
| 92 | Process | Process Modification | Yes | All Hosts | High | TRUE | 2 | 9 |  |
| 93 | Windows Registry | Windows Registry Key Access | Yes | All Hosts | High | FALSE | 4 | 7 |  |
| 94 | Windows Registry | Windows Registry Key Deletion | Yes | All Hosts | High | FALSE | 3 | 4 |  |
| 95 | Process | Process Termination | Yes | All Hosts | High | FALSE | 2 | 3 |  |
| 96 | Firewall | Firewall Disable | Yes | All Hosts | High | FALSE | 1 | 3 | Assuming Host Firewalls |
| 97 | Firewall | Firewall Rule Modification | Yes | All Hosts | High | FALSE | 1 | 3 |  |
| 98 | WMI | WMI Creation | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| 99 | Firewall | Firewall Enumeration | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| 100 | Firewall | Firewall Metadata | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| 101 | Named Pipe | Named Pipe Meta Data | Yes | All Hosts | High | FALSE | 1 | 1 |  |
| 102 | Network Traffic | Network Traffic Content | Yes | Network Taps | Very High | FALSE | 44 | 96 |  |
| 103 | Application Log | Application Log Content | ? | ? | ? | FALSE | 25 | 55 | Varies by application |
| 104 | Internet Scan | Response Content | No | N/A | N/A | FALSE | 6 | 22 |  |
| 105 | Firmware | Firmware Modification | No | N/A | N/A | FALSE | 4 | 9 |  |
| 106 | Malware Repository | Malware Metadata | No | N/A | N/A | TRUE | 2 | 7 |  |
| 107 | Internet Scan | Response Metadata | No | N/A | N/A | FALSE | 2 | 6 |  |
| 108 | Domain Name | Active DNS | No | N/A | N/A | FALSE | 2 | 5 |  |
| 109 | Domain Name | Passive DNS | No | N/A | N/A | FALSE | 2 | 5 |  |
| 110 | Malware Repository | Malware Content | No | N/A | N/A | TRUE | 2 | 4 |  |
| 111 | Persona | Social Media | No | N/A | N/A | FALSE | 2 | 4 |  |
| 112 | Domain Name | Domain Registration | No | N/A | N/A | FALSE | 2 | 4 |  |
| 113 | Certificate | Certificate Registration | No | N/A | N/A | FALSE | 1 | 2 |  |

## Breakdown of the "Application Log" datasource

| Domain | Technique | Subtechnique | Name | Data Source |
|--------|-----------|--------------|------|-------------|
| Enterprise | T1098 | 0.002 | Account Manipulation: Exchange Email Delegate Permissions | Exchange Logs |
| Enterprise | T1110 |  | Brute Force | Application User Account Authentication |
|  |  | 0.001 | Password Guessing | Application User Account Authentication |
|  |  | 0.002 | Password Cracking | Application User Account Authentication |
|  |  | 0.003 | Password Spraying | Application User Account Authentication |
|  |  | 0.004 | Credential Stuffing | Application User Account Authentication |
| Enterprise | T1613 |  | Container and Resource Discovery | Effectively the "Containers" Platform |
| Enterprise | T1213 |  | Data from Information Repositories |  |
|  |  | 0.001 | Confluence | Confluence Logs |
|  |  | 0.002 | Sharepoint | Sharepoint Logs |
|  |  | 0.003 | Code Repositories | Code Repository Logs |
| Enterprise | T1491 |  | Defacement |  |
|  |  | 0.001 | Internal Defacement | Web Application Logs |
|  |  | 0.002 | External Defacement | Web Application Logs |
| Enterprise | T1610 |  | Deploy Container | Effectively the "Containers" Platform |
| Enterprise | T1189 |  | Drive-by Compromise | Proxy Logs |
| Enterprise | T1114 |  | Email Collection |  |
|  |  | 0.003 | Email Forwarding Rule | Mail Server Logs |
| Enterprise | T1499 |  | Endpoint Denial of Service |  |
|  |  | 0.002 | Service Exhaustion Flood | Effectively Application Health |
|  |  | 0.003 | Application Exhaustion Flood | Effectively Application Health |
|  |  | 0.004 | Application or System Exploitation | Effectively Application Health |
| Enterprise | T1190 |  | Exploit Public-Facing Application | Web Application Logs |
| Enterprise | T1210 |  | Exploitation of Remote Services | EDR / Sysmon |
| Enterprise | T1133 |  | External Remote Services | Remote Service Logon Logs |
| Enterprise | T1564 |  | Hide Artifacts |  |
|  |  | 0.008 | Email Hiding Rules | Email Client Logs |
| Enterprise | T1562 | 0.002 | Impair Defenses: Disable Windows Event Logging | Security Event ID 1102, System Event ID 104, Service Control Manager Event ID 7035 |
| Enterprise | T1534 |  | Internal Spearphishing | Mail Server Logs |
| Enterprise | T1137 |  | Office Application Startup |  |
|  |  | 0.003 | Outlook Forms | Email Client Logs |
|  |  | 0.004 | Outlook Home Page | Email Client Logs |
|  |  | 0.005 | Outlook Rules | Email Client Logs |
| Enterprise | T1069 |  | Permission Groups Discovery | Container logs |
|  |  | 0.003 | Cloud Groups |  |
| Enterprise | T1566 |  | Phishing |  |
|  |  | 0.001 | Spearphishing Attachment | Mail Server Logs |
|  |  | 0.002 | Spearphishing Link | Mail Server Logs |
|  |  | 0.003 | Spearphishing via Service | Mail Server Logs |
| Enterprise | T1598 |  | Phishing for Information |  |
|  |  | 0.001 | Spearphishing Service | Mail Server Logs |
|  |  | 0.002 | Spearphishing Attachment | Mail Server Logs |
|  |  | 0.003 | Spearphishing Link | Mail Server Logs |
| Enterprise | T1594 |  | Search Victim-Owned Websites | Web Application Logs |
| Enterprise | T1505 |  | Server Software Component |  |
|  |  | 0.001 | SQL Stored Procedures | SQL Server Logs |
|  |  | 0.002 | Transport Agent | Exchange Logs |
|  |  | 0.003 | Web Shell | Web Application Logs |
| Enterprise | T1072 |  | Software Deployment Tools | Software Deployment Tool Logs |
| Enterprise | T1199 |  | Trusted Relationship | Not specified |
| Enterprise | T1550 |  | Use Alternate Authentication Material |  |
|  |  | 0.001 | Application Access Token | Web Application Logs |
|  |  | 0.004 | Web Session Cookie | Web Application Logs |
| Enterprise | T1204 |  | User Execution |  |
|  |  | 0.003 | Malicious Image | Not specified |