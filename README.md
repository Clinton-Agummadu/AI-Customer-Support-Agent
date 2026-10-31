# n8n Telegram AI Agent

Autonomous customer service pipeline built on n8n using Google Gemini and Telegram Bot API.

## Workflow Overview
* **Trigger:** Telegram Webhook Event
* **Core Agent:** n8n AI Agent Node
* **Model:** Google Gemini Chat Model
* **State Management:** Simple Memory Node
* **Action:** Telegram `sendMessage` API Call

## Key Capabilities
* Zero-database setup with full menu and operational rules contained in the system prompt context.
* Enforces geographic restrictions (Lagos State 24-hour delivery window).
* Captures user order details (Name, Delivery Address, Items, Phone Number).

## Setup
1. Import workflow JSON into n8n.
2. Set Telegram and Gemini API credentials.
3. Configure `WEBHOOK_URL` environment variable for your n8n instance.
4. Activate workflow.
