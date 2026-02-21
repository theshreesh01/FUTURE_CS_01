Vulnerability Assessment Report

Project Overview
This project presents a structured vulnerability assessment conducted on a public web application. The assessment was performed using passive security analysis techniques without exploiting or modifying any system data.
The objective of this project is to identify configuration-level security weaknesses and provide actionable remediation recommendations.


Target
http://testphp.vulnweb.com


Assessment Type
Passive Security Analysis (Read-Only)
No exploitation, brute force, or intrusive testing methods were used during this assessment.

Identified Vulnerabilities
1️⃣ Insecure Communication (No HTTPS) – High Risk

The website operates over HTTP instead of HTTPS, exposing user data to interception risks such as man-in-the-middle attacks.

2️⃣ Missing Security Headers – Medium Risk

Important security headers such as:

X-Frame-Options

Content-Security-Policy

X-Content-Type-Options

Strict-Transport-Security

were not implemented, reducing browser-level protections.

3️⃣ Server & Version Disclosure – Medium Risk

The server reveals backend technologies and version details, which may assist attackers in identifying known vulnerabilities.

📊 Risk Summary
Vulnerability	Risk Level
No HTTPS	High
Missing Security Headers	Medium
Version Disclosure	Medium

Tools Used
Nmap

Browser Developer Tools
Manual HTTP Response Inspection

Evidence
Screenshots and supporting evidence are available in the evidence folder.

Conclusion
This assessment demonstrates how publicly visible misconfigurations can significantly impact a website’s security posture. Implementing HTTPS, configuring proper security headers, and suppressing version disclosure would greatly enhance confidentiality, integrity, and overall trustworthiness.

Prepared By
Shreesh Kumar
