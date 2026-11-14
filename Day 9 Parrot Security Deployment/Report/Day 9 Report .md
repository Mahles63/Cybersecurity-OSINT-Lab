Day 9 Report
Parrot Security OS Deployment & Environment Validation
Date: 14 November 2026

Executive Summary
The objective of Day 9 was to deploy and validate a Parrot Security OS environment as a secondary cybersecurity assessment platform alongside the existing Kali Linux laboratory.

Activities included operating system validation, package repository verification, security tool validation, network connectivity testing, workspace preparation, and initial reconnaissance activities.

The deployment was successful, and the environment was confirmed operational for future reconnaissance, OSINT, vulnerability assessment, and reporting activities.

Scope
The assessment focused on:

Parrot Security OS deployment
Environment validation
Security tool verification
Network connectivity testing
Workspace preparation
Initial reconnaissance testing
Tools Utilized
Parrot Security OS
Nmap
WhatWeb
Curl
Linux Networking Utilities
Oracle VirtualBox
Activities Performed
Environment Validation
Validated installation and operating system information.

Commands performed:

whoami

hostname

cat /etc/os-release

uname -a

Repository Validation
Verified package repository connectivity.

Command:

sudo apt update

Tool Verification
Validated assessment tools.

Commands:

nmap --version

whatweb --version

nikto -Version

amass -version

Network Validation
Confirmed interface configuration and internet connectivity.

Commands:

ip a

ping -c 4 scanme.nmap.org

Initial Reconnaissance
Performed technology fingerprinting and HTTP header collection.

Commands:

whatweb https://scanme.nmap.org

curl -I https://scanme.nmap.org

Conclusion
Parrot Security OS was successfully deployed and validated as a functional assessment platform. Core security tools were verified, network connectivity was confirmed, and the environment is ready for future security assessments and reconnaissance exercises.