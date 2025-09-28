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




- ---

## ✅# GWS Sign-On Creation Procedure

This guide explains how to create a GWS sign-on for agents, including multi-terminal access and alternate paths.

---

## Step 1: Standard GWS Sign-On

- **Command / Format:**  
STD/Z<PCC>/GWS

markdown
Copy code
Example: `STD/Z86W2/GWS`  
*Basic sign-on using your PCC.*

- **Name:** `GWS SIGNON`  
*User-defined name for the sign-on session.*

- **Password:** `LONDON 99`  
*Use your authorized GWS password.*

- **Duty Code:** `AG`  
*AG = Agent duty code.*

- **Multi Terminal:** `Y`  
*Set to 'Y' to enable multiple terminal access.*

---

## Step 2: Alternate Sign-On

- **Command / Format:**  
STD/z62/GWS/**

yaml
Copy code
*Used in specific scenarios like profile resets.*

- **Additional Line:** `RBTC.N.Y`  
*Resets buffer or clears cached sessions.*

---

## Step 3: Additional GWS Sign-On Variation

- **Command / Format:**  
STD/Z62/GWS

yaml
Copy code

- **Password Bypass:** `Y`  
*Press Enter after entering to bypass password.*

---

## Step 4: Multi-Terminal Override

- **Value:** `U`  
*Indicates an issue with Multi Terminal.*

- **Action:**  
*Raise a Bizagi ticket if 'U' appears.*

---

## Notes

- Verify your PCC before signing on.  
- Multi-terminal access should be used only when required.  
- Alternate sign-on paths are for special cases like profile resets.  
- Keep session names and passwords secure.  

  
