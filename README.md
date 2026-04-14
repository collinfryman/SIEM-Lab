# 🛡️ Wazuh SIEM Home Lab

A hands-on cybersecurity home lab built to develop practical SIEM skills relevant to Security Operations Center (SOC) environments. This project involved deploying and configuring a production-grade SIEM platform from scratch, ingesting real system and network log data, simulating security events, and building a custom monitoring dashboard.

---

## 📌 Project Overview

This lab was built to bridge the gap between theoretical cybersecurity knowledge and real-world SOC analyst skills. By standing up a live SIEM environment — rather than using a pre-configured demo — I gained hands-on experience with the full lifecycle of security monitoring: deployment, configuration, log ingestion, alert tuning, and incident visibility.

---

## 🧰 Technologies Used

| Category | Tool / Technology |
|---|---|
| Virtualization | VirtualBox |
| Operating System | Kali Linux |
| SIEM Platform | Wazuh (open-source) |
| Log Sources | System/OS logs, network traffic logs, security event logs |

---

## 🔧 What I Built

### 1. Virtual Environment Setup
- Provisioned a **Kali Linux** virtual machine using **VirtualBox**
- Configured networking to allow log collection and SIEM dashboard access

### 2. Wazuh SIEM Deployment
- Downloaded, installed, and configured **Wazuh** (manager, indexer, and dashboard components) on the Kali Linux VM
- Verified that all services were running and communicating correctly
- Configured agents to forward log data to the Wazuh manager

### 3. Log Monitoring & Ingestion
Configured Wazuh to collect and analyze the following log sources:
- **System/OS logs** — authentication logs, syslog, kernel messages
- **Network traffic logs** — monitored connection events and traffic patterns
- **Security event logs** — tracked access attempts, privilege escalation indicators, and policy violations

### 4. Attack Simulation & Alert Generation
- Simulated a **brute force / failed login attack** to generate real security alerts
- Observed how Wazuh detected, categorized, and escalated the repeated authentication failures
- Reviewed raw alert data and understood how rule IDs map to MITRE ATT&CK techniques

### 5. Dashboard Customization
- Worked within the **Wazuh Dashboard** (built on OpenSearch/Kibana)
- Customized existing panels to surface the most relevant security metrics
- Built a monitoring view focused on authentication events, alert severity distribution, and active agents

---

## 📊 Key Skills Demonstrated

- **SIEM Deployment** — Stood up a full Wazuh stack from scratch in a virtualized environment
- **Log Management** — Configured multi-source log ingestion (OS, network, security events)
- **Alert Analysis** — Interpreted SIEM alerts, understood rule logic, and correlated events
- **Threat Detection** — Observed real alert behavior from a simulated brute force attack
- **Dashboard Development** — Customized monitoring panels for SOC-style visibility
- **Linux Administration** — Managed services, configured files, and troubleshot in a Kali Linux environment

---

## 🎯 SOC Relevance

This project directly maps to Tier 1 SOC Analyst responsibilities:

| SOC Task | Lab Equivalent |
|---|---|
| Monitor SIEM for alerts | Wazuh dashboard monitoring, live alert feeds |
| Investigate authentication anomalies | Brute force simulation, alert triage |
| Review and filter log data | Multi-source log ingestion and analysis |
| Maintain dashboard visibility | Custom Wazuh dashboard panels |
| Work in Linux environments | Kali Linux administration throughout |

🔗 [GitHub Profile](https://github.com/collinfryman)
