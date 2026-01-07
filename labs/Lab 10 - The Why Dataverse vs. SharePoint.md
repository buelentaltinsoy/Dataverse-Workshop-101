# LAB 10 - The "Why": Dataverse vs. SharePoint for Copilot 🤖

*In this final lab, we will explore the architectural differences between a "flat" list and a "relational" database. You will see first-hand why Dataverse is the required foundation for building sophisticated AI Agents in 2026.*

This lab consists of three comparative experiments:

📊 **The Logic Gap**: Testing cross-table reasoning.
🛡️ **The Security Gate**: Comparing granular access control.
🚀 **The Agentic Future**: Understanding why Copilot prefers Dataverse Search.

---

## 📊 Part 1: The Logic Gap (Relational Data)

*First, let's see how Copilot handles data stored in a simple list versus related tables.*

1. **The SharePoint Test:**
   - Go to your [SharePoint Site](microsoft.sharepoint.com) and create a list named `Project_Finances`.
   - Add columns: `Project Name` (Text), `Budget` (Number), and `Manager` (Text).
   - Add 3 rows of data, ensuring one manager has multiple projects.
   - Connect this list to a new agent in [Copilot Studio](copilotstudio.microsoft.com).
   - **Ask Copilot:** *"Which manager is currently managing the highest total budget across all their projects?"*
   - 💡 *Observation:* Copilot usually struggles to aggregate "flat" list data accurately.

2. **The Dataverse Test:**
   - Navigate to [Power Apps](make.powerapps.com) and open your **Tables**.
   - Create a relationship: Link an `Expenses` table to a `Departments` table (1:N).
   - Ensure you have **Rollup Fields** or **Calculated Columns** defined.
   - Add the Dataverse tables as a Knowledge source in Copilot Studio.
   - **Ask Copilot:** *"Compare the total IT spending against their allocated budget cap."*
   - ✅ *Result:* Because Dataverse understands the **Relationship**, the AI can join the data points to give a precise answer.

---

## 🛡️ Part 2: The Security Gate (Granular Access)

*In 2026, data privacy is the #1 priority for AI. Let's see how these platforms protect sensitive info.*

1. **SharePoint "All or Nothing":**
   - In SharePoint, grant a teammate "Read" access to your list.
   - Notice that they can see **every row** in that list. If Copilot indexes this, it will summarize all rows for that user.

2. **Dataverse "Row-Level Security":**
   - Go to the [Power Platform Admin Center](admin.powerplatform.microsoft.com).
   - Open your environment and navigate to **Users > Security Roles**.
   - Create a role where **Read Access** for a specific table is set to **User** (Basic) level.
   - This means a user only sees their *own* records.
   - **Test with Copilot:** Ask a query that targets data the user shouldn't see.
   - 🛡️ *Result:* Dataverse ensures Copilot **cannot** see data outside the user's scope, preventing "Over-sharing" leaks.

---

## 🚀 Part 3: The Agentic Future

*Why is Dataverse considered an "Agent Platform" rather than just a database?*

Review the checklist below to understand the technical requirements for 2026 AI Agents:

- [ ] **Dataverse Search:** Uses high-performance vector indexing. (SharePoint uses keyword search).
- [ ] **Long-term Memory:** Dataverse stores conversation transcripts as relational data for "memory" across sessions.
- [ ] **Action Plugins:** Dataverse allows Copilot to trigger **Power Automate** flows to update records, not just read them.

---

## 💡 Key Learning Outcomes

By completing this lab, you have mastered these core concepts:

*   🧠 **Relational Intelligence:** SharePoint is for lists; Dataverse is for **knowledge graphs**. AI agents need graphs to understand deep business context.
*   🔒 **Security by Design:** Dataverse ensures that if a user shouldn't see a row, the Copilot won't even know it exists—preventing AI hallucinations based on restricted data.
*   📈 **Scalability:** SharePoint performance degrades as lists grow; Dataverse is built on Azure SQL, allowing AI to query millions of records instantly.

---

## 🏆 Congratulations! You have completed the Dataverse Fundamentals Workshop!
