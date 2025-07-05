# 🌊 FlowPulse (Live on Replit)

FlowPulse is a real-time stablecoin flow dashboard built with React, Node.js, and WebSockets.

---

## One-Click Deployment

Click the button below to deploy this application to your own Replit account.

[![Deploy to Replit](https://replit.com/badge/github/YOUR_GITHUB_USERNAME/flowpulse-live)](https://replit.com/github/YOUR_GITHUB_USERNAME/flowpulse-live)

**Important:** After creating the repository, you **must** edit the link above and replace `YOUR_GITHUB_USERNAME` with your actual GitHub username.

---
## Setup After Deploying

1.  **Fork the Repl:** After clicking the button, Replit will fork the project into your account and automatically run `npm run install-all`.
2.  **Set up the Database:**
    -   In the Replit sidebar, go to the **Tools** section and click on **Postgres**.
    -   Click the **Create a database** button. Replit will provision a free PostgreSQL database for you.
3.  **Configure Secrets:**
    -   A `DATABASE_URL` will appear in the Postgres tab. Click the "Copy" icon next to it.
    -   Go to the **Tools** section and click on **Secrets**.
    -   Create a new secret. The key is `DATABASE_URL` and the value is the URL you just copied.
    -   Click "Add new secret".
4.  **Create Database Tables:**
    -   In the Replit sidebar, open the **Shell** tab.
    -   Run the following command to connect to your database and run the schema setup script. Paste this entire block into the shell and press Enter:
    ```bash
    psql $DATABASE_URL -f server/src/db/schema.sql
    ```
5.  **Run the Application:**
    -   Click the big green **"Run"** button at the top.
    -   Replit will start both the backend server and the frontend dev server. A "WebView" tab will open showing your live application!
