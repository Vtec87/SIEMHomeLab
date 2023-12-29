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
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/d24ef5bc-9633-4abc-9cf5-1ffa6d8cffc9)

**Step 2: Installation Process**

After setting up your Linode account, the installation process unfolds. The home screen post-installation will resemble the screenshot below, marking the commencement of our cybersecurity exploration.
**Why Linode 4GB?**
For your digital dominion, the Linode 4GB plan provides substantial space and power. It's not just a plan; it's the infrastructure for your cybersecurity ascendancy.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/5fcd8e5d-d1ac-44d8-bc10-60fd01de523c)



**Additional Insights:**

- **Visual Companion:**
  - For a visual guide through each step, refer to the accompanying screenshots.

- **Target Audience:**
  - Ideal for both beginners and seasoned tech enthusiasts ready to strengthen their digital defenses.

2. **Explore the Marketplace for Wazuh:**
   - Head to the Marketplace and embark on a search for Wazuh, your trusty open-source cybersecurity companion, tailored for Security Information and Event Management (SIEM) practices.

![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/950da2c6-5901-4ce6-a85a-e263e4bb04f4)
**Step 2: Configuring Linode and Unveiling Wazuh**
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/395eec3e-020b-488d-bd1f-5c97b758bf39)
**Why Wazuh?**
Wazuh stands as a stalwart defender, vigilant in monitoring security events and offering real-time insights into potential threats. Integrating Wazuh into our lab promises to elevate our cybersecurity defenses

**Additional Insights:**

- **Comprehensive Cybersecurity:**
  - Gain a deeper understanding of Wazuh's pivotal role in fortifying your digital infrastructure against evolving threats.
**Step 3: Crafting Your Cyber Stronghold with Ubuntu on Linode**

*Forge Ahead with Your Cybersecurity Citadel*

2. **Secure Networking Rendezvous – SSH Access:**
   - Witness the Secure Shell (SSH) extending its virtual arms, offering secure passage into your cyber dominion. Ready your credentials; the gateway awaits.

*Celebrate this achievement, Cyber Sentinel! Your VM stands proud in the cloud, and the dance of Secure Shell beckons for your networking symphony.*

**Why This Matters:**
The successful establishment of your VM in the cloud marks a significant milestone. SSH access paves the way for secure interactions with your cyber creation, heralding a new era in your cybersecurity odyssey.

*Forge ahead, Cyber Sentinel, for Step 6 awaits – the initiation of Wazuh, your vigilant guardian in the realm of Security Information and Event Management (SIEM).*
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/8877875d-7dc6-4cc6-8a97-d335205ea727)
**Step 6: Commanding Your Cyber Minions – SSH Access Key Conquest**

*Powering Up with SSH Mastery*

Great strides, Cyber Maestro! As your Cloud VM stands tall, the time has come to wield the mighty SSH key, granting you command over your digital realm.

**Technical Level: Novice to Intermediate**
1. **Conquering the SSH Access Key:**
   - Behold your key to the kingdom! Copy your SSH Access Key: `ssh root@172.234.29.112`. This cryptographic gem shall open the gateway to your Cloud VM.

2. **Command Center Unveiled – Terminal Convergence:**
   - Rally your forces! Open your chosen terminal – whether PowerShell, Command Prompt, or the sacred realms of Linux. I, Cyber Sentinel, chose the illustrious Admin PowerShell on Win11.

3. **Majestic Key Unleashed – SSH Access Granted:**
   - With a flourish, paste your SSH access key into the terminal. Watch as the gates swing open, welcoming you into the heart of your cyber dominion.

**Security Reminder:**
The SSH key is your digital scepter, and with great power comes great responsibility. Never share or publicly display your SSH key. Guard it as you would the crown jewels.

**Optional Customization:**
Feel the urge to personalize? Explore customizing your terminal prompts and environments to truly make your cyber realm your own.

*Revel in this moment, Cyber Maestro! Your commands echo through the virtual corridors, and Step 7 beckons – the initiation of Wazuh, the vigilant guardian of Security Information and Event Management 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/48911084-629d-41df-bdc0-66a626dd8895) 
As you navigate through the digital expanse of your Cloud VM, savor the authority at your fingertips. Forge ahead with confidence, for the next chapter awaits – the initiation of Wazuh, the vigilant guardian of Security Information and Event Management (SIEM). Onward! 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/d7f1d32d-c11c-444e-8dff-50ccf64adeeb)

"I proficiently use the `htop` command, an interactive system monitor, process viewer, and process manager. This allows me to effectively monitor and manage system processes in real-time."
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/404c588c-8da8-47e2-ab3a-8380be740b4c)
"After successfully logging in with my password, I observed the DPKG (also referred to as the Debian Package) process in Linux actively installing."
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/e5dbaf32-45b2-4f48-b722-dad1f52130bb)
"To exit, press Ctrl+C to return to the main menu. Next, I will retrieve my password by entering 'ls -al' in the terminal." 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/5d4f55b7-81c4-43e1-a8ee-bd0f2bb35d43)
"You should find a file named '.deployment-secrets.txt'. This file contains the secrets, including my passwords." ![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/bdd2a77f-8eac-4769-84a6-808b867dd14e)
cat .deployment-secrets.txt
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/4bffdc37-09af-400a-b9c0-8f80001c10cb)
"Upon success, I encountered a screen displaying my passwords, similar to the one shown here
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/7df6130e-7114-4241-98b3-c1751699a351)
"The specific password I'm looking for is the administrator password, as indicated in the display."
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/8ba8298f-5adb-4def-add1-7d9fb2754f9c)
"The next step involves returning to my Linode VM to retrieve my LE (Let's Encrypt) node reverse DNS. To locate this information, I navigate to the Network tab, scroll down to the IP addresses, and copy the reverse DNS, which in this case is 'Reverse DNS 172-234-29-112.ip.linodeusercontent.com'." 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/14f873ff-b8c1-417f-8d7c-b1780449cac1)
After this, I opened another tab and typed: `https://172-234-29-112.ip.linodeusercontent.com`. Since I was successful, I got a login page like this.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/575f26b5-1d5f-4a33-832a-cd8cfcef5f19)
Now, the username is "admin," and the password will be retrieved from my terminal.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/648a6877-e390-4e26-ba8b-03b1c43e60c9)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/5a076340-f5f0-4a48-8cb8-e91cf03e2d79)
Following the successful completion of this process, I now have access to add agents
How to Install Docker
Create  Linode > images Ubuntu 22.04 >Tab>Shared CPU> LE 2GB
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/448e6370-4b6a-4c08-96d2-ced1e18407dd)
Note; 2gb is confirmed to work on Docker
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/75489418-987c-47f6-87e1-f72b17342aed)
 
Created a container name for my Docker w/t Password and create the Docker. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/795fb8b3-5bfa-4a50-adb3-4b14ada32035)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/55433d7e-2daa-4133-8911-b8a7a05adfbd)
Copied my SSH Access key again and opened my terminal 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/7f2adc9e-d009-4b6d-b904-64a413763eff)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/9fa5f039-f320-4c46-82bc-5d68161503e4)
"I've successfully accessed the system, and my next step is to update the repositories using the command `sudo apt update`. It's recommended to perform repository updates, especially if you're not operating 
















