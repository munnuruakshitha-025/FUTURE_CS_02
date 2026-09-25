# FUTURE_CS_02 - Phishing Detection & Awareness Report

## Overview
This report analyzes phishing email samples to identify common 
attack indicators and provide practical, non-technical prevention 
guidance for employees. The goal is to help users recognize and 
avoid phishing attempts before they cause harm — this is security 
education, not offensive testing.

## Scope
- Passive analysis only — no links were clicked, no attachments 
  were opened, no interaction with malicious infrastructure
- Sample emails were sourced from the task's own reference example 
  and from public, labeled educational phishing datasets

## Samples Analyzed

### Sample 1: Fake Account Lock Alert
- Source: Task reference example
- Classification: Phishing (High confidence)
- Key indicators: Suspicious sender domain, urgency/fear-based 
  language, generic greeting, mismatched verification link

### Sample 2: Fake Fax Notification
- Source: Public educational dataset (autinerd/phishing-mail-examples)
- Classification: Phishing (High confidence)
- Key indicators: Garbled/spoofed sender display name, mismatched 
  sender domain, urgency/curiosity bait, link destination mismatch, 
  inconsistent branding (MetroFax + unrelated NHS footer)

### Sample 3: Fake Voicemail Notification
- Source: Public educational dataset (autinerd/phishing-mail-examples)
- Classification: Phishing (Very High confidence)
- Key indicators: Failed SPF, DKIM, and DMARC authentication checks 
  (technically confirmed spoofing, not just visual suspicion), 
  homoglyph character substitution to evade spam filters, urgency 
  bait, suspicious third-party image hosting

## Analysis Approach
1. Reviewed email headers for sender authenticity (From, Return-Path, 
   authentication results where available)
2. Checked link destinations by inspection only, without clicking
3. Identified psychological/social engineering patterns (urgency, 
   fear, curiosity, generic targeting)
4. Classified each email as Safe / Suspicious / Phishing based on 
   combined evidence
5. Documented findings in plain, non-technical language suitable 
   for a business awareness report

## Tools Used
- Manual email header and content analysis
- Public educational phishing datasets (referenced for study only, 
  not reused or claimed as original)
- Canva (report design and formatting)

## Key Learning
Phishing attacks succeed primarily by exploiting human trust and 
urgency, not by breaking technical systems. Even sophisticated 
attempts (like Sample 3) leave detectable technical evidence when 
email authentication is properly checked — but user awareness 
remains the first and most important line of defense.

## Files
- - [Report.pdf](./Report.pdf) — Full Phishing Detection & Awareness Report
- `sample-01-task-example.txt` — Fake account lock phishing sample
- `sample-02-fake-fax-notification.txt` — Fake fax notification sample
- `sample-03-fake-voicemail.txt` — Fake voicemail sample
