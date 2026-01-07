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
*Use this if you do have a corporate/school email.*
This is the standard for learners. It does not expire as long as you are active.
*   **Benefits:** 2 GB Dataverse capacity, unlimited apps/flows, and up to 3 environments.
*   **How to get it:** Sign up with your work or school account at the [Power Apps Developer Plan website](https://www.microsoft.com/en-us/power-platform/products/power-apps/pricing).
1. Go to [Power Apps Developer Plan website](https://www.microsoft.com/en-us/power-platform/products/power-apps/pricing)
2. Locate the "Get started for free" or "Existing User? Add a developer environment" button.
<img width="475" height="400" alt="image" src="https://github.com/user-attachments/assets/49d8554b-ca53-403e-b084-36d5b2a396cd" />

3.  Enter your Work or School email address (or your Microsoft 365 Developer Program email). Note: Personal emails like @outlook.com or @gmail.com are not supported for this plan.
<img width="431" height="500" alt="image" src="https://github.com/user-attachments/assets/50f62a2a-0186-47ff-b567-3ca6a10c0081" />

4.  If prompted, sign in with your Microsoft 365 account credentials.
5.  Select your Country/Region and click Accept to agree to the terms and conditions. Note: Be aware that **some Copilot related features might not be avaialbe in your region**. To get all the latest features, please select **US** as your region.
6.  Once the setup wizard completes, you will be redirected to the Power Apps Maker Portal. Look at the **Environment Picker** in the top-right corner. Confirm that an environment named **[Your Name]'s Environment** (Type: Developer) is selected.


### 2. Microsoft 365 Developer Program (Alternative)
*Use this if you do not have a corporate/school email. These steps create a private "Sandbox" tenant. This will give you a professional identity to use for the rest of the workshop.*
*   **Benefits:** Provides a free, renewable Microsoft 365 E5 sandbox with 25 licenses.
*   **How to get it:** Register at the [Microsoft 365 Developer Center]([developer.microsoft.com](https://developer.microsoft.com/en-us/microsoft-365/dev-program)). Use this new identity to then sign up for the Developer Plan above.

1. Open your **Workshop Browser Profile**.
2. Navigate to the [Microsoft 365 Developer Center]([developer.microsoft.com](https://developer.microsoft.com/en-us/microsoft-365/dev-program)).
3. Click **Join now**.
4. Sign in with a personal Microsoft account (e.g., @outlook.com, @hotmail.com). If you don't have one, create one at https://outlook.live.com/
5. Select your **Country/Region** and your **Company** (you can use "Personal" or your name). Note: Be aware that **some Copilot related features might not be avaialbe in your region**. To get all the latest features, please select **US** as your region.
6. Choose as primary language **English** and click **Next**.
7. When prompted, select **Configurable Sandbox** (this allows you to choose your own domain name).
8. Click **Next**.
9. **Username:** Choose an admin name (e.g., `admin`).
10. **Domain:** Choose a unique name (e.g., `dataverseworkshop2026`). 
   > Your final email will look like: `admin@dataverseworkshop2026.onmicrosoft.com`.
11. **Password:** Set a strong password and **save it securely**.
12. Provide a mobile phone number for security verification and enter the code you receive.
13. Once your dashboard says "Subscription: Active," copy your new **@onmicrosoft.com** email address.
14. Go to [Power Apps Developer Plan website](https://www.microsoft.com/en-us/power-platform/products/power-apps/pricing)
15. Locate the "Get started for free" or "Existing User? Add a developer environment" button.
<img width="475" height="400" alt="image" src="https://github.com/user-attachments/assets/49d8554b-ca53-403e-b084-36d5b2a396cd" />

16.  Enter your Work or School email address (or your Microsoft 365 Developer Program email).

### ⚠️ Note
> Personal emails like @outlook.com or @gmail.com are not supported for this plan.

<img width="431" height="500" alt="image" src="https://github.com/user-attachments/assets/50f62a2a-0186-47ff-b567-3ca6a10c0081" />

17.  If prompted, sign in with your Microsoft 365 account credentials.
18.  Select your Country/Region and click Accept to agree to the terms and conditions. Note: 

### ⚠️ Note
> Be aware that **some Copilot related features might not be avaialbe in your region**. To get all the latest features, please select **US** as your region.

19.  Once the setup wizard completes, you will be redirected to the Power Apps Maker Portal. Look at the **Environment Picker** in the top-right corner. Confirm that an environment named **[Your Name]'s Environment** (Type: Developer) is selected.

---

### ⚠️ Important Note for 2026
> **Keep it active:** Microsoft detects "development activity." To ensure your sandbox is renewed, make sure to commit at least one change to a Power App or Dataverse table once every 60-90 days.

***

✅ **Identity Created! Now proceed to the Power Platform Admin Center to create your Dataverse environment.**


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

