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
"I've successfully accessed the system, and my next step is to update the repositories using the command `sudo apt update`. It's recommended to perform repository updates, especially if you're not operating with root privileges." 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/17ca1b15-59e4-4789-82dd-3b9a88c9272d)
Following that, I entered the command `sudo apt install docker.io docker-compose -y`. This installs both Docker and Docker Compose. 
After this I use the Wazuh Doc. To copy the Git clone.  https://documentation.wazuh.com/current/deployment-options/docker/wazuh-container.html to clone the the git repository in one command. 
git clone https://github.com/wazuh/wazuh-docker.git -b v4.7.0
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/eadb3111-f89b-4fb7-9f17-60287a99bea7)
Note: It might be necessary to manually input the Git code into the terminal; however, once executed, the process should conclude successfully. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/bd9bc90c-7f0e-4054-b7df-8a9c4038fe6b)
Next, to confirm the creation of the Docker, type "ls" in the terminal. You should see "Wazuh-docker" listed, indicating the successful creation of the Docker.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/cb5421fb-cbe6-458a-b67c-482d473e6f88)
Next, type "cd Wazuh-docker/" to navigate into the directory. Once inside, use the command "ls" to confirm your location. This step is crucial as you are preparing to deploy a single-node or computer setup. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/7ff7aec4-9a84-4b96-8a68-ca498aec6ac5)
To proceed, enter the command "cd single-node/" to navigate into the "single-node" directory. This step is essential as you prepare for the deployment of a single-node configuration. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/cda80905-e243-421d-b633-a1c8bbdfbea6)
Before proceeding with any further actions, I revisited the Wazuh documentation to ensure I generate the necessary self-assigned certificates. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/e0bb4f3d-40f8-47ee-96e0-02ca868e5735)
I copied the command `docker-compose -f generate-indexer-certs.yml run --rm generator` and pasted it into the same terminal where I was currently running commands.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/6af68644-7440-4fe3-9c81-c43f4697d569)
Next, type the command `docker-compose up -d` to launch it in the background. This will handle all necessary processes for me.  
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0afef12f-864f-45a6-ae4d-38ea41ee13ab)
Since I have successfully executed the command, the system is now deploying a multi-tier application and fetching all the required images. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/adfe1899-150d-4c15-996f-d2e065f539d5)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/11f6060b-81f6-4878-b8f0-5ac79dc7beb8)
To verify, I entered the command "docker stats" in the terminal. ![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/c30fba13-8ee7-4fef-a877-c73f8213a423)
This provides a real-time view of my containers, displaying key metrics and resource usage. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/e1850e7b-8e2a-4491-8891-81745ac1165c)
After confirming, I returned to the Linode environment to retrieve my Let's Encrypt (LE) reverse DNS. ![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/484966f0-e346-4e13-b46f-2387e4a76ebf)
Specify where in the Wazuh documentation the password can be found, providing a link or specific section for easier reference. 
User name: admin 
*Password: SecretPassword *
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/e251d218-d8b4-4cb1-843b-fde043d0fe79)
Now that This is completed, I will be adding agents. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/98bf83c0-9982-45dd-9bbb-072300280dea)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/f47c0c33-58fa-4914-aeac-3426db24f25d)
Next I’m going to Deploy a new agent. ![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/b13cf8d9-72dd-4ae2-b0e3-95f97331a499)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/86cae612-2935-44f4-82b9-d6a79643137d)
Next this process is straightforward but if new I have a awesome Video that helps with this entire process
Also I needed to be sure to assign a server address:
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/762f2d09-5c64-4f0c-ad6b-14df246594ec)
Note: The address you should use is the reverse DNS that you previously utilized. Simply copy and paste it into the FQDN, ensuring that the agent can access it. For example, "172-232-4-31.ip.linodeusercontent.com."
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/b252ea6b-39cb-4845-b116-a51c6d32dd2c)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/4751692c-1d15-4493-8466-acb5de258a26)
Proceed by assigning an agent name; for example, I've used "kali_linux". Feel free to choose any name that suits your preference. Subsequently, select a group, usually indicated as "(default)". At this stage, your layout should mirror the following:

After accomplishing this step, you'll receive the command to install the Wazuh agent. Simply copy and paste this command into your terminal:
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0b65897f-2ccd-4cb4-b7b7-2781c4088286)
copy and paste the BASH Command prompt:
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/278e29bc-cfbb-4de7-858c-7e1626ac30c3)
bash sudo systemctl daemon-reload sudo systemctl enable wazuh-agent
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/d299d196-6760-4b6d-b4bf-3e2dddbf4244)
Once this is completed, I now have my Kali Linux machine as one of the agents showing from my VM. Next, I will proceed with deploying a new agent for Windows.  
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/c4a2ee0b-1cc8-48fc-9160-e7a12ff7125d)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/c179b563-2eae-45af-9671-219820c20185)
Next copy the ip address 172-232-4-31.ip.linodeusercontent.com and assign to the server address
Open PowerShell from PC.  >copy the command to install Wazuh agent.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/5755f678-6324-4251-bcc9-7a2ab04cc7e3)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/4ac4731c-b419-4f86-9465-483d8665fe2d)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/c51baabe-ebcb-48b2-b932-f2ae333f835d)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/f456735d-2dcf-466f-8893-259270701854)
Important: run the command for the agent 1st then once it shows completed type  “NET START WazuhSvc”. This is just like Linux net start was a svc 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/1ef9102f-b2f8-479f-b1f7-b938225fbbb3)
Subsequently, I returned to my Wazuh dashboard.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/215cdcae-a6d2-47f6-aff1-3b3f1f72be1c)
I've expanded the number of agents from 2 to 4.

