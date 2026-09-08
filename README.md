# Phishing Email Investigation

## Overview

This project demonstrates a practical Security Operations Center (SOC) investigation of a suspected phishing email.

The investigation focuses on identifying phishing indicators, analyzing suspicious domains and URLs, mapping attacker behavior to the MITRE ATT&CK framework, and developing appropriate incident response and prevention recommendations.

> **Note:** This is a simulated/portfolio investigation created for cybersecurity learning purposes. The indicators used in the investigation should not be interpreted as evidence of a real-world compromise.

---

## Objectives

* Analyze a suspected phishing email.
* Identify Indicators of Compromise (IOCs).
* Investigate suspicious domains, URLs, and IP addresses.
* Identify potential credential-theft behavior.
* Map observed techniques to MITRE ATT&CK.
* Develop containment, eradication, recovery, and prevention recommendations.
* Document findings in a professional SOC investigation report.

---

## Investigation Workflow

```text
Phishing Email
      ↓
Email Analysis
      ↓
IOC Identification
      ↓
Threat Analysis
      ↓
MITRE ATT&CK Mapping
      ↓
Incident Response
      ↓
Final Investigation Report
```

---

## Indicators of Compromise

| Indicator Type | Indicator                                 |
| -------------- | ----------------------------------------- |
| Domain         | `micr0soft-security.com`                  |
| Email Address  | `support@micr0soft-security.com`          |
| IP Address     | `198.51.100.27`                           |
| Suspicious URL | `login-micr0soft-security.example/verify` |

The use of the visually deceptive `micr0soft` domain was identified as an impersonation indicator.

**Important:** `198.51.100.27` belongs to a documentation/example IP range and is included only for simulation purposes.

---

## MITRE ATT&CK Mapping

| Technique | Name                                      | Relevance                                                    |
| --------- | ----------------------------------------- | ------------------------------------------------------------ |
| T1566.002 | Phishing: Spearphishing Link              | Malicious link delivered through phishing email              |
| T1036     | Masquerading                              | Deceptive Microsoft-themed domain                            |
| T1056.002 | Input Capture: GUI Input Capture          | Potential credential capture through a fraudulent login page |
| T1071.001 | Application Layer Protocol: Web Protocols | Web-based communication with the fraudulent page             |

---

## Incident Response

### Containment

* Block suspicious domains and URLs.
* Block the identified sender.
* Quarantine phishing emails.
* Identify additional recipients.
* Disable or reset compromised accounts when necessary.

### Investigation

* Review email headers.
* Search mailboxes for additional copies.
* Review DNS, proxy, firewall, and endpoint logs.
* Identify users who interacted with the phishing link.
* Investigate suspicious authentication activity.

### Eradication

* Remove phishing emails.
* Block malicious indicators across security controls.
* Remove malicious artifacts.
* Reset compromised credentials.
* Revoke active sessions when appropriate.

### Recovery

* Restore affected accounts to a secure state.
* Monitor affected accounts.
* Continue monitoring identified indicators.
* Verify that blocking controls are working correctly.

### Prevention

* Enable Multi-Factor Authentication (MFA).
* Strengthen email security controls.
* Implement SPF, DKIM, and DMARC.
* Improve URL/domain filtering.
* Conduct phishing awareness training.
* Establish a process for reporting suspicious emails.

---

## Evidence

Screenshots documenting the investigation are stored in:

```text
evidence/screenshots/
```

Evidence includes:

1. IOC analysis
2. MITRE ATT&CK mapping
3. Incident response recommendations
4. Final investigation report

---

## Project Structure

```text
Phishing Email Investigation/
│
├── README.md
│
├── analysis/
│   ├── analysis.txt
│   ├── mitre_mapping.txt
│   └── incident_response.txt
│
├── evidence/
│   └── screenshots/
│       ├── 01_ioc_analysis.png
│       ├── 02_mitre_mapping.png
│       ├── 03_incident_response.png
│       └── 04_final_report.png
│
├── iocs/
│   └── iocs.txt
│
└── report/
    └── final_report.txt
```

---

## Skills Demonstrated

* Phishing Email Analysis
* IOC Identification
* Threat Intelligence Analysis
* Domain and URL Analysis
* Email Security
* MITRE ATT&CK Mapping
* Incident Response
* Security Monitoring
* Threat Detection
* Security Documentation
* SOC Investigation Methodology

---

## Conclusion

This project demonstrates an end-to-end phishing investigation workflow from initial email analysis through IOC identification, MITRE ATT&CK mapping, incident response, and final reporting.

The investigation emphasizes the importance of identifying suspicious indicators, containing potential threats, investigating affected users, and implementing controls to reduce the likelihood of successful phishing attacks.
