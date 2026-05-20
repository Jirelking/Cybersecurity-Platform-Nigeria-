## 🧪 Lab Implementation Guide: Microsoft Purview for Finance Data Protection

### ✅ Step 1: Access Microsoft Purview Portal
- Navigate to: https://compliance.microsoft.com
- Log in with admin credentials

📸 Screenshot 1: Purview Dashboard Homepage

---

### ✅ Step 2: Create Custom Sensitive Information Type (SIT)

1. Go to **Data Classification → Sensitive Info Types**
2. Click **+ Create Sensitive Info Type**
3. Enter:
   - Name: "Finance Sensitive Data"
4. Configure detection:
   - Add patterns (Regex for BVN, Bank Account Number)
   - Add keywords (e.g., "BVN", "Account Number")

5. Save and test using sample data file

📸 Screenshot 2: Custom SIT Creation Page  
📸 Screenshot 3: SIT Pattern Configuration  
📸 Screenshot 4: SIT Testing Results  

---

### ✅ Step 3: Create Sensitivity Label

1. Navigate to **Information Protection → Labels**
2. Click **+ Create Label**
3. Name: "Confidential – Finance Only"
4. Configure:
   - Encryption: Enable
   - Access: Finance Department only
   - Content marking (optional)

5. Publish label

📸 Screenshot 5: Label Configuration  
📸 Screenshot 6: Label Publishing Policy  

---

### ✅ Step 4: Configure Auto-Labeling Policy

1. Go to **Information Protection → Auto-labeling**
2. Create a new policy
3. Select:
   - Your custom SIT
   - Apply label automatically

📸 Screenshot 7: Auto-Label Policy Setup  

---

### ✅ Step 5: Create DLP Policy

1. Go to **Data Loss Prevention → Policies**
2. Click **Create Policy**
3. Choose:
   - Custom policy
4. Configure:
   - Condition: Detect SIT
   - Action:
     - Block external email sharing
     - Restrict file sharing

📸 Screenshot 8: DLP Policy Configuration  
📸 Screenshot 9: Block Email Rule  

---

### ✅ Step 6: Configure Copilot Restrictions

1. Go to **Data Security Settings**
2. Apply policies to:
   - Restrict Copilot access to labeled data
3. Ensure:
   - Sensitive data cannot be processed by AI tools

📸 Screenshot 10: Copilot Data Protection Settings  

---

### ✅ Step 7: Testing & Validation

- Send test email with BVN → should be blocked ✅  
- Upload file → should be auto-labeled ✅  
- Test Copilot prompt → restricted ✅  

📸 Screenshot 11: Test Result Evidence  
