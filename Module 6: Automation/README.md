---

## MODULE 6: AUTOMATION — Working Smarter, Not Harder

---

### EXERCISE 22: Creating Workflow Rules (Automatic Actions)

**What you will learn:** How to make Zoho do work automatically.

**Why this matters:** You have 50+ subscribers and growing. You cannot manually remember everything.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Automation** -> **Workflow Rules**.
2. Click **"Create Rule"** or **"New Rule"**.
3. You will see a 3-step wizard.

**WORKFLOW 1: Payment Reminder**
- Module: `Accounts`
- Rule Name: `Payment Overdue Reminder`
- Description: `Automatically create a task when payment status becomes Overdue`
- When: `Edit` or `Create`
- Condition: `Payment Status` is `Overdue`
- Action: `Create Task`
  - Subject: `URGENT: Payment follow-up required`
  - Due Date: `Today`
  - Priority: `High`
  - Description: `Payment is overdue. Call subscriber immediately. Be polite but firm.`
- Click **"Save"**.

**WORKFLOW 2: New Subscriber Welcome**
- Module: `Deals`
- Rule Name: `New Subscriber Welcome Task`
- When: `Create`
- Condition: `Stage` is `Closed Won`
- Action: `Create Task`
  - Subject: `Welcome call new subscriber`
  - Due Date: `Tomorrow`
  - Priority: `Normal`
  - Description: `Welcome the new subscriber. Explain subscription process. Ask about their cat. Set expectations for first delivery.`
- Click **"Save"**.

**WORKFLOW 3: Reorder Reminder**
- Module: `Accounts`
- Rule Name: `Reorder Reminder 3 Days Before`
- When: `Edit`
- Condition: `Next Reorder Date` is `Today + 3 days` (Note: This may require a date-based formula. If too complex, skip and do manually.)
- Action: `Create Task`
  - Subject: `Reorder reminder - call subscriber`
  - Due Date: `Today`
  - Priority: `High`

**TESTING YOUR WORKFLOWS:**
1. Go to Accounts. Find any account with Payment Status = Paid.
2. Edit it. Change Payment Status to Overdue.
3. Click Save.
4. Go to Activities -> Tasks.
5. You should see a new High priority task automatically created!
6. Change the Payment Status back to Paid.

**PRACTICE TASK:**
- Create 3 more workflow rules:
  - When a deal moves to "Closed Lost," create a task: `Win-back attempt in 30 days`
  - When a new lead is created, assign it to you automatically
  - When a task is marked Completed, send an email to your manager

**CHECKPOINT:** Did the workflow automatically create a task when you changed Payment Status? If yes, proceed.

---

### EXERCISE 23: Assignment Rules (Auto-Assigning Leads)

**What you will learn:** How to automatically give new leads to the right person.

**Why this matters:** TrueHunterer gets leads from Instagram, WhatsApp, and pet communities. They need to reach a human fast.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Automation** -> **Assignment Rules**.
2. Click **"Create Rule"**.
3. Rule Name: `TrueHunterer Lead Assignment`
4. Module: `Leads`
5. Apply To: `All Leads`
6. Click **"Next"**.
7. You will see a section for "Assign To." Select your own user name.
8. Click **"Save"**.
9. Now create a test lead:
   - Go to Leads -> Create Lead
   - First Name: `Test`
   - Last Name: `Lead`
   - Email: `test@example.com`
   - Lead Source: `Website`
10. Click **"Save"**.
11. Look at the "Lead Owner" field. It should automatically show YOUR name.

**ADVANCED: Round-Robin Assignment**
- If TrueHunterer had 3 KAMs, you could set up round-robin: Lead 1 -> KAM 1, Lead 2 -> KAM 2, Lead 3 -> KAM 3.
- For now, since you are the only KAM, assign everything to yourself.

**PRACTICE TASK:**
- Create 5 test leads from different sources (Instagram, WhatsApp, Referral, Website, Pet Community).
- Verify that all 5 are automatically assigned to you.

**CHECKPOINT:** Are new leads automatically assigned to you? If yes, proceed.

---

### EXERCISE 24: Blueprint (Step-by-Step Process for Subscription Onboarding)

**What you will learn:** How to create a guided process so no step is missed when onboarding a new subscriber.

**Why this matters:** The JD says "own every subscriber." A Blueprint ensures every new subscriber gets the same excellent experience.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Automation** -> **Blueprint**.
2. Click **"Create Blueprint"**.
3. Module: `Deals`
4. Layout: `Standard`
5. Blueprint Name: `New Subscriber Onboarding`
6. Click **"Next"**.
7. You will see a canvas where you can draw your process.
8. The starting point is usually "New Enquiry."
9. Add these states (click "New State" for each):
   - `Welcome Call Scheduled`
   - `Welcome Call Completed`
   - `Trial Pack Sent`
   - `Trial Feedback Received`
   - `Subscription Confirmed`
   - `First Order Placed`
   - `First Delivery Completed`
   - `Onboarding Complete`
10. Connect the states with transitions (arrows):
    - New Enquiry -> Welcome Call Scheduled
    - Welcome Call Scheduled -> Welcome Call Completed
    - Welcome Call Completed -> Trial Pack Sent
    - Trial Pack Sent -> Trial Feedback Received
    - Trial Feedback Received -> Subscription Confirmed
    - Subscription Confirmed -> First Order Placed
    - First Order Placed -> First Delivery Completed
    - First Delivery Completed -> Onboarding Complete
11. For each transition, add conditions and actions:
    - Transition: New Enquiry -> Welcome Call Scheduled
      - Condition: None
      - Action: Create Task `Schedule welcome call`
    - Transition: Welcome Call Completed -> Trial Pack Sent
      - Condition: None
      - Action: Create Task `Send trial pack`
    - Transition: Trial Feedback Received -> Subscription Confirmed
      - Condition: `Feedback` is `Positive`
      - Action: Create Task `Send payment link for subscription`
12. Click **"Save"** and **"Publish"**.
13. Go to Deals. Create a new deal for a test lead.
14. You should see the Blueprint button on the deal record.
15. Click it and move the deal through each stage.

**PRACTICE TASK:**
- Move a test deal through the entire Blueprint.
- Notice how tasks are automatically created at each step.
- This ensures you never forget to send a trial pack or schedule a welcome call.

**CHECKPOINT:** Can you see the Blueprint on a Deal record? Can you move it through states? If yes, proceed.
