---
title: Threat Analysis
description: Phishing detection and investigation case study
date: 2026-02-26
category: Blue Team / SOC
---

[← Home](/)

# 📧 Email & Phishing Analysis

This case study focuses on identifying, analyzing, and responding to phishing attacks commonly encountered in Security Operations Centers (SOC). 🛡️

---

## 🎯 Objective

- Detect malicious email campaigns
- Analyze spoofed sender domains
- Extract Indicators of Compromise (IOCs)
- Produce SOC-style reports

---

## 🛠️ Tools Used

- Email Header Analyzer  
- VirusTotal  
- WHOIS Lookup  
- Browser DevTools  

---

## 🧪 Investigation Process

1. Collected suspicious email samples  
2. Analyzed email headers  
3. Verified sender domain  
4. Extracted URLs and hashes  
5. Checked reputation databases  

---

## 🔍 Findings

- Detected spoofed sender address
- Malicious URL hosted on suspicious domain
- Payload linked to phishing campaign
- High risk score on reputation tools

---

## ✅ Outcome

- Classified as Phishing (High Risk)
- Report submitted
- Domain recommended for blocking
- User awareness advised

---

## 📚 Lessons Learned

- Importance of header analysis
- How attackers spoof domains
- Faster IOC identification
- Better incident documentation

---

## 📷 Evidence & Analysis

### 1️⃣ Initial Compromise Detection
![Phishing Analysis Screenshot](/sample.jpg)

**Explanation:**  
The attacker successfully gained unauthorized access to a target endpoint. The source IP address was correlated with suspected Command-and-Control (C2) infrastructure.

---

### 2️⃣ C2 Beaconing Identification
![Phishing Analysis Screenshot](/sample.jpg)

**Explanation:**  
Log analysis revealed consistent and periodic outbound connections, indicating C2 beaconing behavior based on repeated time intervals and traffic patterns.