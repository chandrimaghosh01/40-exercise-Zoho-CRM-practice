---

## MODULE 8: ADVANCED — Power User Skills

---

### EXERCISE 29: Using Advanced Filters and Custom Views

**What you will learn:** How to create saved views so you can see exactly what you need with one click.

**Why this matters:** You do not have time to apply 5 filters every morning. Save your views.

**STEP-BY-STEP:**

1. Go to **Accounts**.
2. Click on the **Filters** button.
3. Apply these filters:
   - `Subscription Type` equals `Monthly`
   - `Payment Status` equals `Pending`
   - `Next Reorder Date` is `Next 7 Days`
4. Click **"Apply"**.
5. You now see only monthly subscribers with pending payment whose reorder is due in the next 7 days.
6. Click on the view name dropdown (usually says "All Accounts" or "Recently Created").
7. Select **"Create View"** or **"Save As New View"**.
8. Name: `Urgent: Monthly Reorders This Week`
9. Click **"Save"**.
10. Now this view appears in your dropdown. You can access it anytime with one click.

**PRACTICE TASK:**
- Create these saved views:
  - `Hot Prospects`: Leads with Rating = Hot and Lead Status = Contacted
  - `Overdue Payments`: Accounts with Payment Status = Overdue
  - `High Value Accounts`: Accounts with Subscription Type = Quarterly
  - `Referral Champions`: Accounts with Referral Count > 0
  - `WhatsApp Preferrers`: Accounts with Preferred Communication = WhatsApp
  - `Cat Allergies`: Accounts where Allergies field is not empty

**CHECKPOINT:** Can you create a custom view and access it from the dropdown? If yes, proceed.

---

### EXERCISE 30: Mass Updating Records

**What you will learn:** How to update many records at once instead of one by one.

**Why this matters:** If 10 subscribers all need their Payment Status changed to "Paid" after a batch payment, you do not want to open 10 records.

**STEP-BY-STEP:**

1. Go to **Accounts**.
2. Apply a filter: `Payment Status` equals `Pending`.
3. You will see a list of accounts.
4. Look for checkboxes on the left side of each row.
5. Click the checkbox in the header row (top left). This selects ALL records on the page.
6. Look for a button that says **"Mass Update"** or **"Update"** or three dots menu -> Mass Update.
7. Click it.
8. A dialog appears asking: Which field do you want to update?
9. Select `Payment Status`.
10. Select the new value: `Paid`.
11. Click **"Update"** or **"Save"**.
12. All selected accounts will have their Payment Status changed to Paid.

**PRACTICE TASK:**
- Select 5 accounts with Rating = Cold.
- Mass update their Rating to Warm.
- Verify by clicking on each account.

**CHECKPOINT:** Can you select multiple records and update one field for all of them? If yes, proceed.

---

### EXERCISE 31: Email Integration and Templates

**What you will learn:** How to send professional emails directly from Zoho CRM.

**Why this matters:** You need to send payment links, welcome emails, and reorder reminders. Doing it from CRM keeps a record.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Channels** -> **Email**.
2. Click **"Add Email Account"** or **"Configure"**.
3. Select your email provider (Gmail, Outlook, etc.).
4. Follow the steps to connect your email.
5. Once connected, go to **Setup** -> **Customization** -> **Templates** -> **Email Templates**.
6. Click **"Create Template"**.

**TEMPLATE 1: Welcome Email**
- Template Name: `Welcome New Subscriber`
- Module: `Accounts`
- Subject: `Welcome to TrueHunter, {{Account.Account Name}}!`
- Body:
```
Hi {{Account.Account Name}},

Welcome to the TrueHunter family!

Your subscription is now active. Here's what happens next:
1. We will place your first order within 24 hours.
2. You will receive a payment link via WhatsApp/email.
3. Your cat's food will arrive at your doorstep.

If you have any questions, just reply to this email or WhatsApp us.

Your cat's name: {{Account.Cat Names}}
Subscription type: {{Account.Subscription Type}}

Best regards,
TrueHunter Team
```
7. Click **"Save"**.

