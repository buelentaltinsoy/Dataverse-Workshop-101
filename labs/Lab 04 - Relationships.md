# Lab 4 - Relationships & Lookups 🔗

*In this lab, understanding relationships is the most important skill in Dataverse. You will learn why we link tables instead of using simple lists, and how to connect your countries to their respective continents for a professional 2026 data architecture.*

This lab consists of three parts:

🏰 **The Parent Table**: Creating a master "Continent" table.

🔗 **The Lookup**: Connecting Countries to Continents.

🧠 **Architectural Decision**: Understanding Choice vs. Lookup.

---

## 🏗️ Why Relationships Matter?

In a professional database, we avoid repeating data to prevent errors. Instead of typing "Europe" for every single European country (which leads to typos like "Europ" or "Europa"), we create a **Parent Table** (Continents) and link it to **Child Records** (Countries). 

**Benefits for 2026:**
- **Data Integrity:** You only update a continent's name in one place.
- **AI Accuracy:** Copilot understands the hierarchy and can summarize data by continent automatically.
- **Reporting:** You can easily calculate the total population of a Continent by summing up its related Countries.

---

## 🏰 Part 1: Create the Continent Table

Before we can link a country to a continent, the continent table must exist.

1.  Navigate back to your **Solution** (e.g., `BuelentAltinsoy_Demo`).
2.  Click **+ New** > **Table** > **Table (advanced properties)**.
3.  **Display name:** `Continent`
4.  **Plural name:** `Continents`
5.  Click **Save**.
6.  **Add Data:** Open the table and add a few rows in the **Name** column (e.g., `Europe`, `Asia`, `Africa`, `North America`).

---

## 🔗 Part 2: Create the Relationship (The Lookup)

Now we will create a link. In Dataverse, a "Many-to-One" relationship is created by adding a **Lookup Column** to the "Child" table (Country).

1.  Go back to your **Country** table.
2.  Click **+ New** > **Column**.
3.  **Display name:** `Continent`
4.  **Data type:** Select **Lookup** > **Lookup**.
5.  **Related table:** Search for and select your **Continent** table.
6.  Click **Save**.
7.  Click **Relationships**.
8.  Click **Continent**.
9.  **Advanced options (Relationship Behavior):**
    *   Find the **Type of Behavior** setting.
    *   **Hint:** Usually, this is set to **Referential**. If you choose **Parental**, deleting a Continent would automatically delete all Countries linked to it! For this lab, keep it as **Referential**.
10.  Click **Cancel**.

### 🧪 Test the Relationship
1.  Go to the **Data** tab of your Country table.
2.  Find **Germany** (or choose another European conutry, if Germany doesn't exist; or just create Germany as data).
3.  In the new **Continent** column, click the dropdown. You can now select **Europe**.
    *   *Note: You aren't typing "Europe"; you are picking a record that already exists in the Continent table!*

---

## 🧠 Choice vs. Lookup: What to choose and when?

Beginners often confuse these two. Here is the 2026 gold standard for making the right choice:



