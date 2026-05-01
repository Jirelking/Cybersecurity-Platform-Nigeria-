
# Use Case 1 - Mitigating Fraudulent Emails at Contoso

## Author
**Name:** Ajireloja Solomon Idowu  
**Role:** Security Analyst  
**Organization (Case Study):** Contoso  
**Date:** 30th April, 2026

## Program
Platform Explorers - Cybersecurity Cohort 2

---

## Project Overview

Contoso is a mid-sized organization with approximately 300 users across the United States and Western Europe. The company has been experiencing an increased volume of **fraudulent and phishing emails** being delivered to user mailboxes, creating a risk of credential theft, business email compromise (BEC), and potential data breaches.

This project documents the **analysis, recommended solution, and configuration steps** implemented to mitigate fraudulent emails using **Microsoft 365 security controls**, with a strong focus on protecting **VIP users** such as the CEO, CFO, and CISO.

---

## Objectives

- Reduce the delivery of phishing and fraudulent emails to users
- Protect high‑risk and VIP accounts from impersonation attacks
- Implement Microsoft’s email security best practices
- Pilot new security policies before full deployment
- Document configuration steps with screenshots and explanations

---

## Company Environment

| Item | Details |
|----|----|
| Number of Users | ~300 |
| Regions | United States, Western Europe |
| Email Platform | Microsoft 365 |
| Risk Focus | Phishing, spoofing, impersonation, BEC |
| Email Protection | Microsoft Defender for Office 365 |


---

## Security Features Implemented

### 1. Anti‑Phishing & Impersonation Protection
- Enabled user impersonation protection for VIP accounts
- Enabled domain impersonation protection
- Configured mailbox intelligence
- High‑confidence phishing messages are quarantined

📸 Screenshot: `screenshots/anti-phishing-vip-policy.png`

---

### 2. Preset Security Policies
- **Standard Protection** assigned to pilot users
- **Strict Protection** assigned to executives and high‑risk users

📸 Screenshot: `screenshots/preset-security-policies.png`

---

### 3. Safe Links
- Enabled URL rewriting
- Time‑of‑click malicious link detection
- Enabled for Email, Teams, and Office applications

📸 Screenshot: `screenshots/safe-links-policy.png`

---

### 4. Safe Attachments
- Enabled Safe Attachments for email
- Dynamic delivery enabled
- Malicious attachments blocked after detonation

📸 Screenshot: `screenshots/safe-attachments-policy.png`

---

## 🧪 Pilot Deployment Strategy

Before tenant‑wide deployment, security policies were tested on a **pilot group** to reduce the risk of false positives and business disruption.

### Deployment Phases
1. **Pilot Group:** IT & Security users (10–15 users)
2. **VIP Users:** CEO, CFO, and CISO protected with Strict policies
3. **Full Rollout:** All users after successful testing period

---

## 👑 VIP User Protection

High‑value accounts were given enhanced protection using:
- Strict preset policies
- Dedicated anti‑phishing policy
- Safe Links and Safe Attachments
- Mandatory multifactor authentication (MFA)

This significantly reduces the likelihood of **whaling and BEC attacks**.

---

## 📊 Mail Flow & Threat Reporting

### Reporting Tools Used
- **Threat Protection Status Report**
- **Microsoft Defender Explorer**
- Email threat trends dashboard

### Metrics Shared with Stakeholders
- Number of phishing emails detected
- Reduction in inbox‑delivered threats
- Top attack types (impersonation, malicious links)
- User‑reported phishing trends

📸 Screenshot: `screenshots/mail-flow-reports.png`

---

## 📁 Repository Structure
