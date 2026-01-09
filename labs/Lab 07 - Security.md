# Lab 7 - Dataverse Security Fundamentals 🔐

*Building an app is only half the battle. In 2026, protecting your data is paramount. In this lab, you will learn the fundamentals of Dataverse security: how to control who can see your "Country" data and how to define exactly what they can do with it (Read, Write, or Delete).*

This lab consists of two practical mini-labs:

👤 **Security Roles**: Defining "Who" can do "What".

🤝 **Sharing the App**: Granting access to your colleagues.

---

## 🏗️ Why Security in Dataverse is Unique

Unlike simple spreadsheets, Dataverse uses **Role-Based Access Control (RBAC)**. 
- **Security Roles** are a collection of permissions (privileges).
- **Users** are assigned to these roles.
- **Ownership:** You can decide if a user can see *only their own* countries or *every* country in the database.

---

## 👤 Mini-Lab A: Create a Custom Security Role

In this lab, we will create a "Country Viewer" role for people who should see the data but not change it.

1.  Navigate to the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com).
2.  Select **Manage**/**Environments** on the left and click on the name of your training environment.
3.  Click **Settings** (top menu) > **Users + permissions** > **Security roles**.
4.  Click **+ New role**.
5.  **Role Name:** Enter `Country Viewer - <YOURNAME>`.
6.  Select your **Business Unit**.
7.  Provide this description:
> A role to view countries only.
8. Applies To:
> Visitors
9. Summary of Core Table Privileges: *Leave just a dash (-) there.*
10. Click **Save**.
11.  **Configure Permissions:**
    *   Search for your **Country** table in the list.
    *   Click the **Read** dropdown and select Organization-level access.
    *   Ensure **Write**, **Delete**, and **Create** remain empty/red.
9.  **Essential Apps Access:** Search for the **Model-driven App** privilege and ensure "Read" is granted so the user can actually open your "Global Data Manager" app.
10.  Click **Save and Close**.

---

## 🤝 Mini-Lab B: Share the App and Assign the Role

Now that the role exists, we must link it to our App so users can log in.

1.  Go back to your [Power Apps Maker Portal](https://make.powerapps.com) and enter your solution.
2.  Find your **Global Data Manager** app in the list under **Apps**.
3.  Click the **three dots (...)** next to the app name and select **Share**.
4.  In the sharing pane:
    *   **Add a User:** Type the name of a fellow participant or a test user. For example Raul Razo. 
    *   **Assign Role:** Select the `Country Viewer - <YOURNAME>` role you just created.
5.  Click **Share**.
6.  **Result:** That user now has permission to open the URL of your app and view your countries, but the "New" and "Delete" buttons will be hidden for them!

---

## 💡 Pro-Tip: The "Security Matrix"
Dataverse allows for **Column-Level Security**. If you have a sensitive column (like "Government Secret Code"), you can hide just that one column while letting the user see the rest of the Country record!

---

## ✅ Summary & Next Steps

You have now successfully:
*   Created a custom **Security Role** with specific table permissions.
*   Learned the difference between **Read** and **Write** privileges in a relational database.
*   **Shared** your Model-Driven App with another identity safely.

*Congratulations! You have built a fully functional, secure, and relational Dataverse solution. In our next chapter, we will see how to use Dataverse and Copilot!*
