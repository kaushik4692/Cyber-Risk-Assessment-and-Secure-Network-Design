# Cyber Risk Assessment and Secure Network Design for a Mid-Sized Enterprise

## Project Overview

This project simulates a cybersecurity assessment engagement for a mid-sized enterprise. The objective was to identify security risks within the organization's network infrastructure and implement security controls to reduce the attack surface and protect critical business resources.

The network was designed and simulated using Cisco Packet Tracer.

---

## Business Scenario

ABC Manufacturing Pvt. Ltd. required a review of its network security posture due to concerns regarding:

* Unauthorized access to sensitive finance systems
* Guest users accessing internal resources
* Insecure remote administration
* Unauthorized endpoint connections

---

## Network Architecture

The network consists of:

* HR Department (VLAN 10)
* Finance Department (VLAN 20)
* IT Department (VLAN 30)
* Guest Network (VLAN 40)
* Server Network (VLAN 50)

Inter-VLAN routing was implemented using Router-on-a-Stick architecture.

---

## Security Risks Identified

| Risk                             | Severity |
| -------------------------------- | -------- |
| HR access to Finance resources   | High     |
| Guest access to internal network | Critical |
| Unsecured remote administration  | Medium   |
| Unauthorized device connection   | High     |

---

## Security Controls Implemented

### VLAN Segmentation

Separated departments into dedicated VLANs to reduce lateral movement.

### Access Control Lists (ACLs)

Implemented ACLs to restrict unauthorized communication between network segments.

### Guest Network Isolation

Blocked guest users from accessing internal company resources.

### SSH Secure Management

Replaced insecure management access with encrypted SSH communication.

### Port Security

Restricted switch ports to authorized devices and configured automatic shutdown on violations.

---

## Validation Results

| Test                           | Result  |
| ------------------------------ | ------- |
| HR → Finance Access            | Blocked |
| Guest → Internal Server Access | Blocked |
| IT → Server Access             | Allowed |
| SSH Management                 | Enabled |
| Port Security                  | Enabled |

---

## Technologies Used

* Cisco Packet Tracer
* VLANs
* Access Control Lists (ACLs)
* Router-on-a-Stick
* SSH
* Port Security

---

## Author

Kaushik Das
B.Tech, Applied Electronics & Instrumentation Engineering
University of Burdwan

