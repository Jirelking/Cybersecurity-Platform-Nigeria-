
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
## Objectives

- Reduce the delivery of fraudulent and phishing emails containing malicious links to end users within Contoso.
- Implement Microsoft Defender for Office 365 Safe Links to provide real‑time, time‑of‑click URL protection against evolving phishing threats.
- Protect high‑risk and VIP users (CEO, CFO, CISO) from credential‑harvesting and business email compromise (BEC) attacks.
- Test new security controls using a pilot deployment approach before applying them organization‑wide to minimize user disruption.
- Improve visibility into email‑borne threats through monitoring, reporting, and investigation tools in Microsoft Defender.
- Demonstrate effective security control configuration by documenting policy settings and decisions with supporting screenshots.
- Align Contoso’s email security posture with Microsoft best practices for phishing prevention and user protection.
- Provide measurable security outcomes that can be communicated to technical and non‑technical stakeholders.

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

## Step‑by‑Step Guide: Implementing a Safe Links Policy in Microsoft Defender for Office 365

## Step 1: Access the Microsoft 365 Defender Portal

Configuration portal can be access on Microsoft Defender portal:
https://security.microsoft.com 
The Microsoft Defender portal is the centralized management hub for email and collaboration threat protection policies. 

<img width="1912" height="918" alt="Home" src="https://github.com/user-attachments/assets/bf5afde6-96a1-426d-8731-8d1898efabf8" />

                                       Fig 1: Microsoft 365 Defender Home Page

## Step 2: Navigate to Safe Links Policies

In the left navigation pane, select:
Email & Collaboration and follow the path to safe links

<img width="1919" height="913" alt="Name Policy" src="https://github.com/user-attachments/assets/d17a5249-419b-43e9-94e3-3889f68f92c5" />

                                       Fig 2: Safe Link Policies Page

# Navigation Path: 
Microsoft 365 Defender --> Email & Collaboration --> Policies & Rules --> Threat Policies --> Safe Links

## Step 3: Create a New Safe Links Policy

On the Safe Links page, click Create or + sign to create
Descriptive policy name:
Contoso – Safe Links Protection Policy

## Description:
Protection against phishing and malicious links.

<img width="1889" height="912" alt="1" src="https://github.com/user-attachments/assets/0aea9a09-8f36-47d9-a22b-64b20cc07e59" />

<img width="1911" height="915" alt="2" src="https://github.com/user-attachments/assets/17fecfa5-1096-45c9-a987-904c865dc8b1" />



## Step 4: Configure Safe Links Protection Settings
On the Settings page, configure the following options:

✅ Turn on Safe Links

✅ Rewrite URLs
(Ensures links are scanned when the user clicks them)

✅ Enable time‑of‑click protection

✅ Apply Safe Links to email messages

✅ Apply Safe Links to Microsoft Teams

✅ Apply Safe Links to Office desktop and web apps

❌ Do not allow users to click through malicious link warnings

<img width="1919" height="910" alt="3" src="https://github.com/user-attachments/assets/64c887cd-f46b-417f-8924-575e9ee6f5f0" />


# These settings ensure that users are blocked from accessing malicious destinations and cannot bypass Microsoft warning pages.


## Step 5: Notification

<img width="1913" height="908" alt="4" src="https://github.com/user-attachments/assets/9f7f92e7-c8d7-472b-b37b-ee6d1b4f9af4" />


## Step 6: Review and Submit the Policy

Review all configured settings and Confirm!

<img width="1894" height="911" alt="5a" src="https://github.com/user-attachments/assets/05a34781-1e0c-43ec-b7e5-d45038afb146" />


<img width="1919" height="915" alt="5b" src="https://github.com/user-attachments/assets/05154f8f-3ebf-4e60-bbf2-f803a4605d62" />

Policy Submtted

<img width="1919" height="907" alt="6" src="https://github.com/user-attachments/assets/88ad22e6-cbbe-4743-84ab-a18ee413461b" />


## Monitoring the Implementation Acticities

## Step 9: Monitor Safe Links Activity
Using Defender Explorer

<img width="1914" height="914" alt="Explore" src="https://github.com/user-attachments/assets/d3ad4e7a-3e16-4cb4-b834-c34c7631bb55" />

Navigate to:
Email & Collaboration → Explorer

Filter by:

URL click events
Phish detections


Review blocked messages and user activity

Step 10: Roll Out to All Users
After a successful pilot period (7–14 days):

Edit the Safe Links policy
Expand the scope to:
All users


Save changes

This ensures consistent protection across the organization while minimizing risk during deployment.
 ---
 
## Conclusion
The project successfully showed that implementing Microsoft Defender for Office 365 Safe Links effectively reduces phishing risk by blocking malicious URLs at the time of click. Through pilot testing and prioritizing VIP users, Contoso improved email security with minimal disruption, gained better visibility into threats, and strengthened its overall protection against credential theft and business email compromise.
