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


<img width="1165" height="810" alt="{FB11700A-5194-43F7-B0C8-AF5AC7734D9E}" src="https://github.com/user-attachments/assets/d1c8c7fb-1f83-4d41-a867-73fe90644613" />

<img width="1175" height="871" alt="{CD0BA834-4B42-49D4-A3A5-2F0EAFC88913}" src="https://github.com/user-attachments/assets/dbe9eb3a-09d3-4c5a-9209-92aa6a882a3d" />

<img width="1152" height="799" alt="{CA6B3603-5B5E-41E7-BED3-833B6310E0C3}" src="https://github.com/user-attachments/assets/512c94e7-da56-42e2-bf9c-5beb109dba24" />






## Windows 10 Joined to Domain - Joined a Windows endpoint to the Active Directory domain to simulate enterprise workstations.

<img width="1398" height="872" alt="{EB5DA3A9-F641-487D-A414-F99C37049D03}" src="https://github.com/user-attachments/assets/7bd2f561-e811-4433-b91f-48bfa5813773" />

<img width="1431" height="883" alt="{8AF8BFBF-87EA-4520-879C-ABE5B03A149E}" src="https://github.com/user-attachments/assets/e7dd8254-5163-4ceb-905b-d5abf4a47edf" />



## Configuring Windows Audit Policies - Enabled advanced Windows audit policies to generate detailed security telemetry for threat detection.

<img width="1160" height="830" alt="{3C87EE28-9213-4CAE-83CF-0200D6E60824}" src="https://github.com/user-attachments/assets/b7974dd7-de23-42ec-90e3-8ba72907c1f8" />

<img width="897" height="614" alt="{A8DF0B07-189B-496F-8EE7-7C837FCB7879}" src="https://github.com/user-attachments/assets/fe76e058-fa93-4c8a-8bfb-15cd0988b254" />

<img width="895" height="617" alt="{F94D29E8-D4B8-41EB-A477-D514365C3975}" src="https://github.com/user-attachments/assets/6e3faae9-799e-43be-bcc4-729862db934f" />

<img width="898" height="620" alt="{CD9E91D8-C135-409C-B01A-6041E61303B6}" src="https://github.com/user-attachments/assets/20df7f74-5c26-4abb-ab73-19f6e8c7b4f5" />

<img width="892" height="614" alt="{CD555D8C-5E46-484E-88BE-15BC84950382}" src="https://github.com/user-attachments/assets/cb9aa39e-1c93-4990-addf-ea0ac5f6cdc2" />

<img width="898" height="610" alt="{50509F0F-26B4-44DC-9BD7-0ECF2083AFA6}" src="https://github.com/user-attachments/assets/febd7fbe-6ec9-4509-a3b6-36b215e44e76" />

<img width="905" height="644" alt="{B2EBA55E-2484-444B-BACA-207E1DF63595}" src="https://github.com/user-attachments/assets/6fa85402-ef52-4d4e-b80a-7217087223ac" />




## Splunk Receiving Windows Security Logs - Verified successful ingestion of Windows Security logs into Splunk SIEM.


## Zeek & Suricata Sensor - Configured Zeek and Suricata to capture network metadata and intrusion detection alerts.

## Splunk Network Telemetry - Network telemetry from Zeek and Suricata indexed into Splunk for centralized investigation.

## Kali Linux Attack Simulation - Hosted malicious payloads from Kali Linux to simulate attacker behavior within the lab.

## Atomic Red Team Execution - Executed Atomic Red Team tests to emulate MITRE ATT&CK techniques and generate realistic attack telemetry.

## Splunk Detecting Atomic Red Team Activity - Investigated Windows process creation events generated during Atomic Red Team simulations.



