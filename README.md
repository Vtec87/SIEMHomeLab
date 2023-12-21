# SIEMHomeLab
<h1>Fortifying Digital Defenses: A Personal SIEM Implementation with Wazuh - Wazuh Lindoe Docker</h1>

 ### HyperlinkDoc.-[https://1drv.ms/w/s!AjoLJYJC2c5dnlesJYSCqkf7nspM?e=wvT2Ri)  

<h2>Introduction</h2>
**Description:**
Established a robust Security Information and Event Management (SIEM) environment using Wazuh within a Docker container hosted on Linode. Deployed agents on diverse platforms, including Windows 10, Ubuntu, Kali Linux, and Kali Purple, to monitor security configurations and promptly alert for potential vulnerabilities, malware, and unauthorized activities.
<br />

![yIL5s5O](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/57b9b4ca-f2ab-4f9c-8459-b7761974da38) 

**Key Features:**
- **Comprehensive Monitoring:**
  - Conducted continuous monitoring with Wazuh agents across multiple security aspects:
    - *File Integrity Monitoring:* Tracked changes in directories, provided alerts for file additions/removals, document edits, and Windows registry modifications.
    - *Vulnerability Detection:* Identified known vulnerabilities and malware threats on all monitored systems.
    - *Threat Response:* Enabled active response to cybersecurity threats, including:
      - *Brute Force Attack Detection:* Monitored and automatically blocked suspicious IP addresses.
      - *Log Analysis:* Analyzed logs for potential threats and anomalies.

**System Components:**
- **SIEM Server:**
  - *Platform:* Linode
  - *Operating System:* Ubuntu/Kali Linux
  - *Containerization:* Docker
  - *SIEM Tool:* Wazuh
- **Monitored Devices:**
  - *Operating Systems:* Windows 10, Ubuntu, Kali Linux, Kali Purple
- **Additional Tools:**
  - *PowerShell:* Utilized for automation and scripting tasks on Windows systems/VM.
  - *Virtual Machine:* Optional Oracle VM for specific requirements.

**Technical Specifications:**
- *System Requirements:* Minimum 4GB RAM for the server.

**Benefits:**
- **Enhanced Security Posture:**
  - Continuous monitoring and threat detection significantly improved overall security posture.
- **Early Threat Detection:**
  - Timely alerts for vulnerabilities, malware, and unauthorized activity facilitated prompt response actions.
- **Improved Visibility:**
  - Consolidated log analysis across various systems provided a comprehensive view of the security posture.
- **Active Threat Response:**
  - Automated responses to brute force attacks and other threats mitigated potential damage.

- <b>Wazuh-Open Source Tool</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>

