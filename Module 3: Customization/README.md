---

## MODULE 3: CUSTOMIZATION — Making Zoho CRM Fit TrueHunterer

---

### EXERCISE 11: Creating Custom Fields for Cat Information

**What you will learn:** How to add new fields that Zoho does not have by default.

**Why this matters:** Zoho CRM was built for general businesses. TrueHunterer needs fields like "Cat Name," "Food Preference," and "Allergy."

**STEP-BY-STEP:**

1. Click on the **Setup** icon (gear icon) at the top right of Zoho CRM.
2. In the left panel of the Setup page, find **"Customization"**.
3. Under Customization, click **"Modules and Fields"**.
4. You will see a list of modules: Leads, Accounts, Contacts, Deals, etc.
5. Click on **"Accounts"**.
6. You will see the layout of the Account form. There are sections like Account Information, Address Information, Description Information.
7. Look for a button or link that says **"New Field"** or a plus icon. Click it.
8. A menu appears with field types:
   - **Single Line** — For short text (like a cat's name)
   - **Multi Line** — For longer text (like feeding notes)
   - **Number** — For numbers (like number of cats)
   - **Date** — For dates (like subscription start date)
   - **Pick List** — For dropdown choices (like food preference: Chicken/Fish)
   - **Checkbox** — For yes/no (like has allergies?)
9. Create these custom fields one by one:

**FIELD 1: Number of Cats**
- Field Type: `Number`
- Field Label: `Number of Cats`
- Field Name: `Number_of_Cats`
- Click **"Save"**.

**FIELD 2: Cat Names**
- Field Type: `Single Line`
- Field Label: `Cat Names`
- Field Name: `Cat_Names`
- Click **"Save"**.

**FIELD 3: Food Preference**
- Field Type: `Pick List`
- Field Label: `Food Preference`
- Field Name: `Food_Preference`
- Options: `Chicken`, `Fish`, `Grain-Free`, `Mixed`
- Click **"Save"**.

**FIELD 4: Allergies**
- Field Type: `Multi Line`
- Field Label: `Allergies`
- Field Name: `Allergies`
- Click **"Save"**.

**FIELD 5: Subscription Type**
- Field Type: `Pick List`
- Field Label: `Subscription Type`
- Field Name: `Subscription_Type`
- Options: `Monthly`, `Bi-Weekly`, `Quarterly`, `Annual`
- Click **"Save"**.

**FIELD 6: Subscription Start Date**
- Field Type: `Date`
- Field Label: `Subscription Start Date`
- Field Name: `Subscription_Start_Date`
- Click **"Save"**.

**FIELD 7: Preferred Communication**
- Field Type: `Pick List`
- Field Label: `Preferred Communication`
- Field Name: `Preferred_Communication`
- Options: `WhatsApp`, `Phone Call`, `Email`, `SMS`
- Click **"Save"**.

**FIELD 8: Last Reorder Date**
- Field Type: `Date`
- Field Label: `Last Reorder Date`
- Field Name: `Last_Reorder_Date`
- Click **"Save"**.

**FIELD 9: Next Reorder Date**
- Field Type: `Date`
- Field Label: `Next Reorder Date`
- Field Name: `Next_Reorder_Date`
- Click **"Save"**.

**FIELD 10: Payment Status**
- Field Type: `Pick List`
- Field Label: `Payment Status`
- Field Name: `Payment_Status`
- Options: `Paid`, `Pending`, `Overdue`, `Failed`
- Click **"Save"**.

10. Now go back to the Accounts module.
11. Click on any account (like "Aarav Sharma").
12. Click the **"Edit"** button.
13. Scroll down. You should see your new custom fields.
14. Fill in sample data for 5 accounts:
    - Aarav Sharma: Number of Cats = 1, Cat Names = Whiskers, Food Preference = Chicken, Subscription Type = Monthly, Preferred Communication = Phone Call
    - Priya Patel: Number of Cats = 2, Cat Names = Muffin, Cookie, Food Preference = Chicken, Subscription Type = Bi-Weekly, Preferred Communication = WhatsApp
    - Sneha Nair: Number of Cats = 1, Cat Names = Luna, Food Preference = Chicken, Subscription Type = Monthly, Preferred Communication = WhatsApp, Payment Status = Overdue

**PRACTICE TASK:**
- Edit 10 more accounts and fill in the custom fields using the information from the Deal descriptions.
- For example, Ananya Iyer has 3 cats (Milo, Oreo, Ginger).

**CHECKPOINT:** Can you see your 10 new custom fields when you edit an Account? Have you filled data for at least 5 accounts? If yes, proceed.

---

### EXERCISE 12: Creating a Custom Module — "Cat Profiles"

**What you will learn:** How to create an entirely new section in Zoho CRM just for cat information.

**Why this matters:** Some subscribers have multiple cats. Each cat has its own name, age, weight, and health notes. A separate module keeps this organized.

**STEP-BY-STEP:**

1. Go to **Setup** (gear icon).
2. Under **Customization**, click **"Modules and Fields"**.
3. Look for a button that says **"Create New Module"** or **"New Module"**. Click it.
4. A form appears:
   - **Module Name:** Type `Cat Profiles`
   - **Module Label:** `Cat Profiles`
   - **Plural Label:** `Cat Profiles`
5. Click **"Create"** or **"Save"**.
6. Zoho will create the new module. It may take a few seconds.
7. You will be taken to the layout editor for Cat Profiles.
8. Now add these fields to the Cat Profiles module:

**FIELD 1: Cat Name**
- Type: Single Line
- Label: `Cat Name`
- Required: Yes (check the box)

**FIELD 2: Parent Account**
- Type: Lookup
- Label: `Parent Account`
- Related Module: `Accounts`
- This links each cat to a subscriber account

**FIELD 3: Breed**
- Type: Pick List
- Label: `Breed`
- Options: `Persian`, `Indie`, `Siamese`, `Maine Coon`, `British Shorthair`, `Ragdoll`, `Bengal`, `Mixed Breed`, `Other`

**FIELD 4: Age (Years)**
- Type: Number
- Label: `Age (Years)`

**FIELD 5: Weight (kg)**
- Type: Decimal
- Label: `Weight (kg)`

**FIELD 6: Food Preference**
- Type: Pick List
- Label: `Food Preference`
- Options: `Chicken`, `Fish`, `Grain-Free`, `Mixed`

**FIELD 7: Health Notes**
- Type: Multi Line
- Label: `Health Notes`

**FIELD 8: Allergies**
- Type: Multi Line
- Label: `Allergies`

**FIELD 9: Vet Visit Date**
- Type: Date
- Label: `Last Vet Visit`

**FIELD 10: Photo**
- Type: Image Upload
- Label: `Cat Photo`

9. Click **"Save"** after adding each field.
10. Now go back to the main CRM screen.
11. Look at the left navigation panel. Scroll down. You should see **"Cat Profiles"** as a new module.
12. Click on it. It will be empty.
13. Click **"Create Cat Profile"** (plus icon).
14. Create these cat profiles:

**Cat Profile 1:**
- Cat Name: Whiskers
- Parent Account: Aarav Sharma
- Breed: Indie
- Age: 3
- Weight: 4.5
- Food Preference: Chicken
- Health Notes: Healthy, active, no issues
- Allergies: None

**Cat Profile 2:**
- Cat Name: Muffin
- Parent Account: Priya Patel
- Breed: Persian
- Age: 2
- Weight: 3.8
- Food Preference: Chicken
- Health Notes: Sensitive stomach, needs grain-free sometimes
- Allergies: Wheat

**Cat Profile 3:**
- Cat Name: Cookie
- Parent Account: Priya Patel
- Breed: Indie
- Age: 1
- Weight: 3.2
- Food Preference: Fish
- Health Notes: Very active kitten
- Allergies: None

**Cat Profile 4:**
- Cat Name: Luna
- Parent Account: Sneha Nair
- Breed: British Shorthair
- Age: 4
- Weight: 5.1
- Food Preference: Chicken
- Health Notes: Recently lost weight, monitor closely
- Allergies: Dairy

**Cat Profile 5:**
- Cat Name: Simba
- Parent Account: Vikram Reddy
- Breed: Maine Coon
- Age: 5
- Weight: 6.8
- Food Preference: Fish
- Health Notes: Large breed, needs more food
- Allergies: None

15. Click **"Save"** after each profile.

**PRACTICE TASK:**
- Go to Account "Priya Patel". Look at the right panel or related records section. You should see 2 cat profiles linked.
- Go to Account "Aarav Sharma". You should see 1 cat profile.

**CHECKPOINT:** Can you see the "Cat Profiles" module in the left panel? Can you create a cat profile and link it to an account? If yes, proceed.

---

### EXERCISE 13: Rearranging Fields and Creating Sections

**What you will learn:** How to organize the page so important information is easy to find.

**Why this matters:** You will look at 100+ accounts. The layout should show cat information first, not bury it at the bottom.

**STEP-BY-STEP:**

1. Go to **Setup** -> **Customization** -> **Modules and Fields** -> **Accounts**.
2. You are in the Layout Editor. This shows how the Account page looks.
3. You will see sections like "Account Information" and "Address Information."
4. Look for a button that says **"New Section"** or a plus icon. Click it.
5. Name the new section: `Cat and Subscription Details`
6. Click **"Save"** or **"Create"**.
7. Now you will see a new empty section on the layout.
8. Find your custom fields (Number of Cats, Cat Names, Food Preference, etc.). They are probably in the "Account Information" section.
9. Click and drag each custom field into the new "Cat and Subscription Details" section.
10. Arrange them in this order:
    - Number of Cats
    - Cat Names
    - Food Preference
    - Allergies
    - Subscription Type
    - Subscription Start Date
    - Preferred Communication
    - Last Reorder Date
    - Next Reorder Date
    - Payment Status
11. Click **"Save"** on the layout.
12. Go back to Accounts. Click on "Aarav Sharma."
13. Scroll down. You should see a clean section called "Cat and Subscription Details" with all the important info together.

**PRACTICE TASK:**
- Do the same for the Contacts module. Create a section called `Communication Preferences` and move fields like Preferred Communication there.
- Do the same for the Deals module. Create a section called `Subscription Details` and add custom fields like Reorder Cycle, Payment Link Status, etc.

**CHECKPOINT:** When you open an Account, can you see all cat information in one clean section? If yes, proceed.