**TEMPLATE 2: Payment Reminder**
- Template Name: `Payment Reminder`
- Module: `Accounts`
- Subject: `Payment Reminder - TrueHunter Subscription`
- Body:
```
Hi {{Account.Account Name}},

This is a gentle reminder that your payment for this month's TrueHunter subscription is pending.

Amount due: Rs.{{Account.Amount}}
Payment link: [LINK WILL BE SENT SEPARATELY]

Please complete the payment so we can dispatch your order on time.

If you need any assistance, call us at +91-XXXXXXXXXX.

Thank you!
TrueHunter Team
```
8. Click **"Save"**.

**USING A TEMPLATE:**
1. Go to an Account (e.g., Aarav Sharma).
2. Look for an **"Email"** button or envelope icon.
3. Click it. A compose window opens.
4. Look for a dropdown or button that says **"Templates"**.
5. Select `Welcome New Subscriber`.
6. The template fills in automatically with Aarav's details.
7. Edit if needed. Click **"Send"**.
8. The email is sent AND logged in the Account's activity history.

**PRACTICE TASK:**
- Create a third template: `Reorder Confirmation` with fields for Next Reorder Date, SKU, and quantity.
- Send test emails to yourself using 3 different accounts.

**CHECKPOINT:** Can you create an email template with merge fields? Can you send an email from an Account record? If yes, proceed.

---

### EXERCISE 32: Creating Quotes and Invoices

**What you will learn:** How to generate professional quotes and invoices for subscribers.

**Why this matters:** When upselling or handling corporate orders, you need formal quotes.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Customization** -> **Modules and Fields**.
2. Make sure the **Quotes** module is enabled. If not, enable it.
3. Go to **Quotes** in the left panel.
4. Click **"Create Quote"**.
5. Fill in:
   - Quote Name: `Ananya Iyer - Quarterly Subscription Quote`
   - Account Name: `Ananya Iyer`
   - Contact Name: `Ananya Iyer`
   - Valid Until: `30/09/2026`
6. In the Product Details section, click **"Add Product"**.
7. Search for `TrueHunter Chicken Adult - 2kg`.
8. Quantity: `3` (for quarterly)
9. Click **"Save"**.
10. The system calculates the total: Rs.1,099 x 3 = Rs.3,297
11. Add another line item: `TrueHunter Dental Treats - 100g`, Quantity: `1`
12. Total becomes Rs.3,297 + Rs.199 = Rs.3,496
13. Add tax if applicable.
14. Click **"Save"**.
15. You can now **"Print"** or **"Email"** this quote.

**PRACTICE TASK:**
- Create a quote for `Neha Agarwal` for the Multi-Cat Bundle.
- Create a quote for `Vikram Reddy` for the 5kg bulk pack upsell.
- Convert one quote to an invoice.

**CHECKPOINT:** Can you create a quote with multiple products? Can you email it to a subscriber? If yes, proceed.

---

### EXERCISE 33: Zoho CRM Mobile App Basics

**What you will learn:** How to use Zoho CRM on your phone.

**Why this matters:** You are on the move. You need to check subscriber details and log calls from your phone.

**STEP-BY-STEP:**

1. On your phone, open the App Store (iPhone) or Play Store (Android).
2. Search for `Zoho CRM`.
3. Download and install the app.
4. Open the app.
5. Log in with the same email and password you used on the computer.
6. You will see a simplified version of your dashboard.
7. Tap on **Accounts**.
8. Search for `Aarav Sharma`.
9. Tap on his name. You will see his full record.
10. Scroll down to see custom fields (Number of Cats, Food Preference, etc.).
11. Tap the phone icon next to his phone number. This will call him.
12. After the call, tap **"Log Call"**.
13. Fill in:
    - Call Status: Completed
    - Duration: 5 min
    - Purpose: Reorder
    - Notes: Confirmed August reorder.
14. Tap **"Save"**.
15. The call is logged instantly and syncs with your computer.

**PRACTICE TASK:**
- Log 3 calls from your mobile app.
- Create 2 tasks from your mobile app.
- Check on your computer that the calls and tasks appear.

**CHECKPOINT:** Can you log a call from your phone and see it on your computer within 1 minute? If yes, proceed.

---

### EXERCISE 34: Data Backup and CRM Hygiene

**What you will learn:** How to export all your data and keep the CRM clean.

**Why this matters:** The JD says "keep every account record clean and current. If it isn't written down, it didn't happen."

