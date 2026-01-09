# Lab 5 - Views and Forms 🖥️

*Now that your data structure is ready, you need to define the User Experience (UX). In Dataverse, **Views** determine how users see lists of records, and **Forms** determine how users interact with a single record.*

This lab consists of three parts:

👀 **View Customization**: Designing the "Active Countries" list.

📝 **Form Design**: Arranging fields for the best user experience.

🤖 **AI Data Entry**: Using Copilot to quickly populate your new UI.

---

## 🏗️ Why do we need Views and Forms?

Dataverse separates **Data** from **UI**. This means the table is just the "bucket," while Views and Forms act as the "windows" into that bucket.

- **Views:** Like a filtered Excel sheet. You decide which columns are important enough to show in a summary list.
- **Forms:** The layout for data entry. You organize fields into sections so users don't get overwhelmed by a long list of text boxes.

---

## 👀 Part 1: Create and Modify a View

A View defines which columns are visible in the list and how they are sorted.

1.  Navigate to your solution and open the **Country** table.
2.  In the "Data experiences" section, click on **Views**.
3.  Click on the **Active Countries** view to edit it.
4.  **Add Columns:** On the left-hand panel, click and drag the following columns into the preview table:
    *   `Continent`
    *   `Population`
    *   `Description`
5.  **Adjust Layout:** Click and drag the column headers to reorder them (e.g., Name, Continent, Population).
6.  **Sorting:** Click the **Population** column header and select **Sort Z to A** to see the largest countries first.
7.  Click **Save and Publish** in the top right corner.

---

## 📝 Part 2: Modify the Main Form

The Form is what appears when a user clicks "New" or opens a specific record.

1.  Go back to the **Country** table main page.
2.  In the "Data experiences" section, click on **Forms**.
3.  Click on the **Information** form (Type: **Main**).
4.  **Add Fields:** In the left-hand "Table columns" pane, click on your custom fields to add them to the form:
    *   `Continent`
    *   `Population`
    *   `Description`
5.  **Organize with Sections:** 
    *   Click **+ Component** > **1-column section**. 
    *   Rename the section to `Country Details`.
    *   Drag the `Population` and `Description` fields into this new section.
6.  Click **Save and Publish**.

---

## 🤖 Part 3: Use Copilot to Add Data

Now that the UI shows all our fields, let's use the Copilot sidecar to quickly add new records.

1.  Navigate back to the **All** tab on top of your solution.
2.  Click **New**/**Table**/**Tables**.
3.  Click **+ Exsting Tables** and select the Country table. The Country tile appears in the designer.
4.  Click on the Country tile and then on top menu **View data**.
5.  Configure your view to see County Name, Continent, Popluation and Description.
6.  Click **+New table**.
7.  Enter the following prompt (Note: Use the countries you want to fill in with information for your original Country table):
    > "Create a new Country2 table. Include their Name, Continent, Description (why this country is special) and a 2026 population estimate. Use Australia, Brazil, Canada, China, France, Germany, India, Japan, Mexico, USA.""
8. Copy und paste the infomation from the new temporary country to your country.
9. Click **<-Back**. Don't save the table!
11.   **Review and Keep:** Copilot will stage the rows. Click **"Add all"** to save them.
12.  **Observation:** Notice how the `Continent` field automatically looks up values from your Continent table!

---

## ✅ Summary & Next Steps

You have now successfully:
*   Customized a **View** to display population and continent data.
*   Modified a **Main Form** to create a structured user experience.
*   Used **Copilot** to instantly populate your table through the UI.

*In the next lab, we will build a **Model-Driven App** to package this entire experience into a professional business application!*
