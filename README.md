# 🛡️ Wazuh Home Lab - SOC Analyst Practice Environment

This project sets up a complete **Wazuh-based security monitoring home lab** for aspiring SOC analysts to simulate, detect, and analyze various cyber threats in a virtual environment.

## 📚 Overview

Wazuh is an open-source SIEM solution for threat detection, integrity monitoring, and incident response. This lab allows you to monitor Linux and Windows hosts and simulate attacker activity from Kali Linux.

## 💡 What You'll Learn

- Threat detection for brute force, privilege escalation, and malware activity.
- Real-time alerting and log analysis using Wazuh.
- Onboarding and configuring Linux and Windows agents.
- Hands-on blue team experience using MITRE ATT&CK framework.

## 🖥️ Lab Components

| Component         | Description                         |
|------------------|-------------------------------------|
| Wazuh Server      | Core SIEM with Kibana Dashboard     |
| Ubuntu Server     | Simulated Linux target with agent   |
| Windows 10        | Simulated Windows target with agent |
| Kali Linux        | Attacker machine                    |

## 🧰 Requirements

- **System**: 16GB RAM, 4 CPU cores minimum
- **Software**: VirtualBox or VMware
- **VM Images**:
  - Wazuh OVA
  - Ubuntu Server 22.04
  - Windows 10 OVA
  - Kali Linux OVA

## 🛠️ Setup Instructions

1. Import Wazuh OVA into VirtualBox
2. Import and configure Ubuntu Server, Windows 10, and Kali
3. Onboard Linux and Windows agents to Wazuh
4. Test attacks from Kali Linux (brute force, PowerShell, file access)
5. Monitor alerts in Wazuh dashboard

> See [setup/](setup/) folder for detailed installation and configuration guides.

## ⚙️ Attack Scenarios & Detection

| Scenario                              | Detection by Wazuh           |
|--------------------------------------|------------------------------|
| Failed SSH Logins                    | Brute-force alert            |
| Unauthorized File Access             | FIM alert                    |
| Executable File Modification         | Integrity monitoring         |
| Privilege Escalation                 | Alert on sudo/suspicious cmd |
| Abnormal Process Execution           | Command monitoring           |
| Suspicious PowerShell Commands       | Windows Sysmon log alerts    |
| Outbound to Malicious IPs            | Network monitoring           |

> See [exercises/](exercises/) folder for step-by-step instructions.

## 📸 Screenshots

- ![Wazuh Dashboard](screenshots/wazuh_dashboard.png)
- ![SSH Brute Force Alert](screenshots/ssh_failed_logins_alert.png)

## 📖 Resources

- [Wazuh Documentation](https://documentation.wazuh.com)
- [MITRE ATT&CK](https://attack.mitre.org/)
- [ELK Stack Basics](https://www.elastic.co/what-is/elk-stack)

## ✅ Status

This lab is **fully operational** and tested on a local VirtualBox setup.

---

## 🙋‍♂️ Author

**Your Name**  
Cybersecurity Enthusiast | SOC Analyst Aspirant  
[LinkedIn Profile](https://linkedin.com/in/yourprofile)

---

## 📄 License

This project is open-source and available under the MIT License.
