Home Lab: Web Security & Firewalling
This repository documents a foundational home lab project designed to demonstrate and practice fundamental concepts in web application security, network defense, and ethical hacking. The lab consists of a vulnerable web application (DVWA), a dedicated firewall, and a separate attacking machine used to exploit vulnerabilities.

🚀 Features:

DVWA Setup: Instructions for setting up a Damn Vulnerable Web Application (DVWA) server.

Firewall Integration: A guide to configuring a firewall to filter and protect the web server.

Simulated Attacks: A walkthrough of using a separate machine to conduct attacks and observe firewall effectiveness.

📋 Prerequisites:

To replicate this lab, you will need the following software and an environment capable of running virtual machines:

Virtualization Software:

VirtualBox or VMware Workstation Player

Operating Systems:


A Linux distribution for the web server (e.g., Ubuntu Server).

A penetration testing-focused Linux distribution for the attacking machine (e.g., Kali Linux).

A dedicated OS for the firewall (e.g., IPtables on Linux or a standalone firewall OS).

💻 Setup and Usage:

Follow these steps to set up your home lab:

Server Setup: Install the chosen Linux distribution for your web server. Install and configure the DVWA application following its official documentation.

Firewall Configuration: Install and configure your chosen firewall software on a dedicated machine. Ensure it is placed in a network topology where all traffic to the DVWA server must pass through it (I used Safeline WAF).

Attacker Machine: Set up the Kali Linux virtual machine and ensure it has network connectivity to the DVWA server.

Execute Attacks: From the Kali Linux machine, use tools like sqlmap, Burp Suite, or Nmap to test the DVWA server. Observe how the firewall reacts and whether it successfully blocks the attacks.

For a detailed visual guide and reference, you can watch the following video:

🛡️ Attack Scenarios & Defenses:

This lab was used to test and defend against the following specific attack types:

SQL Injection: Exploiting vulnerabilities in web application inputs to manipulate SQL queries.

Authentication: Testing for weak authentication methods and brute-force vulnerabilities.

HTTP Flood: Simulating a denial-of-service attack to test the firewall's rate-limiting capabilities.

IP Blocking: Demonstrating how the firewall can be configured to block malicious IP addresses.

🛠️ Tools Used:

VirtualBox or VMware

Safeline WAF (or another firewall solution)

Kali Linux

DVWA (Damn Vulnerable Web Application)

⚠️ Disclaimer:

This project is for educational and research purposes only. The techniques and methods described should only be used in a controlled, isolated lab environment. Unauthorized access to computer systems is illegal and unethical.

📄 License:

This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgements:

The DVWA project for providing a safe environment to practice security.

The community of ethical hackers and security researchers.

The creator of the referenced YouTube video for the inspiration.
