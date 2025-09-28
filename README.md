# Travelport-Admin-Portal-Indigo-Integration-Update

## Steps to Update Indigo Credentials in Travelport

### 1. Login
- Access the **Travelport Admin Portal** with your credentials.  

### 2. Change Context to Desired PCC
- On the website, scroll to the middle of the page.  
- Navigate to:  
Change Context → Browse Branches

markdown
Copy code
- Select the **desired PCC**.  
- You are now working under the correct PCC.  

### 3. Navigate to Travelport Credentials
- Go to:  
Providers → Travelport Credentials

markdown
Copy code
- Select the appropriate **Profile**.  
- In **Profile Type**, click the dropdown and select **Branch**.  
- In the next dropdown, select the **Provider PCC/SID**.  
- In the next box, enter the **PCC details**.  

### 4. Travelport Credential Management
- You will reach:  
Travelport Credential Management (Display Providers for: <PCC>-1G)

markdown
Copy code
- Select the required **Profile**.  

### 5. Edit Indigo Credentials
- Locate the **Indigo provider entry**.  
- Click **Edit** (next to Indigo).  
- Update the **Indigo credentials** as required.  

---

## ✅ Outcome
- Indigo integration will be updated successfully.  
- Indigo flights will now display in the **UAPI LowFareSearch response**.
