# BONUS Lab - Data Portability: Dataverse vs. SharePoint 📋

*In this bonus lab, you will explore alternative data sources. While Dataverse is a robust relational database, many organizations use **SharePoint Lists** for simpler tasks. You will create a SharePoint list for "Countries" and see how it differs from the Dataverse experience you just completed.*

This lab consists of three parts:

🏗️ **List Creation**: Building a Country list in SharePoint.

📝 **Schema Setup**: Adding columns for Description and Population.

⚖️ **The Comparison**: Understanding when to use SharePoint vs. Dataverse in 2026.

---

## 🏗️ Part 1: Create the SharePoint List

1.  Navigate to your **Microsoft 365 Home** and open **SharePoint**.
2.  Select a Team Site or your "My Site."
3.  Click **+ New** > **List**.
4.  Select **Blank list**.
5.  **Name:** `Global Countries - SharePoint`.
6.  **Description:** `A flat list of countries for simple tracking.`
7.  Click **Create**.

---

## 📝 Part 2: Add Columns for Countries

In SharePoint, we add columns manually to match our Dataverse schema.

1.  **Rename Title Column:** Click on the "Title" column header > **Column settings** > **Rename** to `Country Name`.
2.  **Add Description:** 
    *   Click **+ Add column** > **Multiple lines of text**.
    *   **Name:** `Description`.
    *   Click **Save**.
3.  **Add Population:** 
    *   Click **+ Add column** > **Number**.
    *   **Name:** `Population`.
    *   **Number of decimal places:** `0`.
    *   Click **Save**.
4.  **Add Continent (Choice):**
    *   Click **+ Add column** > **Choice**.
    *   **Name:** `Continent`.
    *   **Choices:** `Europe`, `Asia`, `Africa`, `North America`, `South America`, `Oceania`.
    *   Click **Save**.

---

## ⚖️ Part 3: Why Dataverse is the better choice

Now that you've built both, let’s compare the two experiences, here are a few items:

 Feature       | SharePoint List                                           | Dataverse (from previous labs)                     
|-----------------|-----------------------------------------------------------|------------------------------------------|
| Relationships    | 	Lookup columns are "fragile" and harder to manage. | Native Relational Engine (Perfect for Continent -> Country).                             |
| Security   | 	Security is per-list or per-item (hard to manage at scale).                  | Role-Based Security (RBAC) with deep granularity.                            |
| AI (Copilot)   |	Basic AI assistance for data entry.          |	Deep Integration (Grounding for custom AI Agents).                              |
| Capacity          | Up to 30 million items per list.                  | Unlimited (constrained only by purchased storage).              |
| Query Threshold          | 5,000 items (List View Threshold).                | No fixed query limit; optimized for millions.               |
|Lookup Limit          | 12 Lookup columns per single view.                | No fixed lookup limit; constrained only by the total column count (max ~1,000).               |
| Storage Base        | 	1 TB per tenant + 10 GB per user license. |20 GB database + 20 GB file base (for Power Apps Premium).                                   |



## ✅ Bonus Summary

You have now successfully:
*   Built a **SharePoint List** to replicate your country data.
*   Added **Description**, **Population**, and **Choice** columns.
*   Learned to distinguish between **Flat Data** (SharePoint) and **Relational Data** (Dataverse).

*This concludes the bonus material. You now have a complete overview of the two most common data backends in the Microsoft Power Platform!*