**Notes:**
- When deploying Ubuntu, stick to the same process, ensuring accurate copying and pasting. For optimal installation of DPKG and updates, consult the instructions provided in this [link](https://www.linuxtechi.com/install-virtualbox-guest-additions-on-ubuntu/).
**Note:**
- If deploying Kali Purple Linux, updated instructions will be necessary. Follow the provided directions and exercise caution not to use Ctrl+V for pasting, as it might trigger a right-click. For details, refer to [this guide](https://www.kali.org/docs/virtualization/install-virtualbox-guest-additions/).
  ![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/860baca0-9e18-4723-b86f-0d8824e1e2e4)
Having successfully deployed four agents, my next task is to perform a Secure Configuration Assessment (SCA). To initiate this process, I will click on the eye icon, directing me to the SCA dashboard.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0a040597-61c7-4028-be93-efbd5560a366)

The SCA dashboard offers a comprehensive overview of the entire system, encompassing categories such as MITRE, and compliance dropdown options including CIS, NIST, GDPR, HIPAA, and more. This facilitates a meticulous assessment of the system's security configuration.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/20e3030b-7398-4352-b744-fa1f29934f53)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/a6f21a5e-94a7-4ac8-9c47-dca430adeba3)
My SCA results indicate a 32% failure, with 262 items requiring further elaboration. This points to areas where security configuration improvements are needed to enhance overall system resilience and compliance
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/10788d24-b3e5-471c-81fc-f17305f5b792)
Accessing the SCA provides a detailed breakdown of passed and failed items, accompanied by actionable insights on how to address and remedy the identified issues
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/57e5d77e-04b4-480f-bd2c-500f02a12156)
For instance, delving deeper into the assessment reveals specific items such as the status of USB storage, providing insights into whether it's disabled or enabled.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0e19e7a3-a61b-41a0-8088-ceda0bddc237)
If that drill down to SSH b/c I can search for specific things like that. So not only is it showing me it tells me whats insecure and teaching me security. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/47e2bfd4-eab2-4620-ba46-954f3938434e)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/e3da759d-edf1-4526-a584-9971cad29696)
For instance, clicking on a specific result not only provides an explanation of how to check and fix the issue but also offers the rationale behind the recommendation. Additionally, it includes relevant MITRE techniques for a comprehensive understanding. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/efa686f7-e6a0-4ec3-a355-8740fec76bb0)
Exploring the Security Events section from the main dashboard allows me to investigate occurrences such as "Authentication failures," which may indicate potential "BRUTE FORCE ATTACKS." While there are currently no instances to confirm, this section also provides insights into the top five alerts for further analysis.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0efc2c96-4ca4-4afb-b8ae-9a5679e447c5)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/ac790e1c-be7c-46d2-849e-426fe021aff7)
Navigating to the "More" section from this screen opens up additional features, including insights into Vulnerabilities, Threat Detection & Response. This allows for a comprehensive view of potential vulnerabilities and a robust capability to respond to and manage detected threats effectively.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/fcb2348d-f51d-439f-af8e-3e6741eec093)
To commence file monitoring on Windows, the first step is to navigate back to the home icon. As a side note, you also have the option to unpin the current agent to reveal all available agents.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/2c4da08e-1d62-4079-8520-e98fc178bf62)
For users, especially those like me who are using it for the first time, the Integrity Monitoring tab will remain blank until you commence implementing and monitoring activities.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/24edabeb-6d0b-4469-98ee-5b5a653ef812)
Clicking on the Inventory tab initiates a scan that has already inventoried all default files within the directory and registry keys. Currently, the system is configured to scan every 12 hours. However, if it detects any changes, it will promptly notify me through an alert.

In the Files section, I can establish real-time notifications and define rule sets to efficiently manage and respond to events as they occur.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/87710b0a-ae36-4f57-8a56-db0e9e2429ba)
First, navigate to "This PC" > "Program Files (x86)" > "ossec-agent" to access the configuration file for the agent.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/5b1ea7a2-fa1d-4df2-953b-d4c57848e4f0)
Open with Note pad
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/285118bb-30d3-4926-af31-eafab368f237)
Next, utilize the Ctrl + F search tool to locate the "syscheck" section in the configuration file. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/3632618b-18c1-4231-90b4-d2d6f01e1bfb)
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/b659f6f1-71fe-41fa-ab4f-4027bd86d1be)
Select a location for the new rule. It is recommended to follow my path if you decide to implement this. Enter the following text in the space provided below:

```xml
<directories realtime="yes" report_changes="yes" check_all="yes">C:\Users\YourUserName\Desktop</directories>
```

Note: Replace "YourUserName" with your actual PC username. Remember to save after completing this task.
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/061d45b9-42bd-4140-9a26-0c14275f3889)
Next, open PowerShell as an administrator, and type the following command: `Restart-Service -Name Wazuh` and press Enter. This will be done quickly. 
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/db41c090-a82e-4478-8a52-65adbc72368d)
Next, open the Wazuh Dashboard and navigate to the Integrity Monitoring Events section
![image](https://github.com/Vtec87/SIEMHomeLab/assets/115051912/0811591c-88f3-4d51-b5a5-5d822794f2db)








