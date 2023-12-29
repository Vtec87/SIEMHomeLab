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

**Call to Action:**

Ready to fortify your digital defenses? Download the comprehensive lab guide for an immersive learning experience. Stay updated with additional insights by following Victor Patterson Sr.

*Warning: This lab is FUN! But buckle up for a delightful journey.*
**Launching the Journey: Setting Up Linode**

*Created and Completed by Victor Patterson Sr.*

**Introduction:**

Embark on an exciting journey as we dive into the intricacies of setting up Linode—a crucial initial step in fortifying our digital defenses. In this guide, I'll walk you through the installation process, laying the foundation for our comprehensive Security Information and Event Management (SIEM) lab.

**Step 1: Downloading Linode**

Your adventure begins with downloading Linode, a pivotal platform for our SIEM implementation. Follow the hyperlink below to initiate the download:

[Download Linode](https://www.linode.com) 

**Step 2: Installation Process**

After setting up your Linode account, the installation process unfolds. The home screen post-installation will resemble the screenshot below, marking the commencement of our cybersecurity exploration.



**Additional Insights:**

- **Visual Companion:**
  - For a visual guide through each step, refer to the accompanying screenshots.

- **Target Audience:**
  - Ideal for both beginners and seasoned tech enthusiasts ready to strengthen their digital defenses.
