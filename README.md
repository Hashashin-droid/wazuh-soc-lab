# wazuh-soc-lab

Welcome to my Wazuh SOC Lab repository

This project documents my journey of building a Security Operations Center (SOC) lab using Wazuh, Suricata, pfSense, Sysmon, and VirusTotal. The purpose of this lab is to simulate real-world cyber attacks, monitor security events, investigate alerts, and develop practical SOC Analyst skills.

### 📌 Overview

This project demonstrates the deployment, configuration, and integration of multiple security tools using the open-source Wazuh SIEM/XDR platform.

The lab is designed to provide hands-on experience in:

- Security monitoring
- Alert triage
- Incident investigation
- Threat detection
- Log analysis
- Threat intelligence enrichment

### 🏗️ Lab Architecture

The lab is built using VirtualBox virtual machines and includes the following components:

- **Wazuh OVA**: Centralized SIEM platform consisting of Wazuh Manager, Indexer, and Dashboard.
- **Windows 10 Host**: Monitored endpoint running Wazuh Agent and Sysmon.
- **Ubuntu Host**: Linux endpoint monitored by Wazuh.
- **Kali Linux Attacker**: Used to simulate attacks and adversary behavior.
- **pfSense Firewall**: Network firewall and traffic monitoring platform.
- **Suricata IDS**: Network intrusion detection system integrated with Wazuh.
- **VirusTotal Integration**: Threat intelligence enrichment for file reputation analysis.

### 🛠️ Setup & Configuration

#### Wazuh Configuration

//wazuh-configuration.pdf

**Summary**:

- Deploy Wazuh using the official OVA package.
- Configure Wazuh services and dashboard.
- Register Windows and Linux agents.
- Verify agent connectivity and log collection.

#### Sysmon Configuration

//sysmon-configuration.pdf

**Summary**:

- Install Sysmon on Windows 10
- Configure event collection using a Sysmon configuration file
- Forward Sysmon events to Wazuh
- Improve endpoint visibility and detection capability

#### Suricata Integration

//suricata-integration-guide.pdf

**Summary**:

- Deploy Suricata IDS
- Configure detection rules
- Forward EVE JSON logs to Wazuh
- Monitor network-based attacks and suspicious traffic

#### pfSense Integration

//pfSense-integration-guide.pdf

**Summary**:

- Configure pfSense firewall
- enable remote logging
- Forward firewall events to Wazuh
- Monitor allowed and blocked network activity

#### VirusTotal Integration

//virusTotal-integration-guide.pdf

- Configure VirusTotal API integration.
- Enrich Wazuh alerts with reputation data.
- Improve malware triage and investigation workflows.


