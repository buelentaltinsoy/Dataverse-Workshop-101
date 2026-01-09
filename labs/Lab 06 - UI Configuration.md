# Lab 6 - UI Configuration: Building the App 📱

*In this lab, you will bring all your hard work together. We will package your Tables, Views, and Forms into a professional **Model-Driven App**. This provides a clean, responsive interface for your users to manage global data in 2026.*

This lab consists of three parts:

🏗️ **App Creation**: Launching the Model-Driven App designer.

🗺️ **Navigation Design**: Organizing the Sitemap with Countries and Continents.

🚀 **Publishing**: Making your application live for testing.

---

## 🏗️ Why a Model-Driven App?

In Dataverse, you don't have to design every button or screen manually. A **Model-Driven App** is "Data-First". It automatically generates the UI based on your table structure. It is perfectly suited for back-office management tools and works natively on mobile, tablet, and web.

---

## 🏗️ Part 1: Start the App from your Solution

Always start within your solution to ensure all components are tracked together for easy deployment.

1.  Navigate to your solution (e.g., `BuelentAltinsoy_Demo`).
2.  Click **+ New** > **App** > **Model-driven app**.
3.  **Name:** Enter `Global Data Manager`.
4.  **Description:** Enter `Internal tool to manage countries and their demographics.`
5.  Click **Create**.
6.  The **Modern App Designer** will open in a new tab.

---

## 🗺️ Part 2: Add Tables to the Navigation (Sitemap)

The "Sitemap" is the left-hand navigation menu of your app. We need to tell the app which tables the user is allowed to interact with.

1.  In the App Designer, Click **+ Add page** > **Subarea** (or click the "+ New" icon next to "Navigation").
2.  Select **Dataverse Table**.
3.  **Select Table:** Search for and select your **Country** and **Continent** table.
4.  **Organize:** Drag the **Country** subarea to the top so it is the first thing users see.
7.  (Optional) Click on the "New Group" heading in the navigation and rename it to `World Management`.

---

## 🚀 Part 3: Preview and Publish

Before anyone can use the app, it must be published to compile all the recent changes to your Forms and Views.

1.  Click **Save** in the top right corner.
2.  Click **Publish** (This makes the app live in the environment).
3.  Click the **Play** button to open the app in a new browser window.
4.  **Test the UI:**
    *   Click on **Countries** in the menu. You should see your customized view with the Population column.
    *   Click **+ New** to see your modified form with the "Country Details" section.
    *   Click on **Continents** to manage the parent categories.

---

## 💡 Pro-Tip: Responsive Design
Notice how the app looks professional without you writing a single line of CSS or HTML. Try resizing your browser window; you will see the navigation and forms automatically adapt—this is the power of the Model-Driven framework in 2026.

---

## ✅ Summary & Next Steps

You have now successfully:
*   Initialized a **Model-Driven App** from within your solution.
*   Configured the **Navigation (Sitemap)** to include both Country and Continent tables.
*   **Published** and tested the application in a live browser session.

*In the next lab, we will tackle **Security**, learning how to share this app with others while protecting your data!*
