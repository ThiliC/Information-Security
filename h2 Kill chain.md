## h2 Kill Chain
___

### X) Summary of "Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains"

- **Cyber Defense Focus**: The paper is all about using intelligence to make computer network defenses stronger by understanding how hackers think and operate.

- **Attacker Campaigns**: It talks about how hackers often plan their attacks like campaigns. If we understand these plans, we can better prepare for potential attacks.

- **Intrusion Kill Chain**: The authors introduce a model called the Intrusion Kill Chain. This breaks down the typical steps a hacker takes during an attack, like planning, launching the attack, and achieving their goals. If we can interrupt them at any point, we can stop the attack.

- **Importance of Intelligence Analysis**: They emphasize that looking at past attacks helps organizations make smarter decisions and better defenses for the future.

- **Using Threat Intelligence**: Organizations are encouraged to use threat intelligence—basically, information about potential threats—so they can stay ahead of hackers by learning from past events.

- **Advice for Organizations**: The paper suggests being proactive: using threat intelligence, continuously monitoring their systems, and having a response plan in place based on the kill chain model.

- **Collaboration and Sharing**: The authors stress that sharing information about threats between organizations can make everyone safer and improve overall cybersecurity.

#### Reference: Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains
---

### a) Detailed Technical Report: Installing Debian 12 " Bookworm" on VirtualBox (Windows Host).

This report outlines the process of installing Debian 12 "Bookworm" on a Virtual Machine. 

- **Host**: Windows  
- **Virtual Version**: Version 7.0.20 r163906 (Qt5.15.2)  
- **Debian ISO**: debian-live-12.6.0-amd64-xfce.iso  

### Download Source
- **Debian ISO**: I downloaded Debian 12 ISO from `debian-live-12.6.0-amd64-xfce.iso`.

### Steps to Install Debian
1. **Open VirtualBox**: I opened VirtualBox on my computer.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2001%20-%20Create%20VM.png)
2. **Create Virtual Machine**: 
   - Clicked on **New** to create a new virtual machine.
   - **Name**: Entered a suitable name for the virtual machine (e.g., `DebianTeroKarvinenCom`).
   - **ISO Image**: Selected the downloaded ISO file (`debian-live-12.6.0-amd64-xfce.iso`).
   - **Type**: Set as **Linux**.
   - **Version**: Set as **Debian (64-bit)**.
3. **Skip Unattended Installation**:
   - Unchecked the option for **Unattended Installation** to proceed with a manual setup.

### Hardware Settings
- **Memory Allocation**:
  - **Base Memory**: Set to **4096 MB** to ensure smooth operation.
- **Processor Configuration**:
  - **CPU**: Allocated **2 CPUs** to the virtual machine.
- **Hard Disk Setup**:
  - Selected **Create a virtual hard disk now**.
  - **File Location**: Chose a suitable directory on my host machine.
  - **Size**: Allocated **60 GB** for the virtual disk.
  - Clicked **Create** to finalize the hard disk setup.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2002%20-%20Created%20VM%20Details.png)

### Start the Virtual Machine and Install Debian
1. **Booting**:
   - I started the virtual machine by double-clicking on it in the VirtualBox Manager.
   - The VM booted from the Debian ISO, displaying the boot menu.
   - Selected **Live System** to boot into a live session of Debian.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2003%20-%20Debian%20VM.png)
2. **Testing Basic Functionality**:
   - After logging in, I opened a web browser and searched for a random topic to ensure that the keyboard, mouse, and network were functioning correctly.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2005%20-%20Checking%20Web%20browser.png)
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2004%20-%20Checking%20Application%20.png)

3. **Launching the Installer**:
   - After confirming the live environment worked correctly, I clicked the **Install Debian** icon on the desktop to begin the installation.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2006%20-%20Installing%20Debian.png)

4. **Language and Local Settings**:
   - **Language**: Selected **American English**.
   - **Time Zone**: Chose **Europe, Helsinki** as the time zone.
   - **Keyboard**: Selected **Finnish Keyboard**.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2007%20-%20Language%20and%20Locale%20Settings.png)

5. **Partitioning the Disk**:
   - Chose the option to **Erase Disk** and proceeded with default partitioning.
   - Confirmed the setup and started the installation.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2008%20-%20Partitioning%20the%20Disk.png)

### User Setup During Debian Installation
- **User Information**:
  - Entered my full name.
  - Chose a login name.
  - Assigned a computer name.
  - Created a password.
After checking the summary, I clicked **Install** to begin the installation process. This took approximately **10 minutes**.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2009%20-%20Users%20and%20setting%20Passwords.png)

### Completion
Once the installation is completed, I clicked **Done** and chose to **Restart Now**.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2010%20-%20system%20installs.png)

### Post-Installation Setup
1. **First Boot**:
   - The installation completed successfully, and I rebooted the virtual machine.
   - I was greeted with the login screen, where I entered the credentials created during installation.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2011%20-%20First%20Login.png)

