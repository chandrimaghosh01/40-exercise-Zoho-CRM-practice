---

## MODULE 2: DATA IMPORT — Bringing TrueHunt Data into Zoho CRM

---

### EXERCISE 4: Importing Leads (Your First Data Import)

**What you will learn:** How to bring a list of potential cat parents into Zoho CRM from a file.

**Why this matters:** TrueHunt gets leads from Instagram, WhatsApp, and referrals. You need to load them all into the system.

**PREPARATION:**
- Download the file: `01_Leads_Import_Data.csv`
- Save it to your Desktop in a folder called `TrueHunt_Zoho_Practice`

**STEP-BY-STEP:**

1. Open Zoho CRM and click on **Leads** in the left panel.
2. Look for a button that says **"Import"** or has an upward arrow icon. It is usually near the top right, next to the Create button.
3. Click **"Import"**.
4. A new screen appears. Select **"Leads"** as the module if it asks.
5. Click **"Browse"** or **"Choose File"**.
6. Navigate to your Desktop. Open the `TrueHunt_Zoho_Practice` folder.
7. Select the file named `01_Leads_Import_Data.csv`. Click **"Open"**.
8. Zoho will show you a preview of the data. You will see columns like First Name, Last Name, Email, Phone, etc.
9. Zoho will try to match the columns automatically. Check each column:
   - The column `First Name` in your file should map to `First Name` in Zoho
   - The column `Last Name` should map to `Last Name`
   - The column `Email` should map to `Email`
   - The column `Phone` should map to `Phone`
   - The column `Company` should map to `Company`
   - The column `Lead Source` should map to `Lead Source`
   - The column `Lead Status` should map to `Lead Status`
   - The column `Description` should map to `Description`
10. If any column is NOT matched correctly, click on the dropdown next to that column and select the correct Zoho field name.
11. When all columns are matched, click **"Next"**.
12. Zoho will ask about duplicate handling. Select: **"Skip"** (this means if a lead already exists, do not import it again).
13. Click **"Import"**.
14. Wait for the import to finish. You will see a message like "30 records imported successfully."
15. Click **"Done"** or **"Finish"**.
16. You will now see the Leads list with 30 names. Scroll through them.

**PRACTICE TASK:**
- Click on the first lead (Aarav Sharma). Look at all the details.
- Click the **"Back"** button in your browser to return to the list.
- Use the search bar at the top to search for "Priya". See how it filters the list.

**CHECKPOINT:** Do you see 30 leads in the Leads module? Can you search and find "Sneha Nair"? If yes, proceed.

---

### EXERCISE 5: Importing Accounts (Subscriber Families)

**What you will learn:** How to import existing subscribers as Accounts.

**Why this matters:** In TrueHunt, each subscriber is an Account. You need all 30 subscribers in the system.

**PREPARATION:**
- Download the file: `02_Accounts_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on **Accounts** in the left panel.
2. Click the **"Import"** button at the top right.
3. Select **"Accounts"** as the module.
4. Click **"Browse"** and select `02_Accounts_Import_Data.csv`.
5. Click **"Next"**.
6. Match the columns:
   - `Account Name` -> `Account Name`
   - `Account Number` -> `Account Number`
   - `Phone` -> `Phone`
   - `Account Type` -> `Account Type`
   - `Industry` -> `Industry`
   - `Rating` -> `Rating`
   - `Billing Street` -> `Billing Street`
   - `Billing City` -> `Billing City`
   - `Billing State` -> `Billing State`
   - `Billing Code` -> `Billing Code`
   - `Billing Country` -> `Billing Country`
   - `Description` -> `Description`
7. Click **"Next"**.
8. Select **"Skip"** for duplicates.
9. Click **"Import"**.
10. Wait for the confirmation message.
11. You should see 30 accounts.

**PRACTICE TASK:**
- Click on the account "Sneha Nair". Read the Description field. Notice it says "AT-RISK."
- Click on "Ananya Iyer". Notice it says "High value account" with 3 cats.
- Go back to the Accounts list. Look at the **Rating** column. You should see Hot, Warm, and Cold ratings.

**CHECKPOINT:** Can you see 30 accounts with ratings (Hot/Warm/Cold)? If yes, proceed.

---

### EXERCISE 6: Importing Contacts (Cat Parents)

**What you will learn:** How to import the people (contacts) linked to each account.

**Why this matters:** The Account is the "family." The Contact is the "person." You call the person, but you manage the family account.

**PREPARATION:**
- Download the file: `03_Contacts_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on **Contacts** in the left panel.
2. Click the **"Import"** button.
3. Select **"Contacts"** as the module.
4. Browse and select `03_Contacts_Import_Data.csv`.
5. Click **"Next"**.
6. Match the columns carefully:
   - `First Name` -> `First Name`
   - `Last Name` -> `Last Name`
   - `Account Name` -> `Account Name` (This is very important — it links the contact to the account)
   - `Email` -> `Email`
   - `Phone` -> `Phone`
   - `Mobile` -> `Mobile`
   - `Title` -> `Title`
   - `Lead Source` -> `Lead Source`
   - `Mailing Street` -> `Mailing Street`
   - `Mailing City` -> `Mailing City`
   - `Mailing State` -> `Mailing State`
   - `Mailing Zip` -> `Mailing Zip`
   - `Mailing Country` -> `Mailing Country`
