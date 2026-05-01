
# Mitigating Fraudulent Emails at Contoso  
**Focus Area: Microsoft Defender for Office 365 – Safe Links**

---

## Author
**Name:** Solomon Ajireloja  
**Role:** Security Analyst  
**Case Study Organization:** Contoso  

---

## Executive Summary

Contoso is a mid-sized organization with approximately 300 users located across the United States and Western Europe. The organization has experienced an increase in fraudulent and phishing emails successfully reaching end users’ mailboxes. These emails pose a serious risk, including credential theft, business email compromise (BEC), and potential financial loss.

This project documents the assessment, design, and implementation of a security solution using **Microsoft Defender for Office 365**, with a primary focus on **Safe Links**, a feature that protects users from malicious URLs through real-time, time-of-click inspection.

---

## Organization Overview

| Category | Details |
|--------|--------|
| User Count | ~300 users |
| Locations | United States, Western Europe |
| Email Platform | Microsoft 365 |
| Primary Risk | Phishing emails with malicious links |
| High-Risk Users | CEO, CFO, CISO |

---

## Problem Statement

Contoso’s existing email security controls were insufficient to prevent phishing emails containing malicious URLs from being delivered to users. Many modern phishing attacks rely on links that appear legitimate at delivery but later redirect users to credential-harvesting or malware-hosting websites.

Because of this, the organization required a solution that could identify and block malicious links **at the time a user clicks them**, rather than only during mail delivery.

---

## Licensing Recommendation

**Recommended License:**
- Microsoft Defender for Office 365 Plan 2 (Add-on)  
  **OR**
- Microsoft 365 E5

**Justification:**
Defender for Office 365 Plan 2 provides advanced phishing protection features such as Safe Links, Safe Attachments, impersonation protection, and enhanced reporting capabilities not available in basic Exchange Online Protection.

---

## Why Safe Links Was Selected

Safe Links was selected as the primary control because:
- Most phishing attacks rely on malicious URLs
- URLs can become malicious after email delivery
- Executives are common targets of credential-harvesting attacks
- Safe Links provides real-time, time-of-click protection

Safe Links inspects URLs dynamically when users attempt to access them, blocking access to malicious destinations even if the link was previously considered safe.

---

## Safe Links Overview

Safe Links provides:
- URL rewriting during mail flow
- Time-of-click URL inspection
- Protection across Email, Microsoft Teams, and Office apps
- Microsoft warning pages for blocked links

This ensures continuous protection against evolving phishing threats.

---

## Safe Links Policy Configuration

**Portal Used:**  
https://security.microsoft.com

### Navigation Path
``
