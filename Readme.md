Bug Hunt 101: Security Assessment of OWASP Juice Shop

Student: Hamdan Bin Hashim
Date: January 17, 2026
Project Type: Web Application Penetration Test

Executive Summary

This repository contains the findings from a security assessment conducted on a locally hosted instance of OWASP Juice Shop. The goal was to simulate a real-world bug bounty engagement, moving from reconnaissance to exploitation and reporting.

Vulnerabilities Identified

SQL Injection (SQLi)
Severity: Critical
Description: Allowed authentication bypass to access the Administrator account.

Reflected XSS
Severity: High
Description: Found in the search bar, allowing arbitrary JavaScript execution.

IDOR
Severity: High
Description: Allowed unauthorized access to other users' shopping baskets (Basket ID 6 -> 2).

Repository Structure

Project_Report.pdf: The complete professional vulnerability report.

scans/: Raw output from Nmap reconnaissance.

evidence/: Proof-of-Concept (PoC) screenshots for all findings.

Tools Used

Nmap (Network discovery & service enumeration)

Burp Suite (Traffic interception & Repeater)

Mozilla Firefox (Manual testing)

Disclaimer: This project was conducted in a controlled lab environment for educational purposes.