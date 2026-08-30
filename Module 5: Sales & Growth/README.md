---

## MODULE 5: SALES and GROWTH — New Subscriptions and Upsells

---

### EXERCISE 19: Creating a Subscription Pipeline

**What you will learn:** How to build a visual pipeline for tracking new subscriptions.

**Why this matters:** You need to see where each potential subscriber is in the journey — from first contact to first payment.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Customization** -> **Modules and Fields** -> **Deals**.
2. Look for **"Stage-Probability Mapping"** or **"Pipeline"**.
3. You will see the default pipeline with stages like:
   - Qualification
   - Needs Analysis
   - Value Proposition
   - Identify Decision Makers
   - Proposal/Price Quote
   - Negotiation/Review
   - Closed Won
   - Closed Lost
4. This is too generic for TrueHunter. We need a simpler pipeline.
5. Look for a button that says **"New Pipeline"** or **"Create Pipeline"**. Click it.
6. Name the pipeline: `TrueHunter Subscription Pipeline`
7. Now add these stages (click "Add Stage" for each):
   - Stage 1: `New Enquiry` — Probability: 10%
   - Stage 2: `Contacted` — Probability: 25%
   - Stage 3: `Plan Pitched` — Probability: 50%
   - Stage 4: `Trial Sent` — Probability: 60%
   - Stage 5: `Payment Pending` — Probability: 80%
   - Stage 6: `Closed Won` — Probability: 100%
   - Stage 7: `Closed Lost` — Probability: 0%
8. For each stage, you can set a color. Use:
   - New Enquiry: Gray
   - Contacted: Blue
   - Plan Pitched: Yellow
   - Trial Sent: Orange
   - Payment Pending: Light Green
   - Closed Won: Green
   - Closed Lost: Red
9. Click **"Save"**.
10. Go back to **Deals**.
11. Look for a dropdown that says "Standard" or "All Deals." Change it to your new pipeline: `TrueHunter Subscription Pipeline`.
12. You will see a Kanban (card) view with columns for each stage.
13. Drag and drop deals between stages.

**PRACTICE TASK:**
- Create 5 new deals for leads who have NOT yet subscribed.
- Use leads from the Leads module who are still "Not Contacted."
- Example: Create a deal for `Sonal Das` with Stage = `New Enquiry`.
- Move each deal through the stages as you imagine the sales process.

**CHECKPOINT:** Can you see your custom pipeline? Can you move deals between stages? If yes, proceed.

---

### EXERCISE 20: Upselling — Creating Upsell Deals

**What you will learn:** How to track upsell opportunities (larger packs, treats, multi-cat plans).

**Why this matters:** The JD says "recommend larger packs, treats, and multi-cat plans where it genuinely helps."

**STEP-BY-STEP:**

1. Go to **Accounts**.
2. Click on `Ananya Iyer` (she has 3 cats — perfect upsell candidate).
3. She currently has a Quarterly subscription (Rs.6,999).
4. Create a new Deal for the upsell:
   - Click on the **"Deals"** related list on Ananya's account page.
   - Click **"Create Deal"** or the plus icon.
   - Deal Name: `Ananya Iyer - Upsell to Treats Pack`
   - Amount: `199`
   - Stage: `Plan Pitched`
   - Type: `Upsell`
   - Description: `Ananya's 3 cats love our food. Recommend monthly treats pack (Dental + Hairball). Total extra revenue: Rs.398/month.`
5. Click **"Save"**.
6. Now create another upsell deal:
   - Go to Account `Neha Agarwal` (2 cats, currently on Quarterly).
   - Create Deal: `Neha Agarwal - Multi-Cat Bundle Upsell`
   - Amount: `1999`
   - Stage: `New Enquiry`
   - Type: `Upsell`
   - Description: `Currently buying 2 separate packs. Multi-cat bundle saves Rs.500/month.`

**PRACTICE TASK:**
- Create upsell deals for 10 subscribers.
- Identify the right upsell for each:
  - Monthly subscribers with 1 cat -> Upsell to larger pack or treats
  - Bi-weekly subscribers -> Upsell to monthly (better value)
  - Subscribers with 2+ cats -> Multi-cat bundle
  - Kitten food buyers -> Adult food transition
- Use the Products module to check prices.

**CHECKPOINT:** Can you create an upsell deal linked to an existing account? Can you see both the original deal and the upsell deal on the account page? If yes, proceed.


### EXERCISE 21: Tracking Referrals

**What you will learn:** How to track which subscribers referred new customers.

**Why this matters:** The JD says "turn happy subscribers into a referral engine."

**STEP-BY-STEP:**

1. First, create a custom field on the Accounts module:
   - Go to Setup -> Customization -> Accounts -> New Field
   - Type: Lookup
   - Label: `Referred By`
   - Related Module: `Accounts`
   - This creates a link: New Account -> was referred by -> Existing Account
2. Also create a field:
   - Type: Number
   - Label: `Referral Count`
   - This counts how many people this subscriber has referred
3. Also create a field:
   - Type: Currency
   - Label: `Referral Credit Earned`
4. Now practice:
   - Go to Account `Aditya Singh`. His description says "Referred by existing customer."
   - Edit Aditya's account. In the `Referred By` field, search for and select `Aarav Sharma` (or whoever referred him).
   - Click Save.
   - Go to Aarav Sharma's account. Change his `Referral Count` to 1. Change `Referral Credit Earned` to 500.
5. Create a task:
   - Subject: `Send referral credit to Aarav Sharma`
   - Related To: Aarav Sharma
   - Description: `Rs.500 credit for referring Aditya Singh. Apply to next order.`

**PRACTICE TASK:**
- Find all accounts that say "Referred by" or "Referral" in their description.
- Link each to the referrer account.
- Update the referrer's Referral Count and Credit.
- Create tasks to send credits.

**CHECKPOINT:** Can you see the "Referred By" field populated? Can you track referral credits? If yes, proceed.
