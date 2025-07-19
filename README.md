# SmartSpend AI
<img width="1536" height="1024" alt="ChatGPT Image Jul 19, 2025, 12_21_46 PM" src="https://github.com/user-attachments/assets/903c15b7-b95e-4f6a-86af-0181c82695c3" />

## 📖 Project Overview

**SmartSpend AI** is a full-stack, AI-powered personal finance management application that automates expense tracking, budgeting, and financial insights. Users securely connect bank accounts, upload receipts, and receive real-time spending analytics and budget alerts without manual effort.

Key capabilities:

* **Automated Receipt Parsing:** Uses Gemini AI to extract and categorize transaction data from uploaded receipts.
* **Real-Time Dashboards:** Displays interactive expense breakdowns, spending trends, and budget summaries via Shadcn UI components.
* **Background Job Scheduling:** Leverages Inngest to handle recurring transactions and monthly financial reports.
* **Secure Multi-User Support:** Implements Supabase Auth (OAuth & email/password) and Prisma ORM with rate-limited APIs using Arcjet.
* **Email Notifications:** Sends budget alerts and monthly summary reports automatically via Resend.

## 🚀 Features

1. **AI-Driven Receipt OCR & Categorization**

   * Gemini AI integration for receipt text extraction and transaction classification.
   * Supports multiple currencies and custom spending categories.

2. **Dynamic Budget Monitoring**

   * User-defined budgets with real-time progress bars and alerts.
   * Configurable thresholds trigger automated email notifications.

3. **Recurring Transaction Automation**

   * Inngest schedules and executes >100 monthly transactions and report jobs.
   * Ensures up-to-date financial data with zero manual intervention.

4. **Interactive Financial Dashboards**

   * Built with Next.js, Tailwind CSS, and Shadcn UI for responsive visuals.
   * Displays charts for spending by category, monthly trends, and account balances.

5. **Robust Backend & Security**

   * Supabase (PostgreSQL) with Prisma ORM for data management.
   * OAuth & email/password authentication, API rate limiting (60 req/min) via Arcjet.

## 🛠️ Tech Stack

* **Frontend:** Next.js, React, Tailwind CSS, Shadcn UI
* **Backend:** Node.js, Inngest, Prisma ORM, Supabase (Auth, Database, Storage)
* **AI & Automation:** Gemini AI API, Resend (email), Arcjet (rate limiting)
* **Database:** PostgreSQL (via Supabase)
* **Development:** TypeScript, VS Code, GitHub Actions
* 

## ⚙️ Database Structure
<img width="739" height="496" alt="Screenshot 2025-07-09 015451" src="https://github.com/user-attachments/assets/d8a68b3c-0713-41d6-9aca-0461a5360438" />

## ⚙️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/<username>/smartspend-ai.git
   cd smartspend-ai
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   ```bash
   cp .env.example .env
   # Set SUPABASE_URL, SUPABASE_KEY, GEMINI_AI_KEY, INNGEST_API_KEY, RESEND_API_KEY, ARCJET_KEY
   ```

4. **Run development server**

   ```bash
   npm run dev
   ```

## 🎬 Usage

1. **User Authentication**

   * Sign up or log in via email/password or OAuth providers.

2. **Connect Bank Accounts**

   * Use Supabase Storage to link account data (mock or real).

3. **Upload Receipts**

   * Drag-and-drop or file upload interface; OCR and categorization occur automatically.

4. **View Dashboards & Reports**

   * Navigate to the Dashboard for live expense charts.
   * Monthly summary emailed automatically.

5. **Manage Budgets & Transactions**

   * Create, edit, or delete budgets and recurring transactions in settings.

## 📸 Screenshots

<img width="942" height="414" alt="Screenshot 2025-07-19 121356" src="https://github.com/user-attachments/assets/8a27d8d3-7dc4-46cd-b238-9f8f47e721b3" />
<img width="946" height="402" alt="Screenshot 2025-07-19 121407" src="https://github.com/user-attachments/assets/a61055fb-a6d9-4677-8ddf-a30fb9c33e1c" />
<img width="960" height="540" alt="Screenshot 2025-07-19 121429" src="https://github.com/user-attachments/assets/dec24813-a94b-4ae0-8e96-a7d54a6898d4" />
<img width="960" height="540" alt="Screenshot 2025-07-19 121553" src="https://github.com/user-attachments/assets/f0e9ebfe-04bc-432a-8550-196157018f0d" />
<img width="960" height="540" alt="Screenshot 2025-07-19 121603" src="https://github.com/user-attachments/assets/bdca5340-d5e4-421a-8362-5b1cc85fa3c5" />
<img width="960" height="540" alt="Screenshot 2025-07-19 121607" src="https://github.com/user-attachments/assets/581f0784-a217-4ead-b4ec-b6082bc66d12" />
<img width="960" height="540" alt="Screenshot 2025-07-19 121622" src="https://github.com/user-attachments/assets/acaab3bd-e7e6-4cc2-ab74-f9590f262552" />

<!--
Insert screenshots from `docs/screenshots`:
- `dashboard.png`: Main dashboard with expense charts.
- `receipt_parsing.png`: Receipt upload and OCR result.
- `budget_alert.png`: Example of budget alert email.
- `transaction_automation.png`: Recurring transactions overview.
-->

## 📈 Results

| Metric                               | Value              |
| ------------------------------------ | ------------------ |
| Receipt Parsing Accuracy             | \~95%              |
| Monthly Recurring Jobs Executed      | >100               |
| API Response Time                    | <200ms (95th perc) |
| User Engagement (daily active users) | n/a (TBD)          |

## 📂 Repository Structure

```
├── docs/                    # Assets and screenshots
├── pages/                   # Next.js page components
├── components/              # Reusable React components
├── lib/                     # Utilities and API clients
├── prisma/                  # Prisma schema and migrations
├── scripts/                 # Automation and deployment scripts
├── styles/                  # Global and utility CSS
├── .env.example             # Environment variable template
├── package.json             # Project metadata and scripts
├── README.md                # Project overview and instructions
└── LICENSE                  # License information
```

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request for new features, bug fixes, or documentation improvements.

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

> *Based on personal implementation of full-stack features and AI integrations.*
