# Use Case 2: Protecting Finance Department Data and Information from Unauthorized Access and Data Breaches
## Microsoft Solution: Microsoft 365 Purview ( Under "Information Protection" & "DLP")  

## Author
**Analyst Name:** Solomon Idowu, Ajireloja  
**Program:** Platform Explorers – Cybersecurity  
**Date:** 15th of May, 2026 


##  Overview
This use case outlines how an organization can implement **Microsoft Purview Sensitivity Labels and Data Loss Prevention (DLP)** to protect sensitive financial data within the finance department.

The primary objective is to:
- Automatically classify and label sensitive financial information  
- Prevent unauthorized sharing of financial data  
- Restrict the use of sensitive data with AI tools such as **Microsoft 365 Copilot**  

---

##  Detailed Use Case

The Finance Department processes highly confidential information, including:
- Personal Identifiable Information (PII)  
- Financial records  
- Corporate financial data and intellectual property  

This data is critical to the organization and must be protected from:
- Unauthorized internal access  
- External data leaks  
- Accidental sharing via email or collaboration tools  
- Exposure through AI tools like Microsoft 365 Copilot  

To mitigate these risks, the organization will implement **Microsoft Purview Information Protection and DLP policies**.

---

##  Requirements & Implementation

### Sensitive Information Type (SIT)

Create custom Sensitive Information Types (SITs) to detect financial data patterns.

#### Examples:
- Croatian Bank Account Number  
- Nigerian Bank Verification Number (BVN)  

## Step‑by‑Step Implementation Guide: Microsoft Purview for Finance Data and Information Protection

###  Step 1: Access Microsoft Purview Portal
- Navigate to: https://compliance.microsoft.com
- Log in with admin credentials
<img width="1912" height="915" alt="Login Page" src="https://github.com/user-attachments/assets/132fa142-b435-4ce0-96fe-2dfc4c677c1a" />

---

###  Step 2: Create Custom Sensitive Information Type (SIT)

1. Navigate as follows:  **Data Classification → Sensitive Info Types**
2. <img width="1917" height="904" alt="SIT Portal" src="https://github.com/user-attachments/assets/2638fbc2-48bb-4924-8c0c-91587894714c" />

3. Click **+ Create Sensitive Info Type**
4.  <img width="1914" height="916" alt="SIT Name Decription" src="https://github.com/user-attachments/assets/c6bbf38b-5d8c-4f1d-b99b-fd21da2a1981" />

5. Enter The Name: "Finance Sensitive Data"
6. Configure detection:  - Add patterns 1  & Add keywords
<img width="1916" height="906" alt="Pattern 1" src="https://github.com/user-attachments/assets/07d59590-31cb-4418-ae31-876e0c3fbd13" />

7. 
8. Configure detection:  - Add patterns 2  & Add keywords 
<img width="1910" height="908" alt="Pattern 2" src="https://github.com/user-attachments/assets/d38c44b7-da01-4f25-ab0f-937221260fb0" />

<img width="1913" height="905" alt="Pattern" src="https://github.com/user-attachments/assets/1f4875bb-e625-4f7e-97d4-58bf4ff270d9" />

Recommended C
<img width="1919" height="925" alt="Recommend Page" src="https://github.com/user-attachments/assets/f0700c00-0b4b-46bf-ada6-84b48a8b4141" />

SIT Successfully Created
<img width="1912" height="918" alt="SIT Cretaed Successfully" src="https://github.com/user-attachments/assets/270b62f6-b11f-41a6-b6cb-7be46e793238" />

 Screenshot 4: SIT Testing Results  

<img width="1919" height="916" alt="Upload TestFile" src="https://github.com/user-attachments/assets/0d32315f-4aaa-4e22-9577-8e1aa1a601d3" />

<img width="1914" height="915" alt="BVN Match result" src="https://github.com/user-attachments/assets/4464e733-24d9-4fa9-8a6a-454dabccb5e5" />

<img width="1894" height="864" alt="Croatian Match Result" src="https://github.com/user-attachments/assets/f05e2edf-97a6-4f08-bc2d-522625383ab8" />
---

