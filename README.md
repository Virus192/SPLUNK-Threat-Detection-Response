# SPLUNK PROJECT
 # Harnessing Splunk for Threat Detection and Mitigation

**Enhancing Cybersecurity Resilience: A Comprehensive Project Report**

**Presented by: Abdulazeez Mohammed**

## Introduction

In today's dynamic cyber landscape, organizations face an ever-evolving array of threats that can compromise the integrity, confidentiality, and availability of their critical assets. To address these challenges and bolster our organization's cybersecurity posture, I spearheaded a multifaceted project aimed at deploying advanced security measures and implementing industry best practices. This comprehensive endeavor encompassed:

- Installation and configuration of a live Splunk server on Ubuntu server OS
- Deployment of Splunk Universal Forwarder and Sysmon to collect and forward logs from Windows 10 machines and an Active Directory Domain Controller on Windows Server 2022
- Simulation of a brute force attack using a Kali machine
- Observation of logs on the Splunk server
- Implementation of configuration management settings to mitigate PowerShell-based attacks
- Enforcement of NIST SP 800-53 controls to restrict PowerShell usage on endpoint devices

## Tools Required

- **Windows Server 2022:** 4 GB RAM, 2 cores, 80 GB storage
- **Windows 10 Pro:** 4 GB RAM, 1 core, 50 GB storage
- **Ubuntu Desktop live-Server 22.04.4:** 6 GB RAM, 2 cores, 90 GB storage
- **Kali Linux:** 6 GB RAM, 2 cores, 90 GB storage
- **Splunk Universal Forwarder 9.2.1**
- **Splunk 9.2.1 for Linux**
- **Sysmon64.exe**

## Logical Diagram

The project comprised several key phases to address specific aspects of the organization's Security Operation needs.
<p align="center">
 <br/>
<img src="https://imgur.com/mTzjDOJ.jpg" height="80%" width="80%" />
<br />

</p>

## Objectives
- ♻ The objective of this project is to enhance an organization's overall security posture by implementing a comprehensive set of measures aimed at improving threat detection, response capabilities, and regulatory compliance. 

Specifically, the project aims to achieve the following objectives:

- **🔰 Enhanced Log Management and Analysis:** Deployed a Splunk server on Ubuntu and configured Splunk Universal Forwarder and Sysmon on Windows systems to collect and forward logs. This enhances visibility into network activity and enables proactive threat detection and response.

- **🔰Threat Simulation and Detection:** Utilized a Kali machine to conduct a simulated brute force attack on Windows systems. Monitor and analyze the attack logs in Splunk to identify potential security threats and vulnerabilities.

- **🔰Configuration Management and Mitigation:** Implemented configuration management settings based on observed attack patterns to block PowerShell scripting, mitigating the risk of further exploitation and unauthorized access.

- **🔰 Compliance with NIST SP 800-53:** Implemented select controls from NIST SP 800-53 to restrict PowerShell usage on endpoint devices, aligning with best practices and regulatory requirements. This ensures adherence to industry standards and strengthens the organization's cybersecurity resilience.

- ⭕ Overall, the objective of this project is to proactively enhance an organization's cybersecurity defenses, minimize the likelihood of successful cyberattacks, and mitigate the impact of potential security incidents. By leveraging advanced security tools and frameworks, and to further safeguard organizational assets, data integrity, and user privacy against evolving cyber threats. 
### Infrastructure Setup
- Deploy Active Directory Domain Controller (AD DC) on Windows Server 2022
- Create user accounts and groups in Active Directory
- Install and configure a live Splunk server on Ubuntu server OS

### Log Collection and Analysis
- Deploy Splunk Universal Forwarder on Windows 10 machines and AD DC
- Configure Sysmon to monitor system activity and generate logs
- Forward logs from Windows machines to Splunk server for analysis

### Threat Simulation and Detection
- Install Ubuntu server and configure Splunk to receive and analyze logs
- Use Kali machine to simulate brute force attack on Windows 10 target PC
- Observe logs on Splunk server to detect and analyze attack patterns