7. Click **"Next"**.
8. Select **"Skip"** for duplicates.
9. Click **"Import"**.
10. Wait for the message: "30 records imported."

**PRACTICE TASK:**
- Click on Contact "Aarav Sharma".
- Look at the right side panel. You should see a section called **"Related Records"** or **"Account Name"** showing "Aarav Sharma" (the account).
- Click on that Account Name link. It should take you to the Account record.
- This is the magic of CRM — everything is connected.

**CHECKPOINT:** Can you click on a Contact and see their linked Account? Can you navigate back? If yes, proceed.

---

### EXERCISE 7: Importing Deals (Subscriptions)

**What you will learn:** How to import subscription records as Deals.

**Why this matters:** In Zoho CRM, a "Deal" represents a sales opportunity. For TrueHunt, each Deal is a subscription.

**PREPARATION:**
- Download the file: `04_Deals_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on **Deals** in the left panel.
2. Click the **"Import"** button.
3. Select **"Deals"** as the module.
4. Browse and select `04_Deals_Import_Data.csv`.
5. Click **"Next"**.
6. Match the columns:
   - `Deal Name` -> `Deal Name`
   - `Account Name` -> `Account Name`
   - `Contact Name` -> `Contact Name`
   - `Amount` -> `Amount`
   - `Closing Date` -> `Closing Date`
   - `Stage` -> `Stage`
   - `Type` -> `Type`
   - `Lead Source` -> `Lead Source`
   - `Next Step` -> `Next Step`
   - `Probability` -> `Probability`
   - `Expected Revenue` -> `Expected Revenue`
   - `Description` -> `Description`
7. Click **"Next"**.
8. For duplicates, select **"Skip"**.
9. Click **"Import"**.
10. Wait for confirmation.

**PRACTICE TASK:**
- Click on Deal "Aarav Sharma - Monthly Subscription".
- Notice the Amount is Rs.2,499. The Stage is "Closed Won."
- Look at the "Next Step" field. It says "Reorder due Aug 15."
- Scroll down to see the Description. It tells you the cat's food preference.

**CHECKPOINT:** Can you see 30 deals, all in "Closed Won" stage? Can you read the Next Step for any deal? If yes, proceed.

---

### EXERCISE 8: Importing Products (Cat Food SKUs)

**What you will learn:** How to import your product catalog.

**Why this matters:** TrueHunt sells specific SKUs. You need these in the system to create quotes and track what each subscriber buys.

**PREPARATION:**
- Download the file: `05_Products_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on the **Products** icon in the left panel. (If you do not see it, click the three dots at the bottom of the left panel to see more modules.)
2. Click the **"Import"** button.
3. Select **"Products"** as the module.
4. Browse and select `05_Products_Import_Data.csv`.
5. Click **"Next"**.
6. Match the columns:
   - `Product Name` -> `Product Name`
   - `Product Code` -> `Product Code`
   - `Product Active` -> `Product Active`
   - `Product Category` -> `Product Category`
   - `Unit Price` -> `Unit Price`
   - `Tax` -> `Tax`
   - `Description` -> `Description`
7. Click **"Next"**.
8. Select **"Skip"** for duplicates.
9. Click **"Import"**.
10. You should see 20 products.

**PRACTICE TASK:**
- Find the product "TrueHunt Chicken Adult - 2kg". Note the Product Code: `TH-CA-2KG` and price: Rs.1,099.
- Find "TrueHunt Dental Treats - 100g". Note the price: Rs.199.
- These are the products you will upsell in later exercises.

