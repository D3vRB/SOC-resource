---
title: SIEM Triage for SOC (Elastic)
description: Hands-on SIEM investigation using Splunk to analyze Linux security logs, detect brute force attacks, privilege escalation, and persistence techniques through real-world SOC scenarios.
date: 2026-02-26
category: Blue Team / SOC
---

[← Home](/)

# 📧 SIEM Triage for SOC (Elastic)

Hands-on SIEM investigation using Elastic to analyze suspicious activity on an IIS and Windows server. Exploring potential indicators of compromise (IoCs) and collect evidence by correlating events across multiple log sources to gain a deeper understanding of the attack.

---

## 🎯 Objective

- Use Kibana to analyze common security logs
- Learn how to identify key indicators of compromise
- Correlate events across multiple log sources
- Uncover the breach through a series of SOC alerts

---

## 🛠️ Tools Used

- Elastic

---

## 🧪 Investigation Process

1. Detection & Initial Triage
2. POST Request Filtering
3. Endpoint Investigation
4. User-Agent Analysis
5. Web Shell Activity Investigation
6. Persistence Hunting
7. Command Execution Review

---

## 🔍 Findings

- Repeated POST Requests to proxyLogon.ecp
- Automated Exploit Tool Detected
- Suspicious Web Shell Parameter
- Command Execution via errorEE.aspx

---

## 📚 Lessons Learned

- Importance of Monitoring POST Requests
- Identifying Automated Attack Tools
- Detecting Web Shell Activity
- Timeline-Based Investigation

---

## 📷 Evidence & Analysis

### 1️. Repeated POST Requests to proxyLogon.ecp
![Image](/elastic/elastic01.png)

**Explanation:**  
Elastic web logs were filtered using the query _index:weblogs AND client.ip:203.0.113.55 AND http.request.method:POST.
The results showed three POST requests targeting /ecp/proxyLogon.ecp, which is an Exchange Control Panel endpoint commonly abused in ProxyLogon exploitation attempts.

**Impact:**
- Possible exploitation attempt against Microsoft Exchange
- Unauthorized interaction with sensitive Exchange endpoints
- Early stage of remote server compromise
- Potential web shell deployment

---

### 2. Automated Exploit Tool Detected
![Image](/elastic/elastic02.png)

**Explanation:**  
The user.agent field in the filtered Elastic logs revealed that the POST requests originated from python-requests/2.25.1, a Python HTTP library frequently used in automated scripts and exploitation tools.

**Impact:**
- Indicates automated attack activity
- Suggests the use of exploit scripts rather than a normal browser
- Higher likelihood of vulnerability scanning or exploitation
- Potential scripted attack against Exchange infrastructure

---

### 3. Suspicious Web Shell Parameter
![Image](/elastic/elastic03.png)

**Explanation:**  
Elastic logs were analyzed for the presence of the cmd= parameter in the url.path field. This parameter is commonly used in web shell interfaces to execute operating system commands remotely.

**Impact:**
- Strong indicator of web shell activity
- Remote command execution capability on the server
- Potential attacker control over the compromised system
- Increased risk of persistence and lateral movement

---

### 4. Timeline-Based Investigation
![Image](/elastic/elastic04.png)

**Explanation:**  
The investigation focused on logs containing the endpoint errorEE.aspx at the specified timestamp. This file is often associated with malicious web shells deployed after successful Exchange exploitation, allowing attackers to execute commands remotely through HTTP requests.

**Impact:**
- Confirmed attacker interaction with the compromised server
- Evidence of remote command execution
- Possible privilege escalation or system reconnaissance
- Potential preparation for further post-exploitation activities



