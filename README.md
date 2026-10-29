# SOC L1 Reports - Lagos Trainee

## Report 001 - Union Bank Phishing
Date: 29 Oct 2026
Title: Phishing Attempt Impersonating Union Bank
Email From: noreply@union-bank-secure.com
Fake Domain: union-bank-secure.com/login
Technique: Added "-secure" to brand, used http (no padlock)
Verification: VirusTotal - 3 vendors flagged as phishing
Action: Block domain, user education
Status: Closed

## Report 002 - GTBank Base64 Analysis
Decoded Base64: R1RCYW5r = GTBank, UGF5c3RhY2s= = Paystack
Learning: Hackers hide brand names in Base64 to bypass filters

## Report 003 - Fake Domain Detection
Real vs Fake:
- gtbank.com = REAL
- gtb-secure-login.com.ng = FAKE (extra -secure-login, http)
- paystack.com-secure.net = FAKE (trick with .com-secure)

Tools Used: VirusTotal, Base64 decoder, URL analysis 
