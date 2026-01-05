# Home Network Security Assessment

## Overview
This project presents a basic security assessment of a small home network. The purpose of the assessment was to identify common security risks, evaluate the current security posture, and apply basic hardening measures aligned with CompTIA Security+ principles.

This project simulates real-world entry-level IT and security tasks such as reviewing configurations, assessing risk, and documenting mitigations.

---

## Assessment Scope
**In Scope**
- Home router and wireless access point
- Personally owned client devices
- Router configuration review
- Basic network scanning

**Out of Scope**
- Exploitation or penetration testing
- Devices not owned by the author
- External or unauthorized networks

All activities were performed on personally owned equipment with proper authorization.

---

## Network Overview
The assessed network consists of a consumer-grade router connected to an ISP modem, supporting both wired and wireless client devices.

![Network Diagram](diagrams/network-diagram.png)

---

## Threat Model
The assessment focused on common home network threats, including:
- Unauthorized wireless access
- Weak or default router credentials
- Unpatched firmware vulnerabilities
- Unnecessary exposed services
- Malware introduced through user behavior

Threats were evaluated using the **CIA Triad**:
- **Confidentiality**
- **Integrity**
- **Availability**

---

## Tools & Methodology
The following tools and methods were used:
- Router administrative interface review
- Operating system security configuration review
- Basic network scanning using `nmap`
- Manual inspection of settings and services

No intrusive or destructive testing was performed.

---

## Key Findings
| Finding | Risk Level | Impact |
|------|-----------|--------|
| Default SSID name | Low | Information disclosure |
| Outdated router firmware | Medium | Exposure to known vulnerabilities |
| UPnP enabled | Medium | Increased attack surface |
| Weak administrative credentials | High | Unauthorized router access |

Risk levels were determined based on likelihood and potential impact.

---

## Mitigations & Hardening
The following security improvements were implemented:
- Changed router administrative credentials to a strong, unique password
- Updated router firmware to the latest available version
- Disabled UPnP to reduce unnecessary exposure
- Enabled WPA3 wireless encryption
- Configured a separate guest wireless network

These changes reduced risk while maintaining usability for daily network use.

---

## Before & After Comparison
**Before**
- Default SSID
- Outdated firmware
- UPnP enabled
- Weak administrative credentials

**After**
- Custom SSID
- Firmware fully updated
- UPnP disabled
- Strong administrative credentials
- WPA3 encryption enabled

---

## Lessons Learned
- Even small configuration changes can significantly reduce security risk
- Firmware patching is a critical but often overlooked control
- Convenience features can introduce security trade-offs
- Clear documentation improves repeatability and accountability

---

## Future Improvements
- Segment IoT devices onto a separate network
- Enable centralized logging and monitoring
- Perform periodic vulnerability scans
- Develop a basic incident response plan

---

## Disclaimer
This project was completed for educational purposes only. All testing was conducted on personally owned equipment with proper authorization.

## CompTIA Security+ Domain Mapping

This project aligns with multiple CompTIA Security+ domains by applying core security concepts to a real-world home network environment.

### 1. Threats, Attacks, and Vulnerabilities
- Identified common home network threats such as unauthorized wireless access and exposed services
- Evaluated risks associated with outdated firmware and weak administrative credentials
- Reduced attack surface by disabling unnecessary services (e.g., UPnP)

### 2. Architecture and Design
- Reviewed and documented the network architecture of a small home environment
- Applied secure network design principles, including network isolation through a guest wireless network
- Considered availability and usability when implementing security controls

### 3. Implementation
- Implemented secure wireless configurations (WPA3 encryption)
- Applied strong authentication practices for router administrative access
- Updated firmware to remediate known vulnerabilities
- Hardened router configurations based on best practices

### 4. Operations and Incident Response
- Conducted routine security checks and configuration reviews
- Assessed potential impact of security incidents such as unauthorized access or malware infection
- Documented lessons learned to improve future response and prevention efforts

### 5. Governance, Risk, and Compliance
- Defined assessment scope and ensured proper authorization
- Performed basic risk analysis based on likelihood and impact
- Documented findings, mitigations, and security decisions
