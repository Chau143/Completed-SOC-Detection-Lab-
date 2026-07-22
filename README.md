# Enterprise SOC Detection Lab | Splunk | Active Directory | Zeek | Suricata | pfSense

## Detection Lab Architecture 

<img width="1538" height="1232" alt="image" src="https://github.com/user-attachments/assets/1f967911-fcf0-4e28-a448-744687f5548f" />

#This project demonstrates the deployment of a complete enterprise Security Operations Center (SOC) detection lab. The environment simulates a corporate network where Windows endpoints generate security events, Zeek and Suricata monitor network traffic, Splunk centralizes log analysis, and Kali Linux emulates attacker activity using Atomic Red Team.

#Lab Components

-Active Directory

-pfSense Firewall

-Network Security Monitoring- Zeek&Suricata

-Centralized Log Management- Splunk Enterprise

-Adversary Emulation- Atomic Red Team

#The primary objective of this project is to conduct Adversary Emulation against Windows endpoints and engineer robust detection queries in Splunk Processing Language mapped directly to the MITRE ATT&CK Framework 

#Lab Setup 

## Installing pfSense Firewall - Configure pfSense as the gateway between the Internet and internal SOC lab network

<img width="1264" height="719" alt="{26BF22D7-39C8-470E-A01C-D60FFCC64102}" src="https://github.com/user-attachments/assets/8bee853d-90ac-472b-b35c-e7f690e3bb4e" />

<img width="1499" height="889" alt="{BC62E030-72F0-4222-A147-4612AA4121C0}" src="https://github.com/user-attachments/assets/adc0ebce-d37b-4ae5-beed-98472e585537" />


<img width="995" height="725" alt="{3CEB8419-9C27-4FF9-A795-C23FE44E71EB}" src="https://github.com/user-attachments/assets/faf7cba3-cb9f-4a67-a658-c2cf9e863d21" />



## Active Directory Controller - Built an enterprise Active Directory environment to simulate a Windows corporate network.


<img width="1171" height="825" alt="{CB728335-07C0-4E0A-B804-CB5ECA146B53}" src="https://github.com/user-attachments/assets/9e688dc5-52e7-4cf2-a8c6-c990bba9a273" />




## Windows 10 Joined to Domain - Joined a Windows endpoint to the Active Directory domain to simulate enterprise workstations.


## Configuring Windows Audit Policies - Enabled advanced Windows audit policies to generate detailed security telemetry for threat detection.

## Splunk Receiving Windows Security Logs - Verified successful ingestion of Windows Security logs into Splunk SIEM.




