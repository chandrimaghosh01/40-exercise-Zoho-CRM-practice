---

## MODULE 7: REPORTS and DASHBOARDS — Numbers That Matter

---

### EXERCISE 25: Creating a Subscriber Overview Report

**What you will learn:** How to build a report showing all active subscribers.

**Why this matters:** The JD says "share weekly numbers on active subscribers, churn, payment conversion."

**STEP-BY-STEP:**

1. Go to **Reports** in the left panel.
2. Click **"Create Report"** or the plus icon.
3. Select module: `Accounts`
4. Report Name: `Active Subscribers Overview`
5. Report Type: `Tabular` (rows and columns, like Excel)
6. Select these columns:
   - Account Name
   - Account Number
   - Rating
   - Subscription Type (custom field)
   - Number of Cats (custom field)
   - Food Preference (custom field)
   - Payment Status (custom field)
   - Next Reorder Date (custom field)
7. Add a filter:
   - `Account Type` equals `Subscriber`
8. Click **"Save"**.
9. You will see a table with all your subscribers.
10. Click **"Export"** to download as Excel or PDF.

**PRACTICE TASK:**
- Create a similar report for Contacts showing:
  - Contact Name
  - Account Name
  - Phone
  - Email
  - Preferred Communication

**CHECKPOINT:** Can you see a table with all subscribers and their key details? Can you export it? If yes, proceed.

---

### EXERCISE 26: Creating a Revenue Report

**What you will learn:** How to calculate total revenue from subscriptions.

**Why this matters:** You need to know how much money the subscriber base is generating.

**STEP-BY-STEP:**

1. Go to **Reports**.
2. Click **"Create Report"**.
3. Module: `Deals`
4. Report Name: `Monthly Subscription Revenue`
5. Report Type: `Summary` (groups data and shows totals)
6. Group By: `Closing Date` (group by month)
7. Select columns:
   - Deal Name
   - Account Name
   - Amount
   - Stage
8. Add filter:
   - `Stage` equals `Closed Won`
9. In the Summary section, add:
   - Sum of Amount
10. Click **"Save"**.
11. You will see revenue grouped by month.

**PRACTICE TASK:**
- Create a report showing revenue by Subscription Type (Monthly, Bi-Weekly, Quarterly).
- Create a report showing revenue by Lead Source (which channel brings the most money?).

**CHECKPOINT:** Does your report show total revenue? Can you group by different fields? If yes, proceed.

---

### EXERCISE 27: Creating a Churn and Retention Report

**What you will learn:** How to track which subscribers are leaving and why.

**Why this matters:** The JD says "spot at-risk accounts early" and "win back the ones who lapsed."

**STEP-BY-STEP:**

1. Go to **Reports**.
2. Create Report -> Module: `Accounts`
3. Report Name: `At-Risk Subscribers`
4. Report Type: `Tabular`
5. Columns:
   - Account Name
   - Rating
   - Payment Status
   - Last Reorder Date
   - Next Reorder Date
   - Description
6. Filter:
   - `Rating` equals `Cold` OR `Payment Status` equals `Overdue`
7. Save.

**PRACTICE TASK:**
- Create a report for `Win-Back Opportunities`:
  - Module: Deals
  - Filter: Stage = `Closed Lost`
  - Columns: Deal Name, Account Name, Amount, Lost Reason (you may need to create a custom field for Lost Reason)
- Create a custom field on Deals called `Lost Reason` (Pick List with options: Price, Product Issue, Delivery Issue, Cat Didn't Like, Moving Away, Other).

**CHECKPOINT:** Can you see a list of at-risk subscribers? Can you filter by multiple conditions? If yes, proceed.

---

### EXERCISE 28: Building a KAM Dashboard

**What you will learn:** How to create a visual dashboard that shows everything at a glance.

**Why this matters:** The JD says "flag problems before they become problems." A dashboard shows problems in red.

**STEP-BY-STEP:**

1. Go to **Analytics** or **Dashboards** in the left panel.
2. Click **"Create Dashboard"** or the plus icon.
3. Dashboard Name: `TrueHunterer KAM Dashboard`
4. You will see a blank canvas with boxes.
5. Add these components (click "Add Component" for each):

**COMPONENT 1: Total Active Subscribers**
- Type: `Count`
- Module: `Accounts`
- Filter: Account Type = Subscriber
- Display as: Big Number

**COMPONENT 2: Revenue This Month**
- Type: `Sum`
- Module: `Deals`
- Field: `Amount`
- Filter: Stage = Closed Won, Closing Date = This Month
- Display as: Big Number with Rs. symbol

**COMPONENT 3: Payment Status Breakdown**
- Type: `Pie Chart`
- Module: `Accounts`
- Field: `Payment Status`
- Filter: Account Type = Subscriber
- This shows a pie chart: Paid vs Pending vs Overdue vs Failed

**COMPONENT 4: At-Risk Accounts**
- Type: `List`
- Module: `Accounts`
- Filter: Rating = Cold
- Columns: Account Name, Phone, Next Reorder Date
- This shows a red-alert list

**COMPONENT 5: Tasks Due Today**
- Type: `List`
- Module: `Tasks`
- Filter: Due Date = Today
- Columns: Subject, Related To, Priority

**COMPONENT 6: New Subscriptions This Month**
- Type: `Bar Chart`
- Module: `Deals`
- X-Axis: `Closing Date` (by week)
- Y-Axis: `Count of Deals`
- Filter: Stage = Closed Won, Type = New Business

**COMPONENT 7: Revenue by Subscription Type**
- Type: `Bar Chart`
- Module: `Deals`
- X-Axis: `Subscription Type` (custom field)
- Y-Axis: `Sum of Amount`

6. Arrange the components on the canvas:
   - Top row: Total Subscribers, Revenue This Month, Payment Status Pie
   - Middle row: At-Risk Accounts, Tasks Due Today
   - Bottom row: New Subscriptions Chart, Revenue by Type Chart
7. Click **"Save"**.
8. Set this as your default dashboard:
   - Click the three dots on the dashboard -> Set as Default

**PRACTICE TASK:**
- Refresh the dashboard after updating some data.
- Notice how numbers change when you mark a task complete or change a payment status.
- Share the dashboard with a colleague (if available) by clicking Share.

**CHECKPOINT:** Can you see all 7 components on one screen? Do the numbers update when you change data? If yes, proceed.
