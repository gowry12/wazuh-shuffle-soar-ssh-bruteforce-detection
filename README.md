# SSH Brute-Force Detection and Automated Response using Wazuh and Shuffle SOAR

## Project Overview

This project demonstrates a Security Orchestration, Automation and Response (SOAR) workflow that detects SSH brute-force attacks using Wazuh SIEM and automates alert enrichment using Shuffle SOAR.

The workflow extracts attacker information from Wazuh alerts, enriches the data with VirusTotal threat intelligence, and notifies security analysts through automated email alerts.

---

## Objectives

* Detect SSH brute-force attacks
* Forward alerts from Wazuh to Shuffle SOAR
* Enrich alerts using VirusTotal
* Reduce analyst workload through automation
* Demonstrate real-world SOC operations workflows

---

## Technologies Used

| Tool              | Purpose              |
| ----------------- | -------------------- |
| Wazuh             | SIEM/XDR Platform    |
| Shuffle SOAR      | Security Automation  |
| Kali Linux        | Attack Simulation    |
| VirusTotal        | Threat Intelligence  |
| Email Integration | Analyst Notification |

---

## Architecture

Kali Linux → Wazuh → Shuffle SOAR → VirusTotal → Email Notification

---

## Workflow

1. SSH brute-force attack simulated using Hydra.
2. Wazuh detects multiple failed login attempts.
3. Alert forwarded to Shuffle using Webhook.
4. Shuffle extracts attacker IP.
5. VirusTotal checks IP reputation.
6. If malicious, email notification is generated.
7. Analyst reviews and escalates if required.

---

## Key Features

* Automated Alert Processing
* Threat Intelligence Enrichment
* Conditional Logic Workflow
* Analyst Notification
* Reduced False Positives

---

## Testing Results

### Scenario 1

Normal IP Address

Result:
No malicious reputation detected.
Workflow terminated successfully.

### Scenario 2

Malicious Test IP

Result:
Threat detected.
Email notification successfully triggered.

---

## SOC Skills Demonstrated

* SIEM Monitoring
* Log Analysis
* Incident Response
* Threat Intelligence
* Alert Triage
* Security Automation
* SOAR Playbook Development
* Wazuh Administration

---

## Future Enhancements

* Automated IP Blocking
* Jira Integration
* ServiceNow Ticket Creation
* Multi-Source Correlation
* Threat Hunting Workflows

---

## Author

Gowry N

Cybersecurity Enthusiast | SOC Analyst Aspirant

GitHub: https://github.com/gowry12

Medium: https://medium.com/@ngowry12
