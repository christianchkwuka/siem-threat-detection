
# 00 — Lab Topology / Lab-Topologie

## EN — Topology overview
- Wazuh Manager (Ubuntu VM) — receives EVE JSON / syslog on UDP 5514 and secure on 1514.
- pfSense (appliance) with Suricata — generates EVE JSON alerts and forwards to Wazuh (UDP 5514).
- Windows host — logs forwarded via Wazuh Agent or Winlogbeat.
- Kali Linux — attacker launching `nmap` & `hydra`.

## DE — Topologie Überblick
- Wazuh Manager (Ubuntu VM) — empfängt EVE JSON / Syslog auf UDP 5514 und secure 1514.
- pfSense (Appliance) mit Suricata — erzeugt EVE JSON-Alarme und sendet an Wazuh (UDP 5514).
- Windows-Host — Logs via Wazuh-Agent oder Winlogbeat.
- Kali Linux — Angreifer (nmap & hydra).

## Diagram & Screenshots (where to capture)
1. Topology diagram (Draw.io/diagrams.net): show connections -> save `docs/img/topology.png`.
2. pfSense interfaces page (Screenshot).
3. Suricata EVE Output page (Screenshot showing remote syslog to `WAZUH_IP:5514`).
4. Wazuh Manager `systemctl status wazuh-manager` (Screenshot).
5. Windows Event Viewer / Sysmon (Screenshot).



<img width="1777" height="798" alt="image" src="https://github.com/user-attachments/assets/c1f7e51c-9a13-4c6d-8a63-ceb027c0b756" />

