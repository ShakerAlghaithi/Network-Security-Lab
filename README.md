🧱 Network Security Controls Lab Portfolio
---------------------------------
Hands-on Deployment and Administration of NAC, NDR, IPS, and Firewalls

👤 About Me
---------------------------------
Name: Shaker Alghaithi

Career Goal: Junior Network Security Engineer

LinkedIn: linkedin.com/in/shaker-alghaithi-1133ab92

Certifications: Cisco CCNA, Cisco DevNet Associate

Currently Studying: Cisco CCNP

🧭 Overview
-----------------------------------
This repository documents my 12-week journey to design, deploy, and administer core network security controls in a virtual lab environment.

Technologies covered:

  - Network Access Control (NAC) – PacketFence / Cisco ISE
  - Network Detection & Response (NDR) – Zeek / Security Onion
  - Intrusion Prevention System (IPS) – Suricata / Snort
  - Firewall / NGFW – pfSense / OPNsense / Palo Alto VM

Goal:
Gain practical, end-to-end experience building a secure enterprise network, integrating controls for visibility, prevention, and response.

🧩 Lab Architecture
--------------------------------------------
Components:
  - Virtualization: VirtualBox / VMware
  - OS: Ubuntu Server, Windows Server, Windows 10 Client, Kali Linux
  - Network Controls:
      1.NAC: PacketFence + FreeRADIUS
      2.NDR: Zeek / Security Onion
      3.IPS: Suricata (inline mode on pfSense)
      4.Firewall: pfSense
      5.SIEM (optional): Wazuh / Graylog

Sample Topology Diagram:
[Client VM] → [Switch/VLAN] → [NAC] → [Firewall (pfSense)] → [IPS/Suricata] → [Internet]
                                        ↳ [NDR/Zeek Sensor] ↳ [SIEM]

🧠 Learning Objectives
-------------------------------------------
Understand how each control fits into a layered defense strategy.

Deploy and configure open-source or enterprise-grade equivalents.

Detect, prevent, and respond to simulated threats.

Integrate logging and event correlation across all layers.

Produce professional documentation and operational insights.

🗓️ Study Plan Summary
--------------------------------------------
| Phase | Weeks | Focus Area                   | Tools                   |
| ----- | ----- | ---------------------------- | ----------------------- |
| 1     | 1–2   | Networking & Lab Setup       | pfSense, Wireshark      |
| 2     | 3–4   | Network Access Control       | PacketFence / Cisco ISE |
| 3     | 5–6   | Network Detection & Response | Zeek, Security Onion    |
| 4     | 7–8   | Intrusion Prevention System  | Suricata / Snort        |
| 5     | 9–10  | Firewalls & NGFW Concepts    | pfSense / Palo Alto VM  |
| 6     | 11–12 | Integration & Operations     | Full Stack Integration  |


🧪 Lab Details
--------------------------------------------
🔸 NAC (Network Access Control)
Objective: Enforce endpoint authentication and posture-based access.
Key Activities:
  Configure 802.1X authentication with FreeRADIUS
  Create guest and BYOD onboarding policies
  Assign VLANs based on compliance status
  Simulate compliant and non-compliant devices

🔸 NDR (Network Detection & Response)
---------------------------------------------
Objective: Monitor and analyze network traffic for anomalies.
Key Activities:

Deploy Zeek/Security Onion to capture and inspect flows

Generate malicious traffic using Kali Linux

Analyze Zeek logs (conn.log, dns.log, http.log)

Create basic detection scripts and dashboards

🔸 IPS (Intrusion Prevention System)
---------------------------------------------
Objective: Segment, control, and secure network traffic.
Key Activities:

Configure firewall rules (inbound/outbound)

Set up NAT, DMZ, and VPNs

Test rule enforcement and logging

Explore NGFW concepts (App-ID, SSL inspection)

🔗 Integration & SIEM
----------------------------------------------
Goal: Combine all controls into a unified detection and response flow.

Steps:

Route NAC VLANs through pfSense.

Mirror traffic to Zeek/NDR sensor.

Inline Suricata IPS for prevention.

Forward logs to Wazuh/Graylog SIEM.

Correlate alerts and document incidents.

Result:
Full visibility from endpoint access → network detection → prevention → response.

📘 Key Takeaways
------------------------------------------------
Learned to integrate multiple open-source and enterprise-grade tools.

Gained practical experience with traffic analysis, detection tuning, and access control.

Built a reusable virtual lab for continuous experimentation.

Developed documentation and reporting skills relevant to SOC and NetSec roles.

🧰 Tools Summary
------------------------------------------------
| Category       | Tools Used                        |
| -------------- | --------------------------------- |
| Virtualization | VirtualBox / VMware               |
| NAC            | PacketFence / Cisco ISE           |
| NDR            | Zeek / Security Onion             |
| IPS            | Suricata / Snort                  |
| Firewall       | pfSense / OPNsense / Palo Alto VM |
| SIEM           | Wazuh / Graylog                   |
--------------------------------------------------
🧾 Future Enhancements

Automate response workflows with TheHive / Cortex.

Add threat intelligence feeds for NDR/IPS correlation.

Deploy microsegmentation using VLAN or SDN tools.

Explore cloud-based equivalents (Azure Firewall, AWS GuardDuty, etc.).

📚 References
--------------------------------------------------
https://packetfence.org/documentation.html

https://docs.securityonion.net/en/2.4/

https://suricata.io/

https://docs.netgate.com/pfsense/en/latest/

https://zeek.org/
