# Lab 1 - Environment Setup 🌐

*Before diving into the technical labs, we’ll make sure that all workshop prerequisites are met and that you have your own working copy of the lab materials. This lab ensures you have a "Clean Room" environment and a properly provisioned Dataverse instance for 2026.*

This lab consists of four parts:

🧼 **The "Clean Room" Setup**: Isolating your training account.

🔑 **Account Provisioning**: Getting your Power Apps Developer Plan.

🏗️ **Environment Creation**: Building your Dataverse database.

🧬 **Repo Preparation**: Forking the workshop materials.

---

## 🧼 Part 1: Create a "Clean Room" Browser Profile

Most users use Microsoft Edge or Google Chrome for their daily work. Since you will be using a **Training/Developer account** today, being logged into your "Work" account in another tab can cause "Session Bleed," leading to permission errors.

### Option A: Create a New Chrome Profile (Recommended)
1. Open **Google Chrome**.
2. Click on the **Profile icon** in the top-right corner.
3. Click **+ Add** at the bottom of the menu.
<img width="233" height="246" alt="image" src="https://github.com/user-attachments/assets/e93ee919-cd44-4319-9e34-29ae4795312b" />

4. Select **"Continue without an account"**.
<img width="752" height="343" alt="image" src="https://github.com/user-attachments/assets/b8d63bea-d9b7-43bc-8d96-a880ed1da2dd" />

5. Name it `Dataverse Workshop` and choose a distinct color.
<img width="585" height="586" alt="image" src="https://github.com/user-attachments/assets/b0148dc8-db0b-45b8-8753-83c7a9f34de4" />

6. **Benefit:** This profile keeps its own cookies and sessions. You won't have to log out of your work account!

### Option B: Using Incognito Mode
- If you cannot create a profile, use **Incognito Mode** (`Ctrl + Shift + N`).
- ⚠️ *Note:* You will have to log in again every time you close the browser.

---

## 🔑 Part 2: Obtain your Training License

The best way to learn Microsoft Dataverse in 2026 is through the **Power Apps Developer Plan**.

### 1. Power Apps Developer Plan (Recommended)
This is the standard for learners. It does not expire as long as you are active.
*   **Benefits:** 2 GB Dataverse capacity, unlimited apps/flows, and up to 3 environments.
*   **How to get it:** Sign up with your work or school account at the [Power Apps Developer Plan website](www.microsoft.com).

### 2. Microsoft 365 Developer Program (Alternative)
*Use this if you do not have a corporate/school email.*
*   **Benefits:** Provides a free, renewable Microsoft 365 E5 sandbox with 25 licenses.
*   **How to get it:** Register at the [Microsoft 365 Developer Center](developer.microsoft.com). Use this new identity to then sign up for the Developer Plan above.

---

## 🏗️ Part 3: Create Your Dataverse Environment

Once you have your credentials, follow these steps to provision your database:

1.  Navigate to the [Power Platform Admin Center](admin.powerplatform.microsoft.com).
2.  Select **Environments** from the left-side menu and click **+ New**.
3.  **Choose Type:** Select **Developer** (for personal learning).
4.  **Add Database:** Ensure you toggle **"Add a Dataverse data store"** to **Yes**. 
5.  **Configure:** Choose your preferred language and currency, then click **Save**.

### Environment Types Comparison
| Type       | Best For                               | Expiration                  |
|------------|----------------------------------------|------------------------------|
| Developer  | Individual learning                    | Renewable (with activity)    |
| Sandbox    | Team testing & "Reset" features        | None (uses tenant capacity)  |
| Trial      | Short-term 30-day testing               | 30 Days                      |
| Teams      | Basic Dataverse within MS Teams         | Linked to Team lifecycle     |

## 🧬 Part 4: Fork and Clone the Workshop Repository

*Now let’s fork the repository and clone it locally so you can work with lab files in your own environment.*

1. Open the **Workshop Repo** in your new Browser Profile: `github.com`
2. Click the **Fork** button in the top right corner to create a copy in your own GitHub account.
3. Click the green **<> Code** button and copy the **HTTPS URL**.
4. Open your terminal (PowerShell or Bash) and run:
   ```bash
   # Navigate to your folder
   cd c:\workshops
   
   # Clone the repo
   git clone <YOUR_COPIED_URL>
   
   # Open in VS Code
   code dataverse-beginner-workshop

---

## 💡 Key Learning Outcomes
*   **Identity Isolation:** You learned how to use Browser Profiles to manage multiple Microsoft 365 identities without conflict.
*   **Environment Readiness:** You verified that your Dataverse "Sandbox" is provisioned and ready for custom tables.

***

✅ **You’re now ready to start Lab 2: The Data Model!**

