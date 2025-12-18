# Active Directory Deployment and Validation

## 1. Executive Summary

This project documents the end-to-end deployment and functional validation of a three-tier security lab environment. The primary goal was to establish reliable connectivity and data ingestion between an Active Directory target, a Kali Linux attack platform, and a Splunk Security Information and Event Management (SIEM) system.
Validation was achieved by performing a simulated Remote Desktop Protocol (RDP) brute-force attack and successfully confirming the presence of the resulting security telemetry in the Splunk index.

## 2. Project Objectives

The project successfully met the following technical objectives:

### Deployment and Connectivity Objectives
* **Active Directory Deployment:** Successfully set up a Windows machine as the Active Directory Target, configured for Remote Desktop access.
* **Cross-Platform Integration:** Established reliable network connectivity between the Windows Target, the Kali Linux Attacker, and the Splunk Indexer.

### 🔑 Validation and Security Objectives
* **Attack Validation:** Executed a successful RDP brute-force attack using **Hydra** to confirm the target's reachability and service response.
* **Detection Validation:** Configured the **Splunk Universal Forwarder** on the target and verified the ingestion of security logs (`EventCode=4625`) into the SIEM.

### 🛠️ Troubleshooting and Configuration Objectives
* **System Integrity:** Resolved critical Active Directory and DNS misconfigurations that interfered with user authorization.
* **SIEM Health:** Tuned the Splunk data pipeline to resolve ingestion latency issues, ensuring real-time security visibility.
