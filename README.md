📧 Email Automation with n8n, Gmail & OpenAI

This project demonstrates an automated email processing workflow built with n8n, integrating Gmail, OpenAI, and Google Sheets.
The workflow automatically filters, classifies, and processes emails based on their content, then takes actions such as labeling, marking as read, storing in sheets, or preparing drafts.

⚡ Workflow Overview

Gmail Trigger

Starts when a new email arrives in the Gmail inbox.

Text Classifier (OpenAI Model)

Uses OpenAI’s text model to classify the incoming email content into categories.

Conditional Branches & Labels

Based on classification, labels are applied to emails (e.g., Important, Promotions, Spam, etc.).

Emails can also be marked as Read automatically.

Message Processing (OpenAI)

Email body is passed through OpenAI for generating structured responses.

Example actions include:

Extracting important details.

Drafting auto-replies.

Summarizing long emails.

Google Sheets Integration

Extracted data from emails is appended/updated in a Google Sheet for record-keeping or analytics.

Draft Creation in Gmail

Automatically prepares a draft email reply based on processed content.

🔑 Features

✅ Automatic classification of incoming emails.

✅ Add custom Gmail labels for better organization.

✅ Mark selected emails as read.

✅ Store important details in Google Sheets.

✅ Auto-generate draft replies using OpenAI.

✅ Fully customizable workflow in n8n.

🛠️ Tech Stack

n8n – Workflow automation platform.

Gmail API – For fetching and sending emails.

OpenAI API – For email classification & drafting.

Google Sheets API – For structured data storage.

🚀 Getting Started
1. Clone this repository
git clone https://github.com/your-username/email-automation-n8n.git
cd email-automation-n8n

2. Install n8n

Follow the official docs: n8n installation guide

3. Setup Environment Variables

Configure API keys for Gmail, Google Sheets, and OpenAI in your n8n environment.

GMAIL_CLIENT_ID=your_client_id
GMAIL_CLIENT_SECRET=your_client_secret
OPENAI_API_KEY=your_openai_api_key
GOOGLE_SHEETS_CREDENTIALS=your_sheets_credentials

4. Import Workflow

Open n8n dashboard.

Import the provided workflow JSON (exported from this project).

Connect your Gmail, OpenAI, and Google Sheets credentials.

5. Run Workflow

Activate the workflow.

Incoming emails will now be automatically classified, labeled, stored, and drafted.

📊 Example Use Cases

Auto-labeling work vs. personal emails.

Summarizing long reports into short notes.

Tracking client inquiries in Google Sheets.

Preparing instant draft responses to common queries.

📌 Notes

This is a demo project – customize according to your needs.

Ensure correct OAuth permissions for Gmail & Sheets.

Fine-tune the OpenAI prompts for better classification/drafts.

📜 License

MIT License © 2025
