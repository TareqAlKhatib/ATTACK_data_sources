# MITRE ATT&CK Data Sources
This repo contains my (Tareq's) work on MITRE ATT&CK data sources. Details about each section are included in the relevant Medium Blog posts.

## Data Sources Ordered By Collection Priority
The aim here is to create a prioritized list of data sources that is based on objective metrics. Full details are at the link below, but the general criteria for ordering are:
1. Prioritize sources that can be collected, for obvious reason.
1. Prioritize sources with lower volume. 
1. Prioritize sources that do not require collection from all hosts.
1. Prioritize sources by the number of subtechniques.
1. Prioritize source by the number of techniques.

TODO: Link to Medium Post

| Data Source | Sub Source | Collectable | Num of Sensors | Volume | Polymorphic | Num of Techniques | Num of Subtechniques | Notes |
|-----|-----|-----|-----|-----|-----|-----|-----|-----|
| Active Directory | Active Directory Object Modification | Yes | Domain Controllers | Low | FALSE | 7 | 13 |  |
| User Account | User Account Metadata | Yes | Domain Controllers | Low | FALSE | 4 | 8 | Assuming Domain Accounts |
| Container | Container Creation | Yes | Containers | Low | FALSE | 4 | 6 |  |
| User Account | User Account Modification | Yes | Domain Controllers | Low | FALSE | 3 | 6 | Assuming Domain Accounts |
| User Account | User Account Creation | Yes | Domain Controllers | Low | FALSE | 2 | 6 | Assuming Domain Accounts |
| Web Credentials | Web Credentials Usage | Yes | Domain Controllers | Low | FALSE | 2 | 6 |  |
| Instance | Instance Creation | Yes | Cloud API | Low | FALSE | 3 | 5 |  |
| Image | Image Creation | Yes | Cloud API | Low | FALSE | 3 | 4 |  |
| Active Directory | Active Directory Object Creation | Yes | Domain Controllers | Low | FALSE | 2 | 4 |  |
| Instance | Instance Start | Yes | Cloud API | Low | FALSE | 2 | 4 |  |
| Instance | Instance Metadata | Yes | Cloud API | Low | FALSE | 3 | 3 |  |
| Snapshot | Snapshot Creation | Yes | Cloud API | Low | FALSE | 2 | 3 |  |
| Active Directory | Active Directory Object Access | Yes | Domain Controllers | Low | FALSE | 2 | 3 |  |
| Instance | Instance Deletion | Yes | Cloud API | Low | FALSE | 2 | 3 |  |
| Container | Container Start | Yes | Containers | Low | FALSE | 2 | 3 |  |
| Web Credentials | Web Credentials Creation | Yes | Domain Controllers | Low | FALSE | 1 | 3 |  |
| Firewall | Firewall Disable | Yes | Firewalls | Low | FALSE | 1 | 3 | Assuming Network Firewalls |
| Firewall | Firewall Rule Modification | Yes | Firewalls | Low | FALSE | 1 | 3 |  |
| Cloud Storage | Cloud Storage Enumeration | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Cloud Storage | Cloud Storage Metadata | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Pod | Pod Metadata | Yes | Containers | Low | FALSE | 2 | 2 |  |
| Snapshot | Snapshot Deletion | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Snapshot | Snapshot Modification | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Cloud Service | Cloud Service Enumeration | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Volume | Volume Deletion | Yes | Cloud API | Low | FALSE | 2 | 2 |  |
| Image | Image Metadata | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| Cloud Service | Cloud Service Disable | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| Cloud Service | Cloud Service Modification | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| Active Directory | Active Directory Object Deletion | Yes | Domain Controllers | Low | FALSE | 1 | 2 |  |
| Instance | Instance Modification | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| Instance | Instance Stop | Yes | Cloud API | Low | FALSE | 1 | 2 |  |
| Group | Group Enumeration | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| Group | Group Metadata | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| Group | Group Modification | Yes | Domain Controllers | Low | FALSE | 1 | 2 | Assuming Domain Accounts |
| Firewall | Firewall Enumeration | Yes | Firewalls | Low | FALSE | 1 | 2 |  |
| Firewall | Firewall Metadata | Yes | Firewalls | Low | FALSE | 1 | 2 |  |
| Image | Image Modification | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| User Account | User Account Deletion | Yes | Domain Controllers | Low | FALSE | 1 | 1 | Assuming Domain Accounts |
| Image | Image Deletion | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Cloud Storage | Cloud Storage Creation | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Cloud Storage | Cloud Storage Deletion | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Pod | Pod Creation | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Pod | Pod Enumeration | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Pod | Pod Modification | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Snapshot | Snapshot Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Snapshot | Snapshot Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Cloud Service | Cloud Service Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Instance | Instance Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Cluster | Cluster Metadata | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Container | Container Enumeration | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Container | Container Metadata | Yes | Containers | Low | FALSE | 1 | 1 |  |
| Volume | Volume Creation | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Volume | Volume Enumeration | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Volume | Volume Metadata | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Volume | Volume Modification | Yes | Cloud API | Low | FALSE | 1 | 1 |  |
| Logon Session Creation | Logon Session Creation | Yes | All Hosts | Low | FALSE | 11 | 32 |  |
| Service | Service Creation | Yes | All Hosts | Low | FALSE | 6 | 15 |  |
| Sensor Health | Host Status | Yes | All Hosts | Low | FALSE | 5 | 15 |  |
| Service | Service Metadata | Yes | All Hosts | Low | FALSE | 7 | 12 |  |
| Driver | Driver Load | Yes | All Hosts | Low | FALSE | 5 | 10 |  |
| Logon Session Creation | Logon Session Metadata | Yes | All Hosts | Low | FALSE | 4 | 9 |  |
| Scheduled Job | Scheduled Job Creation | Yes | All Hosts | Low | FALSE | 1 | 7 |  |
| Drive | Drive Modification | Yes | All Hosts | Low | FALSE | 3 | 6 |  |
| Network Share | Network Share Access | Yes | All Hosts | Low | FALSE | 4 | 5 |  |
| Drive | Drive Access | Yes | All Hosts | Low | FALSE | 3 | 5 |  |
| Service | Service Modification | Yes | All Hosts | Low | FALSE | 1 | 5 |  |
| Drive | Drive Creation | Yes | All Hosts | Low | FALSE | 3 | 4 |  |
| Scheduled Job | Scheduled Job Metadata | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| Scheduled Job | Scheduled Job Modification | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| Kernel | Kernel Module Load | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| Driver | Driver Metadata | Yes | All Hosts | Low | FALSE | 1 | 2 |  |
| Network Traffic | Network Traffic Flow | Yes | Network Taps | High | FALSE | 38 | 82 |  |
| Network Traffic | Network Connection Creation | Yes | Network Taps | High | FALSE | 30 | 58 |  |
| User Account | User Account Authentication | Yes | Domain Controllers | High | FALSE | 7 | 20 | Assuming Domain Accounts |
| Active Directory | Active Directory Credential Request | Yes | Domain Controllers | High | FALSE | 2 | 7 |  |
| Cloud Storage | Cloud Storage Access | Yes | Cloud API | High | FALSE | 2 | 2 |  |
| Cloud Storage | Cloud Storage Modification | Yes | Cloud API | High | FALSE | 2 | 2 |  |
| Command | Command Execution | Yes | All Hosts | High | TRUE | 25 | 255 |  |
| Process | Process Creation | Yes | All Hosts | High | FALSE | 79 | 206 |  |
| File | File Modification | Yes | All Hosts | High | FALSE | 29 | 98 |  |
| File | File Creation | Yes | All Hosts | High | FALSE | 30 | 88 |  |
| Process | OS API Execution | Yes | All Hosts | High | FALSE | 40 | 78 |  |
| Windows Registry | Windows Registry Key Modification | Yes | All Hosts | High | FALSE | 19 | 58 |  |
| Module | Module Load | Yes | All Hosts | High | FALSE | 15 | 50 |  |
| File | File Access | Yes | All Hosts | High | FALSE | 22 | 46 |  |
| File | File Metadata | Yes | All Hosts | High | FALSE | 13 | 37 |  |
| Script | Script Execution | Yes | All Hosts | High | TRUE | 15 | 26 |  |
| Process | Process Access | Yes | All Hosts | High | FALSE | 6 | 18 |  |
| Windows Registry | Windows Registry Key Creation | Yes | All Hosts | High | FALSE | 8 | 17 |  |
| Process | Process Metadata | Yes | All Hosts | High | FALSE | 5 | 11 |  |
| File | File Deletion | Yes | All Hosts | High | FALSE | 5 | 10 |  |
| Process | Process Modification | Yes | All Hosts | High | TRUE | 2 | 9 |  |
| Windows Registry | Windows Registry Key Access | Yes | All Hosts | High | FALSE | 4 | 7 |  |
| Windows Registry | Windows Registry Key Deletion | Yes | All Hosts | High | FALSE | 3 | 4 |  |
| Process | Process Termination | Yes | All Hosts | High | FALSE | 2 | 3 |  |
| Firewall | Firewall Disable | Yes | All Hosts | High | FALSE | 1 | 3 | Assuming Host Firewalls |
| Firewall | Firewall Rule Modification | Yes | All Hosts | High | FALSE | 1 | 3 |  |
| WMI | WMI Creation | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| Firewall | Firewall Enumeration | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| Firewall | Firewall Metadata | Yes | All Hosts | High | FALSE | 1 | 2 |  |
| Named Pipe | Named Pipe Meta Data | Yes | All Hosts | High | FALSE | 1 | 1 |  |
| Network Traffic | Network Traffic Content | Yes | Network Taps | Very High | FALSE | 44 | 96 |  |
| Application Log | Application Log Content | ? | ? | ? | FALSE | 25 | 55 | Varies by application |
| Internet Scan | Response Content | No | N/A | N/A | FALSE | 6 | 22 |  |
| Firmware | Firmware Modification | No | N/A | N/A | FALSE | 4 | 9 |  |
| Malware Repository | Malware Metadata | No | N/A | N/A | TRUE | 2 | 7 |  |
| Internet Scan | Response Metadata | No | N/A | N/A | FALSE | 2 | 6 |  |
| Domain Name | Active DNS | No | N/A | N/A | FALSE | 2 | 5 |  |
| Domain Name | Passive DNS | No | N/A | N/A | FALSE | 2 | 5 |  |
| Malware Repository | Malware Content | No | N/A | N/A | TRUE | 2 | 4 |  |
| Persona | Social Media | No | N/A | N/A | FALSE | 2 | 4 |  |
| Domain Name | Domain Registration | No | N/A | N/A | FALSE | 2 | 4 |  |
| Certificate | Certificate Registration | No | N/A | N/A | FALSE | 1 | 2 |  |