# FUTURE_CS_02 - Phishing Detection & Awareness Report

## Overview
This report analyzes phishing email samples to identify common 
attack indicators and provide practical prevention guidance for 
employees.

## Samples Analyzed
- Sample 1: Fake Account Lock Alert (task-provided example)
- Sample 2: Fake Fax Notification (educational dataset)
- Sample 3: Fake Voicemail Notification (educational dataset)

## Approach
- Header analysis (sender domain, authentication results)
- Link inspection (without clicking)
- Language pattern analysis (urgency, tone, greetings)
- Classification: Safe / Suspicious / Phishing

## Tools Used
- Manual email header analysis
- Public educational phishing datasets (for study, not reused as-is)
- Canva (report design)

## Summary of Findings
All 3 analyzed samples were classified as Phishing, ranging from 
High to Very High confidence. Common indicators included spoofed 
sender domains, urgency-based language, mismatched links, and — 
in one case — technically confirmed email authentication failures 
(SPF/DKIM/DMARC). Full analysis and prevention guidelines are in 
the attached report.

## Files
- `Report.pdf` — Full Phishing Detection & Awareness Report
- `sample-*.txt` — Analyzed email samples with indicators noted