**CHECKPOINT:** Can you see 20 products with correct prices? If yes, proceed.

---

### EXERCISE 9: Importing Tasks (Your To-Do List)

**What you will learn:** How to import a list of follow-up tasks.

**Why this matters:** As a KAM, you have 100+ moving parts. Tasks keep you organized.

**PREPARATION:**
- Download the file: `06_Tasks_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on **Activities** in the left panel.
2. Make sure you are on the **Tasks** tab.
3. Look for an **"Import"** option. In some Zoho versions, you may need to click the three dots (More Actions) menu at the top right of the Tasks list.
4. If Import is not visible, do this manually for practice:
   - Click **"Create Task"** (plus icon or colored button).
   - For each row in the CSV, create one task.
   - This manual practice is actually very good for learning.
5. If Import is available, select `06_Tasks_Import_Data.csv`.
6. Match columns:
   - `Subject` -> `Subject`
   - `Related To` -> `Related To` (This links the task to an Account)
   - `Due Date` -> `Due Date`
   - `Status` -> `Status`
   - `Priority` -> `Priority`
   - `Description` -> `Description`
7. Click **"Import"**.

**ALTERNATIVE (Recommended for beginners):** Since task import can be tricky, create 5 tasks manually:
1. Click **"Create Task"**.
2. Subject: `Call Aarav - Confirm reorder for Aug`
3. Related To: Select Account `Aarav Sharma`
4. Due Date: `10/08/2026`
5. Priority: `High`
6. Description: `Call to confirm August reorder. Send payment link after confirmation.`
7. Click **"Save"**.
8. Repeat for the next 4 tasks.

**PRACTICE TASK:**
- Look at your Tasks list. Sort by Priority. The High priority tasks should appear at the top.
- Click on a High priority task. Notice the red color or exclamation mark.

**CHECKPOINT:** Can you see tasks in your Activities module? Can you sort by Priority? If yes, proceed.

---

### EXERCISE 10: Importing Calls (Communication History)

**What you will learn:** How to import past call records.

**Why this matters:** TrueHunt promises fast replies and personal service. You must log every call.

**PREPARATION:**
- Download the file: `07_Calls_Import_Data.csv`

**STEP-BY-STEP:**

1. Click on **Activities** in the left panel.
2. Click on the **Calls** tab.
3. Calls are usually imported or logged manually. For this exercise, we will log 3 calls manually to understand the process:

**CALL 1 — Aarav Sharma:**
1. Click **"Log Call"** or **"Create Call"** (plus icon).
2. Call To: Search for and select `Aarav Sharma`
3. Related To: Select Account `Aarav Sharma`
4. Call Type: `Outgoing`
5. Outgoing Call Status: `Completed`
6. Call Start Time: `01/08/2026 10:30`
7. Call Duration: `5 min`
8. Subject: `August reorder confirmation`
9. Call Purpose: `Reorder`
10. Description: `Confirmed reorder for 1x Chicken Adult 2kg. Payment link sent. Expected delivery Aug 5.`
11. Click **"Save"**.

**CALL 2 — Sneha Nair (No Answer):**
1. Click **"Log Call"**.
2. Call To: `Sneha Nair`
3. Related To: Account `Sneha Nair`
4. Call Type: `Outgoing`
5. Outgoing Call Status: `No Answer`
6. Call Start Time: `01/08/2026 15:30`
7. Call Duration: `0 min`
8. Subject: `Win-back attempt - no answer`
9. Call Purpose: `Retention`
10. Description: `Called twice, no answer. Left WhatsApp message with offer.`
11. Click **"Save"**.

**CALL 3 — Rohan Bhat (Saved Account):**
1. Click **"Log Call"**.
2. Call To: `Rohan Bhat`
3. Related To: Account `Rohan Bhat`
4. Call Type: `Outgoing`
5. Outgoing Call Status: `Completed`
6. Call Start Time: `04/08/2026 14:30`
7. Call Duration: `11 min`
8. Subject: `Retention call - saved account`
9. Call Purpose: `Retention`
10. Description: `Customer was cancelling due to price. Offered pause option. Customer stayed!`
11. Click **"Save"**.

**PRACTICE TASK:**
- Go to the Calls tab. You should see 3 calls.
- Filter by Call Purpose. Look for all "Retention" calls.
- Notice how the "No Answer" call shows 0 minutes. This is correct.

**CHECKPOINT:** Can you see 3 logged calls? Can you filter by Call Purpose? If yes, proceed.
