Day 3 - Source Validation & Analytical Notes
Overview

This document supplements Day 3 OSINT activities by documenting source material, collection dates, validation methods, confidence levels, and analytical observations. The objective is to distinguish observed facts from analytical conclusions and maintain transparency throughout the investigation process.

Finding D3-F001: Domain Registration Information
Observation

WHOIS records were collected for microsoft.com.

Source

WHOIS Record

Collection Date

05 November 2026

Source Output
Plain Text
Domain Name: MICROSOFT.COM
Registrar: MarkMonitor Inc.
Creation Date: 1991-05-02
Registry Expiry Date: 2027-05-03
DNSSEC: unsigned
Evidence
Plain Text
Evidence/microsoft_whois.txt
Screenshot: 002 Whois MS.png
Screenshot: 003 whois output.png
Validation

The information was obtained directly from WHOIS registration records and reviewed against supporting DNS information.

Confidence Level

High

Assessment

The collected WHOIS data provided registration and ownership-related information for the domain at the time of collection.

Limitations

WHOIS records reflect information available at the time of collection and may change in the future.

Finding D3-F002: DNS Infrastructure Identification
Observation

DNS infrastructure associated with microsoft.com was identified.

Source

WHOIS Record and DNS Queries

Collection Date

05 November 2026

Source Output
Plain Text
NS1-39.AZURE-DNS.COM
NS2-39.AZURE-DNS.NET
NS3-39.AZURE-DNS.ORG
NS4-39.AZURE-DNS.INFO
Evidence
Plain Text
Evidence/microsoft_whois.txt
Evidence/microsoft_dns.txt
Screenshot: 003 whois output.png
Validation

Name server information identified within the WHOIS records was supported by DNS query results collected during the exercise.

Confidence Level

High

Assessment

The domain was configured to use Azure DNS name servers during the collection period.

Limitations

DNS configurations may change over time and represent a point-in-time observation.

Source Reliability Assessment
Source	Reliability	Reason
WHOIS	High	Information obtained directly from domain registration records.
DIG	High	Direct DNS query responses.
WhatWeb	Medium	Technology fingerprinting relies on observable responses and may not reveal complete infrastructure details.
Revised Findings
RF-D3-001
Initial Assumption

Microsoft uses Azure DNS infrastructure.

Validation

WHOIS records identified Azure DNS name servers, and DNS queries confirmed active resolution during the collection period.

Final Assessment

The evidence supports the conclusion that microsoft.com was configured with Azure DNS name servers at the time of collection.

Status

Confirmed

False Positive Review
FP-D3-001
Review Outcome

No false positives were identified during Day 3 activities.

Analyst Note

All findings were derived from direct WHOIS and DNS outputs and were supported through validation during the collection process.