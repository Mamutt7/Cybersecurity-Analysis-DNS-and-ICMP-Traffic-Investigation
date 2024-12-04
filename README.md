# Cybersecurity Scenario: DNS and ICMP Traffic Investigation

This project is part of the Google Cybersecurity Professional Certificate, focusing on analyzing simulated DNS and ICMP traffic logs to diagnose and document network-related incidents. The exercise demonstrates network analysis and incident reporting skills.

---

## 📋 Project Overview

### Scenario
A client reported issues accessing their website, **www.yummyrecipesforme.com**, with the error message: **"destination port unreachable."** As part of this simulated exercise, I analyzed the provided `tcpdump` log data to diagnose the issue.

---

## 🔍 Key Findings

- **Error Identified:** UDP packets sent to the DNS server on port 53 resulted in ICMP "udp port 53 unreachable" error messages.
- **Cause:** The DNS server was not listening on port 53, preventing DNS queries from resolving the domain name.
- **Impact:** Users were unable to access the client's website due to failed DNS resolution.

---

## 🛠️ Skills Demonstrated

- **Network Traffic Analysis:**
  - Interpreted DNS and ICMP traffic logs to identify root causes.
- **Incident Response:**
  - Diagnosed issues with DNS protocols and provided actionable findings.
- **Technical Writing:**
  - Summarized findings and analysis in a concise incident report.

---

## 📖 Incident Report Summary

### Part 1: Summary of the Problem
The UDP protocol analysis reveals that DNS queries sent from the client computer (IP: `192.51.100.15`) to the DNS server (IP: `203.0.113.2`) failed, with ICMP error messages indicating "udp port 53 unreachable." Port 53, used for DNS services, was unresponsive, likely due to a misconfiguration or the DNS service not running on the server. This caused DNS resolution to fail, making the website inaccessible.

### Part 2: Analysis of the Data and Incident Causes
The incident occurred at multiple timestamps, starting at **13:24:32**. The IT team became aware of the issue through customer reports of the website being unreachable, confirmed by replication of the error. Using **tcpdump**, they analyzed network traffic and identified that UDP packets to port 53 were met with ICMP error responses. The root cause was determined to be a misconfigured or inactive DNS server, which prevented proper DNS resolution.

---

## 📷 Screenshot of Network Logs

Below is a sample of the provided `tcpdump` logs analyzed during the exercise:

![image](https://github.com/user-attachments/assets/3c68fe98-bed0-4d30-9d05-f6244b422398)


---

## 🏆 Key Takeaways

- Understanding how to interpret DNS and ICMP traffic is essential for diagnosing network issues.
- Tools like **tcpdump** are critical for identifying protocol-related failures.
- Clear documentation of findings is crucial for effective incident response and reporting.

---

### License

This project is shared for educational purposes and is licensed under the MIT License.
