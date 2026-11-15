<div align="center">

# 🔐 Cybersecurity Week 2: Penetration Testing, Footprinting and Network Scanning

**Passive Reconnaissance, Active Host Discovery, and Penetration Testing Documentation**

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" /> <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" /><img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" /><img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Waqas%20Karim%20CCIE-C00000?style=flat-square" />
</p>

---


# Disclaimer
All activities were performed using publicly available information and an authorized VirtualBox lab environment for educational purposes.

Personally identifiable information visible in the screenshots have been redacted.

No unauthorized access was performed.

# 📌 Project Overview

This lab focuses on practicing reconnaissance and network scanning using theHarvester in Kali Linux and Zenmap on Windows 11. The goal is to gather publicly available information about a target domain and discover live devices on a local network in a safe and controlled way.

These activities provide hands-on experience with the early stages of cybersecurity testing. Using theHarvester, public details like subdomains, hosts, and email addresses are collected from open sources without directly touching the target system. With Zenmap, ping scans are used to identify active hosts, record their IP and MAC addresses, and map out the local network topology.

All results and screenshots from both modules are documented in a formal Penetration Testing Report (W2-PM-FINAL). Organizing the findings into a clear report helps connect technical scan results with basic risk analysis and practical security improvements for future exercises.


## ✅Completed Modules

- 🌐 **W2-PM4:** theHarvester Footprinting Attacks 
- 📶 **W2-PM5:** Zenmap Network Scanning (Ping, ARP and Nmap Host Discovery 

[Click here to view my Week 2 Penetration Testing Report (PDF)](NETWORKWALKS-DAMILARE-ODESANMI-B084-WK2-PM4-PM5-PENETRATION-TESTING.pdf)
https://drive.google.com/file/d/1JgpG8c7wLhQ7RTnwOu_QVoHqTx49fhkx/view?usp=drivesdk

# 🎯 Objectives

The main objectives of this project are to:

- Install and configure Zenmap on Windows and prepare theHarvester in Kali Linux for reconnaissance and scanning tasks.
- Gather publicly available email addresses, subdomains, and host details for a target domain using theHarvester across Baidu and all supported public sources.
- Identify the local IP address and LAN subnet configuration on the host Windows machine.
- Perform ping scan in Zenmap to discover live hosts and record their IP and MAC addresses on the local network.
- Generate and export a visual network topology map in PDF format with the legend enabled.
- Document all commands and screenshots, and security recommendations into a formal Penetration Testing Report (W2-PM-FINAL).
- Build practical hands-on experience in passive footprinting and active network discovery for future cybersecurity and penetration testing exercises

---

# 🛡️ Purpose of the Lab

The lab provides a safe and controlled environment where reconnaissance and network scanning techniques can be practiced without affecting live production systems. It allows hands-on learning and experimentation while keeping testing limited to public information and owned local devices.

Possible uses of the lab include:
- Gathering publicly available information about target domains
- Identifying active hosts and devices on a local network
- Recording IP and MAC addresses across a subnet
- Mapping out visual network topologies
- Comparing results from different open-source intelligence tools
- Documenting scan findings into structured penetration testing reports
- Practicing early-stage cybersecurity and ethical hacking techniques
---

# 🏗️ Lab Architecture

- **Kali Linux Virtual Machine:** Used with `theHarvester` for passive reconnaissance (`W2-PM4`)
- **Windows Host Machine:** Used with Command Prompt (`ipconfig`) and Zenmap (Nmap GUI) for active local network scanning (`W2-PM5`)

---

# 🪜 Lab Setup Procedure

 ### Module 🌐- W2-PM4: theHarvester Footprinting Attacks 

### Steps In Order:

#### Task 1: Targeted Search Using Baidu

1. Open **`theHarvester`**: Launch **`theHarvester`** in Kali Linux from the applications menu located in the top left side of the screen.
2. Review Usage Instructions: Check the tool's commonly used commands and supported data sources to verify the syntax before running the scan.

  ![Image 1](<Usage Guidlines.png>)
*Figure 1: Review*


3. Run the Baidu Search: Execute the following command in the terminal to search for email IDs and subdomains related to **`microsoft.com`** (which is the target domain) using Baidu with a result limit of 1000:

> theHarvester -d microsoft.com -l 1000 -b baidu

4. Review and Save Output: Take the screenshot of the given output and save the results into a text file.

Below is the screenshot for the Baidu Search:

![Image 2](<Task 1 Search with Baidu.png>)
*Figure 2: Baidu Search*
