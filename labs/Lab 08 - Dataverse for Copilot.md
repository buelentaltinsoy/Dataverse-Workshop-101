# Lab 8 - Dataverse with Copilot: Knowledge & Grounding 🤖

*In this final lab, you will move beyond basic data entry and transform your database into a "Brain" for AI. You will learn how to "ground" a custom AI agent in your Dataverse tables, allowing users to ask natural language questions about your countries and continents. This is the cutting edge of Retrieval-Augmented Generation (RAG) in 2026.*

This lab consists of three parts:

🧠 **Knowledge Integration**: Connecting Dataverse tables to Copilot Studio.

🔍 **Search Optimization**: Enabling AI to "read" your custom columns.

💬 **The AI Test**: Chatting with your data in real-time.

---

## 🏗️ Why Grounding Matters?

By default, a general AI has no idea about *your* specific database updates (like your 2026 population estimates). **Grounding** is the process of giving an AI agent access to your Dataverse tables as its primary "source of truth."

**In 2026:**
- Your agent won't "hallucinate" because it is anchored to your specific records.
- You can ask complex questions like: *"Which country in my database has the highest population and what is its description?"*

---

## 🧠 Part 1: Connect Dataverse to Copilot Studio

We will use **Microsoft Copilot Studio** to build an agent that uses your "Country" and "Continent" tables as knowledge sources.

1.  Navigate to [Microsoft Copilot Studio](https://copilotstudio.microsoft.com).
2.  Ensure you are in the same **Developer Environment** used for your tables.
3.  Click **+ Create** > **New agent**.
4.  **Name:** `Global Geography Expert`.
5.  On the **Knowledge** tab, click **+ Add knowledge**.
6.  Select **Dataverse** from the list of sources.
7.  **Select Tables:** Search for and select your `Country` and `Continent` tables.
8.  Click **Add**.

---

## 🔍 Part 2: Optimize Search (The "Brain" Setup)

For the AI to find your data, you must ensure your columns are "Searchable" within the Dataverse index.

1.  Navigate back to the [Power Apps Maker Portal](https://make.powerapps.com).
2.  Open your **Country** table and select **Views**.
3.  Open the **Quick Find View** (this is the view AI uses to crawl data).
4.  On the right-hand panel, click **Edit find table columns**.
5.  Ensure `Country Name`, `Population`, and `Description` are all checked.
6.  Click **Apply**, then **Save and Publish**.
    *   *Note: This allows the Dataverse Search engine to index these specific fields for the AI.*

---

## 💬 Part 3: Test Your Grounded Agent

Now, let's see if the AI can truly understand your custom data.

1.  Return to **Copilot Studio** and open your `Global Geography Expert` agent.
2.  Open the **Test pane** on the right side.
3.  **Try these prompts:**
    *   *"What is the population of Germany according to my data?"*
    *   *"Give me a summary of the countries located in Europe."*
    *   *"Which country is described as being special because of its history?"*
4.  **Observe:** Notice the "citations" or small numbers next to the AI's answer. If you click them, they will link directly back to your Dataverse record!

---

## ✅ Final Workshop Summary

Congratulations! You have completed the **2026 Dataverse Beginner Training**. 

You have successfully:
*   Built a **Relational Data Model** from scratch.
*   Automated data entry with **AI Copilot**.
*   Designed a professional **Model-Driven App**.
*   Secured your data with **Role-Based Access Control (RBAC)**.
*   **Grounded a Custom AI Agent** in your business data.

**Next Steps:** You are now ready to explore [Power Automate](https://make.powerautomate.com) to create workflows, such as sending an email alert whenever a new Country is added to your database!