### Configuration Management and Enforcement
- Implement settings to block PowerShell scripting on endpoint devices
- Enforce NIST SP 800-53 controls to restrict PowerShell usage

## Project Overview

### Infrastructure Setup
1. **Active Directory Configuration**
   - Set up AD DC on Windows Server 2022
   - Create OUs and add user accounts

2. **Splunk Server Installation**
   - Install and configure Splunk server on Ubuntu

### Log Collection and Analysis
1. **Splunk Forwarder and Sysmon**
   - Install and configure on AD DC and Windows 10

2. **Log Aggregation**
   - Forward logs to Splunk server

### Threat Simulation and Detection
1. **Kali Linux Attack Simulation**
   - Perform brute force attack on Windows 10

2. **Log Observation**
   - Analyze Splunk logs to detect attack patterns

### Configuration Management and Enforcement
1. **PowerShell Restrictions**
   - Implement policies to mitigate risks

2. **NIST SP 800-53 Controls**
   - Enforce security measures on endpoint devices

## Conclusion

Upon completion, several security recommendations were made based on the simulated brute force attack, including:

- **🔰 Implement Account Lockout Policies:**
Enforce account lockout policies to temporarily lock user accounts after a certain number of failed login attempts. This helps mitigate the risk of brute force attacks by limiting the number of password guesses an attacker can make.
- **🔰 Use Complex and Unique Passwords:**
Encourage users to create complex passwords that are difficult to guess and ensure they are not reused across multiple accounts. Consider implementing password complexity requirements and regular password expiration policies to enhance security.
- **🔰 Enable Multi-Factor Authentication (MFA):**
Implement multi-factor authentication (MFA) for user accounts, requiring users to provide additional verification factors (e.g., SMS codes, authenticator apps, biometrics) in addition to passwords. MFA adds an extra layer of security and helps prevent unauthorized access even if passwords are compromised.
- **🔰 Monitor and Analyze Login Attempts:**
Implement logging and monitoring mechanisms to track login attempts, including successful and failed logins. Use security information and event management (SIEM) solutions or log analysis tools to detect anomalous login patterns indicative of brute force attacks.
- **🔰 Deploy Intrusion Detection and Prevention Systems (IDPS):**
Deploy IDPS solutions to detect and block brute force attacks in real-time. Configure IDPS rules to analyze network traffic and identify patterns consistent with brute force attack techniques, such as repeated login attempts from the same IP address.
- **🔰 Educate Users on Security Awareness:**
Provide regular security awareness training to users to educate them about the risks of weak passwords, phishing attacks, and other common security threats. Empower users to recognize suspicious login attempts and report them to the IT security team.
- **🔰 Regularly Update and Patch Systems:**
Keep all systems, including the Windows 10 target PC and network infrastructure, up to date with the latest security patches and updates. Vulnerabilities in operating systems and software can be exploited by attackers to gain unauthorized access.
- **🔰 Conduct Regular Security Assessments:**
Perform regular security assessments, including vulnerability scans and penetration tests, to identify and remediate security weaknesses in the organization's infrastructure. Address any vulnerabilities discovered during these assessments promptly to reduce the risk of exploitation.
- **🔰 Enforce Principle of Least Privilege (PoLP):**
Follow the principle of least privilege (PoLP) by granting users only the permissions necessary to perform their job responsibilities. Restrict administrative privileges to essential personnel and minimize the attack surface available to potential attackers.
- **🔰 Establish an Incident Response Plan:**
Develop and maintain an incident response plan outlining procedures for responding to security incidents, including brute force attacks. Establish roles and responsibilities, define escalation procedures, and conduct regular incident response drills to ensure readiness in the event of a security breach.

⭕By implementing these security recommendations, organizations can enhance their resilience against brute force attacks and other common cyber threats, safeguarding their systems and data from unauthorized access and exploitation.


This project demonstrates the importance of proactive measures and continuous monitoring to maintain a robust cybersecurity posture. The detailed steps and configurations provided can serve as a guide for similar implementations in other organizations.

