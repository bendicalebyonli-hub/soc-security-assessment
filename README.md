 SOC Network Security Assessment
 Overview
This project demonstrates a real-world Security Operations Center (SOC) workflow through an internal network security assessment.
It includes:
•	 Network reconnaissance
•	Vulnerability detection
•	 Risk analysis
•	Professional SOC reporting
The goal is to simulate how a cybersecurity analyst identifies and communicates risks in an enterprise environment.

 Objectives
•	Identify live hosts and exposed services
•	Detect vulnerabilities using automated scanning
•	Assess risk levels (High / Medium / Low)
•	Provide actionable remediation strategies

 Scope
•	Target Network: 192.168.100.0/24
•	Assessment Type: Internal Security Assessment

 Tools & Environment
Tool	Purpose
Nmap	Network scanning & service enumeration
Kali Linux	Penetration testing environment

 Methodology
The assessment followed structured industry practices:
nmap -sS -p- -sV -O --script vuln 192.168.100.0/24
•	SYN Scan (Stealth scanning)
•	Full Port Scan (All ports)
•	Service Detection
•	OS Fingerprinting
•	Vulnerability Scripts

Key Findings
Finding	Risk	Impact
Vulnerable Web Server	🔴 HIGH	Remote Code Execution
SMB Exposure	🔴 HIGH	Lateral Movement / Credential Theft
RDP Open	🔴 HIGH	Brute-force Attacks
Slowloris DoS	🔴 HIGH	Service Disruption
IoT Devices	🟠 MEDIUM	Data Exposure

 Risk Distribution
HIGH    ██████████ 6
MEDIUM  █████      3
LOW     ██         2

 Critical Alerts
•	 Outdated web server with known vulnerabilities
•	 SMB exposed internally (high lateral movement risk)
•	 RDP accessible without restriction
•	 IoT devices not segmented

 Recommendations
 Immediate (0–7 days)
•	Patch vulnerable systems
•	Disable unused services
•	Restrict SMB & RDP access
 Short Term (1–4 weeks)
•	Implement VLAN segmentation
•	Isolate IoT devices
•	Enforce strong authentication
 Long Term (1–3 months)
•	Deploy SIEM (Wazuh / Splunk)
•	Implement IDS/IPS
•	Continuous vulnerability scanning

 Evidence
Screenshots of scan results are stored in
Examples:
•	Web server vulnerability detection
•	SMB port exposure (139, 445)
•	RDP port (3389) open


 Skills Demonstrated
•	Network Reconnaissance
•	Vulnerability Assessment
•	Risk Analysis
•	Security Reporting (SOC Format)
•	Cybersecurity Documentation

 Why This Project Matters
This project demonstrates the ability to:
•	Think like a SOC Analyst
•	Identify real-world security risks
•	Communicate findings in a professional, business-ready format

 Author
BENDI CALEB YONLI
Cybersecurity Analyst
Contact : +226 71782892 / 0557230269

 Disclaimer
This project was conducted in a controlled lab environment for educational purposes only.
Unauthorized network scanning is illegal.

 Support
If you found this project useful:
•	⭐ Star the repository
•	🍴 Fork it
•	🔗 Share it


