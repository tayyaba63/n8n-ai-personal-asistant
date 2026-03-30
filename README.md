 AI Personal Assistant Workflow (n8n)

-> Overview

This project is an " AI-powered Personal Assistant built using n8n ".
It automates daily tasks like managing emails, scheduling events, tracking expenses, and handling notes — all through a single intelligent workflow.

The assistant understands user input, decides the correct action, and uses integrated tools to complete tasks efficiently.



-> Features

🔍 Information & Web Search
* Fetch real-time information using Google Search
* Answer general queries intelligently

📅 Calendar Management
* Create calendar events
* Get single or multiple events
* Manage schedules بسهولة

📧 Email Automation (Gmail)
* Read emails
* Fetch multiple messages
* Send or reply to emails automatically

📝 Notes & Task Management
* Create tasks
* Fetch tasks
* Delete completed tasks

📊 Expense Tracking
* Add expenses to Google Sheets
* Retrieve expense records
* Perform calculations using built-in calculator

🧠 AI-Powered Decision Making
* Uses AI Agent to understand user intent
* Automatically selects the correct tool
* Maintains conversation memory



-> Workflow Architecture:
The workflow follows this structure:

User Request → Webhook → AI Agent → Tool Selection → Action Execution → Response

1. Webhook Trigger
   * Receives user input (message)

2. AI Agent
   * Understands intent
   * Decides which tool to use

3. Memory Buffer
   * Stores conversation context

4. Tool Execution:
   * Google Calendar
   * Gmail
   * Google Sheets
   * Google Tasks
   * Web Search
   * Calculator

5. Response Node
   * Sends output back to user

⚙️ Technologies Used:
* n8n – Workflow automation
* Google Gemini (LLM) – AI reasoning
* SerpAPI – Web search
* Google Services:
  * Gmail API
  * Google Calendar API
  * Google Sheets API
  * Google Tasks API



-> Setup Instructions

1. Import Workflow
* Download the JSON file
* Open n8n
* Click **Import Workflow**
* Upload the file

2. Configure Credentials
Connect the following services:
* Google Calendar
* Gmail
* Google Sheets
* Google Tasks
* SerpAPI
* Google Gemini API


3. Activate Workflow
* Turn ON the workflow in n8n


4. Use Webhook
Send a POST request to:

```
/webhook/bc1054f6-7836-4704-a858-7f60ca88c478
```

Example request body:

```json
{
  "msg": "Schedule a meeting tomorrow at 5 PM"
}
```

-> Example Use Cases

* "Schedule a meeting tomorrow"
* "Show my emails"
* "Add expense: Food 500"
* "What is the weather today?"
* "Create a task: Complete assignment"


-> Notes & Best Practices

* Ensure all APIs are properly authenticated
* Do not expose API keys publicly
* Confirm destructive actions (like deleting tasks)


-> Future Improvements

* WhatsApp / Telegram integration
* Voice assistant support
* Advanced analytics dashboard
* Multi-user support


-> Author: **Tayyaba**


⭐ Support
If you like this project:
* Give it a ⭐ on GitHub
* Share with others


-> License

This project is open-source and free to use.
