# 🤖 Daily AI News Email Automation

An automated AI news digest built using **n8n, Apify, Reddit API, and Gmail**. This workflow collects the top AI-related posts from Reddit every morning and delivers them directly to your inbox.

## 🚀 Project Overview

Keeping up with the latest developments in Artificial Intelligence can be time-consuming.

This project automates the process by collecting the top daily AI posts from Reddit and sending them as an organized email digest every morning at 8:00 AM (Dubai Time).

## ⚙️ Workflow Architecture

**Automation Flow:**

Schedule Trigger → Apify Reddit Scraper → Gmail Email Delivery

### Workflow Nodes

| Node | Function |
|---|---|
| Every Morning 8AM | Triggers the workflow daily at 8 AM |
| Get Reddit AI Posts | Fetches the top 5 daily posts from r/artificial using Apify |
| Send AI News Email | Sends the collected AI news to Gmail |

## 🛠️ Tech Stack

- **n8n Cloud** – Workflow automation
- **Apify** – Reddit data extraction
- **Reddit** – AI news source (r/artificial)
- **Gmail** – Automated email delivery
- **JSON** – Workflow export and configuration

## 🔄 How It Works

1. The Schedule Trigger starts the workflow every morning at 8:00 AM.
2. The HTTP Request node connects to the Apify Reddit Scraper Lite actor.
3. The scraper collects up to 5 top posts from Reddit's r/artificial daily feed.
4. The Gmail node processes the post titles and URLs.
5. An HTML-formatted email containing the AI news links is delivered to the configured inbox.

## 📂 Project Structure

```text
n8n-daily-ai-news-automation/
│
├── workflows/
│   └── daily-ai-news-email.json
│
├── screenshots/
│   └── workflow-overview.png
│
├── README.md
└── .gitignore
```

## ⚡ Setup Instructions

### Prerequisites

- n8n Cloud account
- Apify account
- Gmail account

### Installation

1. Clone or download this repository.
2. Open your n8n workspace.
3. Import `workflows/daily-ai-news-email.json`.
4. Configure your Apify API credentials.
5. Connect your Gmail OAuth2 account.
6. Update the recipient email address.
7. Set the workflow timezone to `Asia/Dubai`.
8. Execute the workflow manually to test it.
9. Activate the workflow after successful testing.

## 🔐 Security

- API credentials are not included in this repository.
- Gmail OAuth2 credentials must be configured securely inside n8n.
- Never expose API tokens, passwords, or authentication credentials.
- Configure your own recipient email address after importing the workflow.

## 🎯 Key Features

- Daily automated AI news collection
- Reddit AI community monitoring
- Apify-powered web data extraction
- Automated Gmail notifications
- Scheduled execution at 8 AM Dubai time
- No manual daily news searching required

## 📌 Future Improvements

- Add multiple AI-related Reddit communities.
- Integrate AI summarization using an LLM.
- Categorize news by AI, Machine Learning, Generative AI, and LLMs.
- Generate a daily HTML newsletter.
- Add Telegram notifications.
- Store collected news in Google Sheets.

## 👩‍💻 Author

**Divya Anu Sri Valavala**

AI Engineer | Generative AI | Machine Learning | LLMs | Workflow Automation

GitHub: [@Vvanunagesh09](https://github.com/Vvanunagesh09)

---

⭐ If you find this project useful, consider giving this repository a star!

**Built with n8n to make staying updated with AI effortless.**