2. **Testing Basic Functionality**:
   - After logging in, I opened a web browser and searched for a random topic to ensure that the keyboard, mouse, and network were functioning correctly.

### Voluntary Bonus: Update All Software on Your Linux Box Using `apt-get`
- **Update All Software**:
  - Opened the terminal: **Applications: Terminal Emulator**.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2012%20-%20Terminal%20Emulator..png)

  - Ran the following commands to update the system:
    ```
    sudo apt-get update
    sudo apt-get -y dist-upgrade
    ```
  - This updated all packages to their latest versions. This took a while. Should not interrupt the upgrade while it is working and should not close the window before it is done. 
  - I rebooted after the upgrade as the kernel `linux-image` was upgraded.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2013%20-%20Update%20All%20Software.png)
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2014%20-%20Update%20All%20Software%20ii.png)

- **Firewall Setup**:
  ```
  sudo apt-get -y install ufw
  sudo ufw enable
  ```
  ### Voluntary Bonus: Install a Local Web Server on Linux Using `apache2`
  **Reference**: https://terokarvinen.com/2008/install-apache-web-server-on-ubuntu-4/  

- **Install Apache**:
  - Opened the terminal: **Applications: Terminal**
  - Executed the following command:
    ```
    sudo apt-get install apache2
    ```
- **Test the Installation**:
  - Surfed to my local server using the following command:
    ```
    firefox "http://localhost"
    ```
  - This directed me to my web browser.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2015%20-%20Download%20a%20web%20page%20using%20netcat%20'nc'.png)
---

### Voluntary Bonus: Download a Web Page from Your Local Web Server Manually Using `netcat`
**Reference**: https://www.geeksforgeeks.org/how-to-make-an-http-get-request-manually-with-netcat/?ref=oin_asr9nc/  
- **Install Netcat**:
  - Opened the terminal: **Applications: Terminal**
  - Executed the following command:
    ```
    sudo apt-get install netcat
    ```
**Download a Web Page**:
  - To download the Wikipedia Main Page, I ran:
    ```
    cat wikipedia.org
    ```

  - After entering the following manually:
  
    ```
    GET /wiki/Main_Page HTTP/1.1
    Host: Wikipedia.org:8080
    Connection: close
    ```
  - The webpage downloaded successfully.
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2015%20-%20Download%20a%20web%20page%20using%20netcat%20'nc'.png)
---

### Voluntary Bonus: Find a Log Line Created by Your Manual Web Page Download
**Reference**: https://www.loggly.com/use-cases/how-to-monitor-your-apache-logs/  
**Reference** OpenAI. (2024). ChatGPT (GPT-4).  

- **Access Apache Logs**:
  - Initially, I tried to view the log file with:
    ```
    /var/log/apache2/access.log
    ```
  - Access was denied, so I used the following command to view the last 10 lines:
    ```
    sudo tail -n 10 /var/log/apache2/access.log
    ```
![image](https://github.com/ThiliC/Information-Security/blob/main/Installing%20Debian/Fig.%2016%20-%20log%20in.png)
---
### Voluntary Bonus: ATT&CK. Compare MITRE ATT&CK Framework to Cyber Kill Chain

**Cyber Kill Chain**:
The Cyber Kill Chain framework is designed for understanding and preventing cyber attacks. It breaks down the attack process into seven phases:

- **Reconnaissance**
- **Weaponisation**
- **Delivery**
- **Exploitation**
- **Installation**
- **Command and Control**
- **Action on Objectives**

By understanding these phases, security professionals can develop effective mitigation strategies to protect against attacks.

---

**MITRE ATT&CK**:
MITRE ATT&CK is a framework developed by the non-profit organization MITRE in 2013. It considers each stage of the cyberattack lifecycle from the perspective of the attacker. It is a globally accessible knowledge base of adversary Tactics, Techniques, and Procedures (TTP) based on real-world observations. The ATT&CK knowledge base is used as a foundation for the development of specific threat models and methodologies in the private sector, government, and the cybersecurity product and service community.

---

### Comparison:

**Level of Detail**:
- **MITRE ATT&CK** provides a more granular approach, with a detailed catalog of techniques and tactics. This allows for precise threat modeling and defense strategies.
- **Cyber Kill Chain** outlines broader phases of an attack, making it easier to conceptualize the overall attack lifecycle.

**Application**:
- The **ATT&CK framework** is widely used for threat hunting, incident response, and defensive measures based on observed techniques.
- The **Kill Chain** is often used for developing security postures and proactive measures to prevent attacks by disrupting them at various stages.

**Adaptability**:
- The **ATT&CK framework** is continuously updated with new tactics and techniques based on current threat landscapes.
- The **Kill Chain** is more static and may not account for the evolving nature of cyber threats.

---

**Reference**: https://www.obriain.com/training/otsec2/odt/Topic_2-Cyber_Kill_Chain-MITRE_ATT&CK_for_ICS_odt.pdf


    

