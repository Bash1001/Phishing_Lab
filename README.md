# Phishing_Lab
Real scenario to detect phishing attack


## Objective

## Objective

To simulate and investigate a phishing attack where a malicious ODS LibreOffice file (Similar to Microsoft Office) containing a macro is used to download and execute a PowerShell payload, ultimately giving the attacker remote access. This exercise demonstrates the detection and response process using Splunk and endpoint telemetry

### Skills Learned

- Simulating phishing scenarios with macro-based payload delivery
- Detecting malicious process chains in endpoint telemetry
- Correlating Sysmon Event IDs (1, 3, 11) for full attack visibility
- Building Splunk queries for phishing detection
- Performing containment, eradication, and recovery actions
- Creating basic alerting logic in Splunk

### Tools Used

- SIEM for log collection and analysis                -> Splunk
- Windows logging for detailed telemetry              -> Sysmon
- Forwarding logs to Splunk                           -> 
- Crafting macro-enabled document                     -> Libre Office
- Attacker machine                                    -> Kali Linux
- Payload creation                                    -> msfvenom
- Hosting the malicious payload                       -> Python HTTP Server
- Reverse shell listener                              -> Metasploit


### Skills Learned

- Threat detection and incident analysis using SIEM (Splunk).
- Log correlation and parsing with Sysmon logs.
- Hands-on experience with offensive tools (Nmap, Metasploit, msfvenom).
- Windows process and registry behavior analysis.
- Basic knowledge of attack techniques aligned with MITRE ATT&CK (e.g., process injection, reverse shell).
- Building and maintaining a virtual home lab for cybersecurity training.



## Steps

<img width="1920" height="1080" alt="create Payload" src="https://github.com/user-attachments/assets/5fe9a64d-4fd0-4675-aed2-5f121f4da8e2" />
Create Payload


<img width="1920" height="1080" alt="Listening on kali kinux" src="https://github.com/user-attachments/assets/eb598378-d9ab-4216-954a-47631a0d0e1a" />
Listening on kali linux


<img width="1920" height="1080" alt="open local server" src="https://github.com/user-attachments/assets/046c5d2c-507b-4dc3-99ea-176b779e49c3" />
Open Local Server - Python

<img width="1920" height="1080" alt="Process Creation " src="https://github.com/user-attachments/assets/0c6fb915-7e78-4490-9aba-540f062e2f04" />
Analysis of newly created processes With event = 1



<img width="1920" height="1080" alt="Network Connection" src="https://github.com/user-attachments/assets/4e6b3526-e031-4735-b916-fbf3651db539" />
Network Connection With event = 3

<img width="1920" height="1080" alt="create files" src="https://github.com/user-attachments/assets/1bfda592-2aeb-47de-9ab5-9dfb4d09f212" />
Files Creation Analysis With event = 11


<img width="1920" height="1080" alt="Macro setting" src="https://github.com/user-attachments/assets/8d28a0fe-ac7d-4de1-8556-d45b3652614f" />
Mcaro Setting to 


<img width="1920" height="1080" alt="Isolating the affected device" src="https://github.com/user-attachments/assets/f821a5cc-8ee1-4b97-9eaf-9484fa99b6b3" />

<img width="1920" height="1080" alt="Isolating the affected device 2" src="https://github.com/user-attachments/assets/2a79b85c-4c8d-489c-bf5a-da2f27e5f184" />
Isolating Affected Device



<img width="1920" height="1080" alt="schedual task " src="https://github.com/user-attachments/assets/e95ccae8-b573-4650-8dad-81f14dd268a8" />
Check Schedual Task 




Because the video is large, I uploaded it to LinkedIn - This video shows the stage of exploitation
[http://linkedin.com/in](https://www.linkedin.com/posts/bashir-hasabelnabi_cybersecurity-soc-siem-activity-7353506367854256131-9WJr?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFwzdDIBWE1WjziZuD20Duh9ttAddbZavQA)

[http://linkedin.com/in](https://www.linkedin.com/posts/bashir-hasabelnabi_cybersecurity-soc-siem-activity-7353507192450211840-_PxT?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFwzdDIBWE1WjziZuD20Duh9ttAddbZavQA)

