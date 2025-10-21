
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

<img width="1777" height="798" alt="image" src="https://github.com/user-attachments/assets/c1f7e51c-9a13-4c6d-8a63-ceb027c0b756" />


3. Suricata EVE Output page (Screenshot showing remote syslog to `WAZUH_IP:5514`).

<img width="1887" height="870" alt="image" src="https://github.com/user-attachments/assets/dbd72715-7b0e-445c-93d6-48dcd29374be" />
<img width="1862" height="835" alt="image" src="https://github.com/user-attachments/assets/a504407e-e7a5-4eea-8022-a9aca93a41bf" />

4. Wazuh Manager `systemctl status wazuh-manager` (Screenshot).
/home/ubuntu-grc/Pictures/Screenshots/Screenshot from 2025-10-21 21-30-13.png
   
6. Windows Event Viewer / Sysmon (Screenshot).


