## AI Email Assistant (Personal Project)

A personal project built in n8n (v8.10) that automates email responses in Gmail. This assistant drafts and replies to emails using AI, ensuring each response is professional, respectful, and open, directly from the content of incoming messages.

#🛠 Features

Gmail Trigger: Automatically detects unread emails in your Gmail account.

AI Email Drafting: Uses a combination of LangChain and Google Gemini AI to generate professional replies.

Automated Responses: Creates drafts or replies directly in Gmail while keeping responses personalized and respectful.

Configurable: Easy to update prompts and AI parameters for different email tones or workflows.

#⚡ How It Works

# Trigger:
The workflow monitors your Gmail inbox for unread messages every minute.

# AI Assistant:
The AI assistant reads the snippet of the incoming email and generates a professional response using:

LangChain agent node

Google Gemini Chat Model

# Gmail Actions:
The generated response can:

Create a draft in Gmail

Reply to the message automatically (optional)

Flow Overview:

Gmail Trigger → Email Assistant → (Create Draft in Gmail / Reply to Message)
                      ↑
         Google Gemini Chat Model

⚙️ Setup

Clone the repository:

git clone https://github.com/iamkeithaustria/your-repo-name.git
cd your-repo-name


# Import Workflow in n8n:

Open n8n, click Import from JSON, and select the workflow JSON.

Set Up Credentials:

Configure your Gmail OAuth2 account.

Configure Google Gemini API credentials.

# Activate Workflow:

Start the workflow to monitor your Gmail inbox and automatically draft/reply to emails.

# 📝 Usage Tips

Adjust the prompt in the Email Assistant node to change the tone (formal, friendly, concise, etc.).

Use Gmail’s draft mode first to review AI-generated emails before sending automatically.

Ensure your API keys and credentials are correctly set to avoid failures.

# 🔒 Security

All credentials (Gmail OAuth2, Google Gemini API) are stored in n8n and not shared in the workflow JSON.

The workflow only processes emails in your Gmail account and doesn’t store emails outside your configured nodes.

# 📂 Workflow Nodes
Node Name	Function
Gmail Trigger	Detect unread emails
Email Assistant (LangChain)	Generate professional email drafts
Google Gemini Chat Model	AI language model for content generation
Reply to a Message in Gmail	Sends AI-generated replies directly
Create a Draft in Gmail	Saves AI-generated email as a draft

# 🔗 GitHub

https://github.com/iamkeithaustria
