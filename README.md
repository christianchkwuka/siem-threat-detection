# SIEM-based Threat Detection Lab (Wazuh / Splunk)

**Objective (EN):** Demonstrate design, detection, and incident response for SSH brute force and port-scan scenarios using Wazuh (or Splunk), pfSense, Suricata, Windows event logs, and Kali Linux.

**Ziel (DE):** Nachweis von Design, Detektion und Incident Response für SSH-Bruteforce- und Portscan-Szenarien mit Wazuh (oder Splunk), pfSense, Suricata, Windows-Eventlogs und Kali Linux.

## Components / Komponenten
- Wazuh Manager (Ubuntu) – UDP 5514 syslog input, JSON rules
- pfSense + Suricata (EVE JSON to Wazuh)
- Windows (Sysmon + Winlogbeat or Wazuh Agent)
- Kali Linux (nmap, hydra)

## Outcomes / Ergebnisse
- Alerts: *SSH Brute Force Detected*, *Possible Port Scan*
- Correlation & Triage notes
- Containment: IP block on pfSense
- Post-incident Root Cause Analysis (RCA)
