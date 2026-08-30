---

## MODULE 9: BONUS EXERCISES — Expert Level

---

### EXERCISE 36: Creating a Web Form for Lead Capture

**What you will learn:** How to create a form that cat parents can fill on your website.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Developer Space** -> **Webforms**.
2. Click **"Create Webform"**.
3. Module: `Leads`
4. Layout: `Standard`
5. Drag and drop these fields into the form:
   - First Name (required)
   - Last Name (required)
   - Email (required)
   - Phone (required)
   - Company
   - Lead Source (set default to `Website`)
   - Description (label it: "Tell us about your cat")
6. Click on the form title. Change it to: `Join TrueHunter - Subscribe for Your Cat`
7. Click **"Generate Embed Code"**.
8. Zoho gives you HTML code. Copy it.
9. In a real scenario, your developer would paste this into the TrueHunter website.
10. For practice, click **"Preview"** and fill out the form.
11. Submit it.
12. Go to Leads. You should see the new lead automatically created.

---

### EXERCISE 37: Zoho CRM Integration with WhatsApp (Conceptual)

**What you will learn:** How Zoho connects with WhatsApp for business.

**NOTE:** WhatsApp Business API requires Meta approval. This is a conceptual exercise.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Marketplace**.
2. Search for `WhatsApp`.
3. You will see integrations like `WhatsApp for Business by Zoho` or third-party apps.
4. Click on one to read the description.
5. In a real setup:
   - You would connect your WhatsApp Business account.
   - Incoming WhatsApp messages would appear in Zoho CRM.
   - You could reply from Zoho CRM.
   - All chats would be saved under the contact's record.
6. For practice: Create a custom field on Contacts called `WhatsApp Number`.
7. Fill it in for 10 subscribers.
8. Create a task template: `Send WhatsApp reminder to [Name]`.

---

### EXERCISE 38: Creating a Churn Prediction Score

**What you will learn:** How to use formula fields to calculate risk scores.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Customization** -> **Accounts** -> **New Field**.
2. Field Type: `Formula`
3. Label: `Churn Risk Score`
4. Formula:
   - This is advanced. For simplicity, create a Pick List instead:
   - Label: `Churn Risk`
   - Options: `Low`, `Medium`, `High`, `Critical`
5. Manually set the risk for each account based on:
   - High = Skipped cycle + Overdue payment + Cold rating
   - Medium = One of the above
   - Low = None of the above
6. Create a report: `Churn Risk Analysis` grouped by Churn Risk.

---

### EXERCISE 39: Territory Management (For Future Growth)

**What you will learn:** How to divide Bengaluru into delivery zones.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Users and Control** -> **Territories**.
2. Click **"Create Territory"**.
3. Create territories:
   - `North Bengaluru`
   - `South Bengaluru`
   - `East Bengaluru`
   - `West Bengaluru`
   - `Central Bengaluru`
4. Assign accounts to territories based on their pincode:
   - 560001-560020: Central
   - 560021-560050: South
   - 560051-560080: North
   - 560081-560110: East
   - 560111-560140: West
5. Create a report showing accounts by territory.

---

### EXERCISE 40: Creating a Year-End Review Report

**What you will learn:** How to compile everything for management review.

**STEP-BY-STEP:**

1. Create a folder in Reports called `Year-End Review`.
2. Create these reports inside it:
   - `Total Subscribers Gained`: Count of Accounts created this year
   - `Total Revenue`: Sum of Deal Amounts (Closed Won)
   - `Churn Rate`: (Closed Lost Deals / Total Deals) x 100
   - `Average Subscription Value`: Average Deal Amount
   - `Top 5 Referrers`: Accounts sorted by Referral Count
   - `Best Lead Source`: Lead Source with most Closed Won deals
3. Create a dashboard called `Year-End Dashboard`.
4. Add all reports as components.
5. Schedule the dashboard to email to your manager every Monday at 9 AM.

---
