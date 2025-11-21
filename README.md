<h1> 🛡 Cyber Security Internship – Task 2</h1>  
<h2> Security Alert Monitoring & Incident Response (SOC Simulation)</h2>

### ✉ Basic Information
- **Tool Used:** Splunk SIEM  
- **Dataset:** SOC_Task2_Sample_Logs  
- **Objective:** To monitor, detect, and analyze suspicious security events within a simulated enterprise environment and prepare an incident response summary.

---

### 🔍 Key Findings
During the log analysis using Splunk, several suspicious patterns were detected:

- **Malware Activity:**  
  Trojan malware detected on host system **172.16.0.3 (user=bob)**, indicating a possible infection or compromise.

- **Unauthorized Login Attempts:**  
  Multiple failed login attempts were recorded, suggesting potential **brute-force** or **credential theft** attempts.

- **Unusual Network Connections:**  
  Outbound connections were detected from internal systems to unknown or unauthorized IP addresses, potentially linked to **command-and-control (C2)** activity or **data exfiltration** attempts.

These findings highlight a mix of **high and medium-risk events** that required containment and further analysis.

---

### 📈 Severity Classification
Based on the analysis of the simulated logs, the detected threats were classified according to their potential impact and risk level:

- **Trojan Malware Detection (High Severity):**  
  Confirmed malicious activity observed on host **172.16.0.3 (user=bob)**, indicating a successful infection that could lead to data theft, unauthorized access, or lateral movement within the network.

- **Multiple Failed Logins (Medium Severity):**  
  Repeated authentication failures suggest a **brute-force** or **password spraying** attack aimed at gaining unauthorized access.

- **Suspicious Network Connections (Medium Severity):**  
  Outbound connection attempts from internal systems to unknown IPs, suggesting possible **C2 communication** or reconnaissance by a compromised endpoint.

---

### 📃 Testing & Validation
To verify the system’s ability to detect and classify security incidents, multiple Splunk queries were executed, including analysis of:
- Raw log dashboard  
- Successful and failed logins  
- File access activity  
- Connection attempts  
- Malware detection logs  

Each result confirmed the correct correlation and visualization of suspicious events in the Splunk dashboard.  

---

### 🔷 Summary & Conclusion
This analysis successfully simulated a **real-world SOC workflow** — from log ingestion to threat detection, severity classification, and incident response.

The **Trojan malware detection** was identified as the most critical threat, followed by **unauthorized login attempts** and **suspicious network activity**.  
Using Splunk’s SIEM capabilities, all alerts were correlated and contained effectively.

Preventive recommendations such as **MFA implementation**, **NTP synchronization**, and **enhanced monitoring** were proposed to improve future resilience against cyber threats.

---
