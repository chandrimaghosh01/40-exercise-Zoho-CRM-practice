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

## FINAL CHECKLIST

Before you apply for the TrueHunter KAM role, make sure you can do ALL of the following WITHOUT help:

- [ ] Log in to Zoho CRM in under 60 seconds
- [ ] Import data from CSV files
- [ ] Create and edit Leads, Accounts, Contacts, and Deals
- [ ] Convert a Lead to a subscriber
- [ ] Create custom fields and modules
- [ ] Log calls and tasks
- [ ] Send emails using templates
- [ ] Create workflow rules that run automatically
- [ ] Build reports and dashboards
- [ ] Filter and search records quickly
- [ ] Update records in bulk
- [ ] Use the mobile app
- [ ] Export data for backup
- [ ] Explain what each module is for
- [ ] Complete the "Full KAM Week" exercise without getting stuck

**If you can check all 15 boxes, you are ready for the interview.**

---

## QUICK REFERENCE: Zoho CRM Shortcuts

| Action | How to Do It |
|--------|-------------|
| Create new record | Click the + icon or colored button |
| Search | Use the magnifying glass at the top |
| Edit record | Open record -> Click pencil icon |
| Delete record | Open record -> Three dots -> Delete |
| Import data | Module page -> Import button |
| Export data | Module page -> Three dots -> Export |
| Mass update | Select records -> Mass Update button |
| Create task | Account page -> Add Task |
| Log call | Account page -> Log Call |
| Send email | Account page -> Email button |
| Run report | Reports -> Click report name |
| View dashboard | Dashboards -> Select dashboard |
| Go to Setup | Click gear icon (top right) |
| Get help | Click ? icon (top right) |

---

## TROUBLESHOOTING COMMON PROBLEMS

**Problem: I cannot find the Import button.**
- Solution: Make sure you are on the list view (showing multiple records), not the detail view (showing one record). Click the module name in the left panel to go to list view.

**Problem: My imported data shows in the wrong columns.**
- Solution: During import, carefully match each CSV column to the correct Zoho field. If wrong, delete the imported records and import again.

**Problem: Custom fields do not appear.**
- Solution: Go to Setup -> Customization -> [Module] -> Layouts. Make sure the fields are in the layout assigned to your profile.

**Problem: Workflow did not trigger.**
- Solution: Check if the workflow is Active (not Draft). Go to Setup -> Automation -> Workflow Rules. Make sure the rule status is "Active."

**Problem: I deleted something by mistake.**
- Solution: Go to Setup -> Data Administration -> Recycle Bin. You can restore deleted records within 60 days.

**Problem: Dashboard shows old data.**
- Solution: Click the refresh icon on the dashboard. Dashboards do not auto-refresh in real-time.

---

## GLOSSARY OF TERMS

| Term | Meaning |
|------|---------|
| **Lead** | A person who showed interest but is not yet a customer |
| **Account** | A company or family unit (in TrueHunter, each subscriber is an Account) |
| **Contact** | A person you can contact (the cat parent) |
| **Deal** | A sales opportunity (a subscription) |
| **Task** | Something you need to do (call, email, send payment link) |
| **Call** | A logged phone conversation |
| **Pipeline** | Visual stages showing where a deal is in the sales process |
| **Stage** | A step in the pipeline (e.g., New Enquiry, Closed Won) |
| **Workflow** | An automatic action triggered by an event |
| **Blueprint** | A guided step-by-step process |
| **Module** | A section of CRM (Leads, Accounts, Deals, etc.) |
| **Field** | A piece of information (Name, Phone, Email, etc.) |
| **Custom Field** | A field you created (not built into Zoho) |
| **Custom Module** | A new section you created (like Cat Profiles) |
| **Filter** | A way to show only certain records |
| **View** | A saved set of filters |
| **Report** | A summary of data in table or chart form |
| **Dashboard** | A screen with multiple charts and numbers |
| **Import** | Bringing data into Zoho from a file |
| **Export** | Saving Zoho data to a file |
| **CRM Hygiene** | Keeping data clean, complete, and up-to-date |

---
