---
title: "Network Testing"
date: 2018-11-18T12:33:46+10:00
weight: 2
date: 2024-03-18 
layout: page
description: The best defense is a good offense.
image: "/images/illustrations/network.webp"
---

[External](#external) testing of your Internet-facing perimeter, or [Internal](#internal) testing to simulate an insider threat or rogue employee. Blend both, or add on [Phishing](/services/phishing) for a well-rounded engagement.
<!--more-->

![hacking webapp](/images/illustrations/network.webp){: width="600"}
<!-- TOC --><a name="external"></a>
# External Penetration Tests 
## Objective:
External Penetration Tests are designed to evaluate the security posture of an organization's external network assets, such as websites, web applications, and network interfaces, to identify vulnerabilities that could be exploited by external threats. The aim is to assess the resilience of the organization’s public-facing infrastructure against internet-based attacks, ensuring that security measures are capable of preventing unauthorized access or data compromise.

## Methodology:
The assessment process includes a comprehensive examination of all internet-facing assets, including web servers, email servers, DNS servers, and firewalls. The methodology integrates a mix of automated scanning tools and manual testing techniques to uncover a range of security issues, such as misconfigurations, outdated software, weak encryption methods, and other vulnerabilities in exposed services. Main features include:

- **Open Source Intelligence (OSINT):** Gathering publicly available information to aid in identifying potential attack vectors and understanding the organization's external digital footprint.
- **Network Scanning and Analysis:** Systematic scanning of all external IP addresses and domain names to map out accessible services and identify potential vulnerabilities.
- **Exploitation:** Attempting to exploit identified vulnerabilities to assess the potential for unauthorized access or information exfiltration, simulating the actions of real-world attackers.
- **Lateral Movement:** Evaluating the possibility of moving across the network to access additional resources or sensitive information, demonstrating how an attacker could extend their reach within the compromised infrastructure.

Goal-Based Penetration Testing focuses testing based on specific objectives, such as accessing sensitive data, compromising critical systems, or evaluating the effectiveness of security controls and incident response mechanisms.

This testing emulates real-world threat actors, employing tactics, techniques, and procedures (TTPs) used in actual cyber attacks. It goes beyond the scope of automated or scanner-based vulnerability assessments by incorporating a strategic approach to identify and exploit vulnerabilities, providing a comprehensive evaluation of the organization’s ability to protect against and respond to external threats. 

## Scoping Parameters:
Scoping requires the identification of all external IP addresses and domain names to ensure comprehensive coverage. It must clearly outline testing objectives and document any out-of-scope elements to avoid unintended disruptions. The testing period is agreed upon to minimize operational impact.

Targets refers to live systems on the external perimeter exposing at least one port or service. If you provide a /24 for testing, and only 30 systems are found to be live and hosting at least one port or service, the scope should be 30, not 255. 

<!-- TOC --><a name="internal"></a>
# Internal Penetration Tests 
## Objective:
Internal Penetration Testing targets an organization's internal network and systems to identify vulnerabilities that could be exploited by insiders or attackers who have breached the network perimeter. The primary aim is to evaluate the security of internal infrastructure, identify weaknesses in internal controls, and assess the potential impact of insider threats, such as employees, contractors, or compromised accounts.

## Methodology:
This testing methodology focuses on the internal environment, including servers, workstations, network devices, and applications accessible within the network. It employs a combination of automated scanning tools and manual testing techniques to comprehensively assess the security posture of internal systems.

## Features:

- **Network Scanning and Enumeration:** Systematic identification and mapping of network assets, services, and vulnerabilities within the internal network to understand the network's structure and potential attack vectors.
- **Credential Testing and Privilege Escalation:** Examination of authentication mechanisms, password policies, and practices for managing credentials. Testing includes attempts to escalate privileges to gain higher levels of access.
- **Vulnerability Exploitation:** Identifying and exploiting vulnerabilities in software, configurations, and security controls to understand the potential for unauthorized access or data exfiltration.
- **Lateral Movement:** Assessing the ability to move laterally across the network to access additional systems and data, simulating how an attacker could extend their reach within the network after gaining initial access.
- **Access Controls and Segmentation:** Evaluating the effectiveness of network segmentation and access controls in limiting movement and access to sensitive areas of the network.
- **Sensitive Data Exposure:** Assessing the protection mechanisms for sensitive data to determine if such data can be accessed or exfiltrated by unauthorized users.
- **Incident Detection and Response:** Testing the organization's ability to detect and respond to internal security incidents, including the effectiveness of monitoring, logging, and incident response processes.

This methodology aims to emulate real-world scenarios where an attacker has internal access, providing a realistic assessment of the organization's internal security posture. It goes beyond simple vulnerability scanning by incorporating manual testing and exploitation techniques to understand the real-world implications of identified vulnerabilities.

## Engagement Scale and Duration:
The scale and duration of an internal penetration test can vary based on the size of the internal network, the number of systems to be tested, and the depth of the testing required. Engagements can range from focused assessments of specific network segments or applications to comprehensive testing of the entire internal network.

## Scoping Parameters:
Testing treats the entire LAN (and all attached systems) as in-scope. For target selection, pick a sampling of critical systems. Consider domain controllers, database servers, systems in varying security zones (cloud environments, DMZs, etc), and supporting infrastructure. 

When scoping, consider the goals of the engagement. Is it to see if an attacker in a general user environment could work their way to a protected cloud VPC? To a OT factory floor? To systems in a connected office environment across the country? Consider placing systems from those environments into the targets list. Also consider providing a no-strike list of systems that should not be touched during testing (historically sensitive or critical systems).

---
# Lets Chat
If you're interested in pricing or methodology for this service (or any others), fill out the form and we will be in touch!
{% include contact-form.html %}
