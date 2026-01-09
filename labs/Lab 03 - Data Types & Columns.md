# Lab 3 - Data Types and Columns 📊

*Now that you have created your table, it’s time to define the specific details we want to track. In Dataverse, we do this by adding **Columns**. You will learn how to manually create different data types and use **Copilot** to intelligently fill in the missing information for 2026.*

This lab consists of three parts:

📝 **Text Columns**: Adding a description field.

🔢 **Number Columns**: Adding a population field.

🤖 **AI Data Enrichment**: Using Copilot to fill in the blanks.

---

## 📝 Part 1: Create a Description Column (String)

A "String" or "Text" column is used for alphanumeric characters. We will use this to store a brief summary of each country.

1.  Navigate to your solution and click on your **Country** table to open it.
2.  In the top menu or the "Schema" section, click **+ New** > **Column**.
3.  **Display name:** `Description`
4.  **Data type:** Select **Text** > **Plain text**.
5.  **Required:** Set to **Optional** (default).
6.  **Advanced options:** Verify that the "Logical name" starts with your prefix (e.g., `jane_description`).
7.  Click **Save**.

---

## 🔢 Part 2: Create a Population Column (Number)

For statistics like population, we use a Number data type. This allows the system to perform calculations and sorting later.

1.  While still in the table editor, click **+ New** > **Column** again.
2.  **Display name:** `Population`
3.  **Data type:** Select **Number** > **Whole number**.
    *   *Note: We use "Whole number" because you cannot have half a person!*
4.  **Format:** Select **None** (or leave as default).
5.  Click **Save**.

---

## 📚 Understanding Dataverse Data Types

When building professional apps in 2026, choosing the right "container" for your data is vital:

 Data Type       | Best Used For...                                           | Example Text (String)                     |
|-----------------|-----------------------------------------------------------|------------------------------------------|
| Names, descriptions, addresses, or any alphanumeric notes. | "France is in Europe"                                  |
| Whole Number    | Quantities, counts, or IDs where decimals aren't needed.  | 67,000,000                                |
| Decimal/Float   | Precise measurements or scientific data.                  | 9.81 (Gravity)                            |
| Currency        | Financial values (automatically handles exchange rates).  | $500.00                                   |
| Date and Time   | Deadlines, birthdays, or transaction timestamps.          | 01/09/2026                                |
| Choice          | A dropdown list of predefined options.                    | North America, Europe, Asia               |
| Lookup          | Creating a relationship to another table.                 | Linking a City to a Country               |


## ✅ Summary & Next Steps

You have now successfully:
*   Manually added a **Text** column for descriptions.
*   Created a **Whole Number** column for population data.
*   Used **Copilot** to research and auto-fill your table with real-world data.

*In the next lab, we will learn how to create **Relationships** to link our Countries to a new table called "Cities"!*