**STEP-BY-STEP:**

1. Go to **Setup** -> **Data Administration** -> **Export**.
2. You will see options to export each module.
3. Export Accounts:
   - Select `Accounts`
   - Select `All Accounts`
   - Select `CSV` format
   - Click `Export`
   - Save the file as `TrueHunter_Accounts_Backup_[today's date].csv`
4. Export Contacts, Deals, Tasks, and Calls the same way.
5. Store these files in a `Zoho_Backups` folder on your computer.
6. Do this weekly.

**CLEANING DATA:**
1. Go to **Accounts**.
2. Filter for accounts where `Description` is empty.
3. These accounts are incomplete.
4. Open each one and add a description.
5. Go to **Leads**.
6. Filter for leads where `Email` is empty.
7. These leads cannot be contacted. Either find the email or delete them.
8. To delete: Select the lead -> Click the three dots -> Delete.

**PRACTICE TASK:**
- Export all modules as CSV files.
- Find and fix 5 incomplete records (missing phone, email, or description).
- Delete 2 test leads that are no longer needed.

**CHECKPOINT:** Do you have backup files for all modules? Have you cleaned at least 5 records? If yes, proceed.

---

### EXERCISE 35: Role-Playing a Full KAM Week in Zoho CRM

**What you will learn:** How to use ALL the skills together in a realistic scenario.

**Why this matters:** This is the final exam. If you can do this, you are ready for the TrueHunter job.

**SCENARIO: It is Monday morning, 9 AM. You are the TrueHunter KAM. Here is your week:**

**MONDAY:**
1. Open your Dashboard. Check `Tasks Due Today`.
2. You see: `Call Aarav - Confirm reorder for Aug` (High priority).
3. Call Aarav. Log the call. He confirms 1x Chicken Adult 2kg.
4. Create a task: `Send payment link to Aarav` (Due: Today).
5. Update Aarav's Account: Next Reorder Date = 10/09/2026, Payment Status = Pending.
6. You also see: `URGENT CALL - Sneha win-back attempt`.
7. Call Sneha. She does not answer. Log the call as `No Answer`.
8. Create a task: `WhatsApp Sneha with 20% discount offer` (Due: Today).
9. Send her an email using the `Payment Reminder` template (customized with discount).
10. End of day: Run the `Active Subscribers Overview` report. Email it to your manager.

**TUESDAY:**
1. Check Dashboard. Payment Status pie chart shows 3 overdue accounts.
2. Call all 3 overdue accounts. Log each call.
3. For those who pay, update Payment Status to Paid.
4. For those who need time, update Payment Status to Pending and set a follow-up task.
5. Create upsell deals for 5 subscribers who are ready for larger packs or treats.

**WEDNESDAY:**
1. A new lead comes in from Instagram: `Riya Kapoor`, riya.k@email.com, 1 cat, interested in monthly plan.
2. Create the lead in Zoho CRM.
3. The assignment rule automatically assigns it to you.
4. Call Riya within 30 minutes (TrueHunter promise).
5. Log the call. She is interested. Move her lead status to `Contacted`.
6. Schedule a follow-up call for Friday.

**THURSDAY:**
1. Check your `Urgent: Monthly Reorders This Week` view.
2. 8 subscribers need reorder confirmation this week.
3. Call 4 of them. Log calls. Update Next Reorder Dates.
4. Send payment links to those who confirmed.
5. Update Payment Status to Pending.

**FRIDAY:**
1. Follow-up call with Riya Kapoor.
2. She agrees to subscribe! Convert her lead to Account + Contact + Deal.
3. Use the Blueprint to move her deal through `Welcome Call Scheduled`.
4. Create a welcome task.
5. Send her the `Welcome New Subscriber` email template.
6. End of week: Review your Dashboard.
   - How many new subscriptions this week?
   - How many reorders processed?
   - How many at-risk accounts saved?
   - How much revenue generated?
7. Export a backup of all data.

**PRACTICE TASK:**
- Actually perform every step above in your Zoho CRM trial.
- Do not skip any step.
- At the end, take a screenshot of your Dashboard (for your own reference).

**CHECKPOINT:** Can you complete all 5 days of tasks without getting stuck? Can you explain each action you took? If yes, YOU ARE READY.
