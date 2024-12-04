# Cybersecurity Analysis: DNS and ICMP Traffic Investigation

This project is part of the Google Cybersecurity Professional Certificate, focusing on analyzing DNS and ICMP traffic to identify the root cause of a network-related incident. It demonstrates the use of **tcpdump** to investigate network protocols and provides an incident report based on the findings.

---

## 📋 Project Overview

### Scenario
A client reported that their website, **www.yummyrecipesforme.com**, was inaccessible, displaying the error message: **"destination port unreachable."** As a cybersecurity analyst, I analyzed packet data using **tcpdump** to identify and troubleshoot the issue.

### Objective
- Use a network protocol analyzer to capture and analyze **DNS** and **ICMP** traffic.
- Determine which network protocol and service were affected during the incident.
- Summarize findings in a professional cybersecurity incident report.

---

## 📂 File Contents

### 1. `tcpdump_log.txt`
- Contains the raw tcpdump logs captured during the analysis.
- Displays UDP requests and ICMP error messages for DNS traffic.

### 2. `Incident_Report.pdf`
- A detailed incident report summarizing the problem, analysis, and findings.
- Explains the cause of the incident: the **DNS server's port 53** was not listening, resulting in ICMP error messages.

### 3. `README.md` (this file)
- An overview of the project, scenario, and key takeaways.

---

## 🔍 Key Findings

- **Error Identified:** UDP packets sent to the DNS server on port 53 resulted in **ICMP "udp port 53 unreachable"** error messages.
- **Cause:** The DNS server was not listening on port 53, preventing the domain name resolution process.
- **Impact:** End-users were unable to access the client's website.

---

## 🛠️ Tools and Skills Demonstrated

- **Network Protocol Analysis:**
  - Utilized **tcpdump** to capture and examine network traffic.
  - Analyzed ICMP and DNS protocols in transit.
- **Incident Response:**
  - Identified potential risks and communicated findings in an incident report.
- **Technical Writing:**
  - Structured a clear and concise report for stakeholders.

---

## 📖 How to Use This Repository

1. **Explore the tcpdump Logs:**
   - Open the `tcpdump_log.txt` file to examine the captured traffic.
2. **Review the Incident Report:**
   - The `Incident_Report.pdf` explains the findings and provides a root cause analysis.
3. **Use for Learning:**
   - Reference this project as an example of network analysis and reporting.

---

## 🏆 Key Takeaways

- Understanding DNS and ICMP traffic is essential for diagnosing network issues.
- Tools like **tcpdump** can provide critical insights during cybersecurity incidents.
- Clear communication of findings is a vital skill for cybersecurity analysts.

---

### License

This project is for educational purposes and is shared under the MIT License.
