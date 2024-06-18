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

## Objectives

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

- Implementing account lockout policies
- Using complex passwords
- Enabling MFA
- Monitoring login attempts
- Deploying IDPS
- Educating users
- Updating systems
- Conducting security assessments
- Enforcing PoLP
- Establishing an incident response plan

This project demonstrates the importance of proactive measures and continuous monitoring to maintain a robust cybersecurity posture. The detailed steps and configurations provided can serve as a guide for similar implementations in other organizations.

