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

<img width="1161" height="644" alt="{E30482C8-570E-4D2A-9AF9-254C92B02100}" src="https://github.com/user-attachments/assets/eb6178f2-8528-407f-af7e-b761434cdd0b" />

<img width="992" height="711" alt="{FA6BE8B4-1934-46B3-9923-7411765831A8}" src="https://github.com/user-attachments/assets/2e7304ee-b159-40f4-b151-fa2078dc910d" />

<img width="1013" height="726" alt="{88909BEC-F8EF-434C-A513-75093EA072FC}" src="https://github.com/user-attachments/assets/e2afe560-0089-4aa4-9436-bf969f45b73c" />




## Splunk Receiving Windows Security Logs - Verified successful ingestion of Windows Security logs into Splunk SIEM.

<img width="1015" height="415" alt="{3D6E39E6-01C0-4D11-A0AC-5B4F68072B86}" src="https://github.com/user-attachments/assets/a33989a0-0979-4935-a090-64208efad5a4" />

<img width="825" height="596" alt="{441B8D4B-604E-4B4E-81D7-F414DD246565}" src="https://github.com/user-attachments/assets/9aed0716-7f8e-4188-9f38-6659c3e35a2c" />

<img width="1019" height="724" alt="{A77B9268-0185-4FB5-A391-8433685A60F4}" src="https://github.com/user-attachments/assets/ebc9ace0-2e55-4532-9af0-d91dd518add8" />

## Zeek & Suricata Sensor - Configured Zeek and Suricata to capture network metadata and intrusion detection alerts.

<img width="1381" height="814" alt="{7320DFB5-2D10-4ECB-84EE-8F3D3A9C4719}" src="https://github.com/user-attachments/assets/9d0c8678-7a4d-4533-878e-ac00917e40f4" />

<img width="786" height="132" alt="{D8347483-E415-4AB2-8AB0-D5E561090261}" src="https://github.com/user-attachments/assets/3c742bcc-070c-48eb-a63a-55e835f2d729" />


## Splunk Network Telemetry - Network telemetry from Zeek and Suricata indexed into Splunk for centralized investigation.

<img width="1006" height="705" alt="{866B7735-D24A-495D-B34E-860F6B6DEDBA}" src="https://github.com/user-attachments/assets/9f643ad0-5f49-483f-bd0c-13f737cc496b" />

<img width="1041" height="732" alt="{6A9E3851-5E34-4638-98CA-E8BC41C104D1}" src="https://github.com/user-attachments/assets/6ac8a30e-edd0-4964-8e1b-03cd9f0d72db" />


## Kali Linux Attack Simulation - Hosted malicious payloads from Kali Linux to simulate attacker behavior within the lab.

<img width="632" height="126" alt="{986B319F-073D-4FAF-A045-EB369FF167C8}" src="https://github.com/user-attachments/assets/79ec2aee-476b-4430-bde7-56682144b252" />

## Malware Download Simulation - Simulated malware delivery over HTTP from the attacker machine to the Windows endpoint. 

<img width="1025" height="316" alt="{A16D2C69-5E37-4378-AD6A-D1224199A9C4}" src="https://github.com/user-attachments/assets/c4679a30-3fdc-491d-a4bd-8c00af92f358" />


## Atomic Red Team Execution - Executed Atomic Red Team tests to emulate MITRE ATT&CK techniques and generate realistic attack telemetry.

<img width="857" height="692" alt="{B7A66477-B69F-4DAB-AB25-B72574A0EE4C}" src="https://github.com/user-attachments/assets/5fd9f9b8-50eb-4beb-b7d1-64d3369e7f8d" />


## Splunk Detecting Atomic Red Team Activity - Investigated Windows process creation events generated during Atomic Red Team simulations.

<img width="1015" height="720" alt="{B2C87581-7E6A-49B5-9FF9-0BDBB0C7A747}" src="https://github.com/user-attachments/assets/c41a99d9-2233-4f2d-a48c-d52a25a999c3" />

<img width="1000" height="716" alt="{6F4F8519-2AF1-4FED-A22F-93A2F02CC9F0}" src="https://github.com/user-attachments/assets/fc6019ea-7c7b-47d0-8db2-181df03fb4b2" />

<img width="1019" height="714" alt="{B7296502-41DF-4BD1-8C07-37B734D60ACC}" src="https://github.com/user-attachments/assets/16ca0200-df98-4b11-9770-0d89048940f7" />

<img width="1021" height="725" alt="{689490C4-B88F-40DD-9E70-807377E48BE6}" src="https://github.com/user-attachments/assets/afb8bead-98a6-4356-9483-51035150a665" />

<img width="1006" height="723" alt="{D24246B5-22E1-45E6-B9F7-7B62EBCF2E8F}" src="https://github.com/user-attachments/assets/4942f5bb-5346-47fe-91ae-57dfcbb2888b" />