###  Step 3: Create Sensitivity Label

1. Navigate to **Information Protection → Labels**
2. Click **+ Create Label**
<img width="1908" height="902" alt="Label portal" src="https://github.com/user-attachments/assets/5b8911cd-319b-4f46-9870-d53b0083b0c3" />

4. Name: "Confidential – Finance Only"
5. Configure:
   - Encryption: Enable
   - Access: Finance Department only
   - Content marking (optional)
<img width="1919" height="907" alt="Label Details" src="https://github.com/user-attachments/assets/ddbc946d-2d74-4485-98e8-c4464fab85cb" />
<img width="1918" height="916" alt="Label Scope" src="https://github.com/user-attachments/assets/4ec2d197-c93c-4a28-99ed-11cd9d85a706" />
Label Configuration
<img width="1919" height="846" alt="Label Items2" src="https://github.com/user-attachments/assets/ad8c6342-df44-4cbf-b25f-a44fe8177be0" />
<img width="1919" height="914" alt="Label Content Marking" src="https://github.com/user-attachments/assets/196a2e37-72ee-460a-af5b-e76e45334316" />

 Publish label
<img width="1917" height="918" alt="Sensitivity label created" src="https://github.com/user-attachments/assets/458d6b1e-7b9b-4437-8467-3757dfae81d4" />

---

###  Step 4: Configure Auto-Labeling Policy

1. Go to **Information Protection → Auto-labeling**
2. Create a new policy
<img width="1891" height="760" alt="Auto Label Policy" src="https://github.com/user-attachments/assets/9efd804d-cd41-4438-93f8-bf78ead4e43b" />

4. Select:
   - Your custom SIT
   - Apply label automatically

 Screenshot 7: Auto-Label Policy Setup  
<img width="1902" height="913" alt="Auto Apply policy" src="https://github.com/user-attachments/assets/b5d37002-7779-48d9-aeb2-dbf73fcf7be6" />

Selected Label
<img width="1919" height="916" alt="Auto Label Policy 1" src="https://github.com/user-attachments/assets/d5f2d517-1abe-4938-b6a3-8a2e0ddec6da" />

Label to Auto Apply
<img width="1919" height="910" alt="Auto LAbel" src="https://github.com/user-attachments/assets/b8d7bc6c-2de3-427a-afbb-40d406ce8310" />

New Rules Configuration
<img width="1918" height="916" alt="Auto  apply configured" src="https://github.com/user-attachments/assets/1989e0c9-d054-46b6-b889-fb9ca078117f" />

Rules Definition
<img width="1919" height="902" alt="rules" src="https://github.com/user-attachments/assets/b5bf871a-d3fa-4109-84d9-e52d39d13642" />

Auto Labelling Review
<img width="1919" height="901" alt="Auto Label Review" src="https://github.com/user-attachments/assets/6ddf941f-ec79-4d3d-b65e-666bc04575fa" />

Auto Labelling Policy Created
<img width="1919" height="916" alt="Auto labelling policy created" src="https://github.com/user-attachments/assets/262f8e75-34af-4847-9710-f7b618fe3fc2" />

---

###  Step 5: Create DLP Policy

1. Go to **Data Loss Prevention → Policies**
2. Click **Create Policy**
3. Choose:
   - Custom policy
4. Configure:
   - Condition: Detect SIT
   - Action:
     - Block external email sharing
     - Restrict file sharing

Screenshot 8: DLP Policy Configuration  
Screenshot 9: Block Email Rule  

---

### Step 6: Configure Copilot Restrictions

1. Go to **Data Security Settings**
2. Apply policies to:
   - Restrict Copilot access to labeled data
3. Ensure:
   - Sensitive data cannot be processed by AI tools

 Screenshot 10: Copilot Data Protection Settings  

---

### Step 7: Testing & Validation

- Send test email with BVN → should be blocked   
- Upload file → should be auto-labeled   
- Test Copilot prompt → restricted   

Screenshot 11: Test Result Evidence  
