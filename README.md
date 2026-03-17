# AI-Data-Analyzer
# AI Data Analyzer (Telegram Bot using n8n)

## Project Description

AI Data Analyzer is an intelligent Telegram-based chatbot built using n8n that processes user queries and retrieves relevant data from Google Sheets. It uses an AI model to interpret input and generate meaningful, data-driven responses in real time.

This project demonstrates how AI can be integrated with workflow automation tools to build smart and interactive data analysis systems.

---

## Features

* Real-time message handling through Telegram
* AI-based query understanding and response generation
* Integration with Google Sheets for live data retrieval
* Context-aware conversation using memory
* Fully automated workflow using n8n

---

## Workflow Architecture

```
Telegram Trigger → AI Agent → (Memory + Google Sheets Tool) → Telegram Response
```

---

## Workflow Explanation

### Telegram Trigger

Captures incoming messages from Telegram and initiates the workflow.

### AI Agent

Processes user queries using an AI model and connects with memory and external tools.

### Memory Node

Stores previous interactions to maintain conversational context.

### Google Sheets Node

Fetches structured data based on user queries for analysis.

### Telegram Send Message

Sends the processed response back to the user.

---

## Tech Stack

* n8n (workflow automation)
* Telegram Bot API
* OpenRouter API (AI model integration)
* Google Sheets API

---

## Setup Instructions

### Install n8n

```bash
npm install -g n8n
```

### Run n8n

```bash
n8n
```

Access the editor at: http://localhost:5678

---

### Import Workflow

* Open n8n editor
* Click "Import"
* Upload the workflow.json file

---

### Configure Credentials

#### Telegram Bot

* Create a bot using BotFather
* Copy the bot token
* Add it in n8n credentials

#### OpenRouter API

* Generate an API key
* Add it to the AI model node

#### Google Sheets

* Connect your Google account
* Provide the Sheet ID
* Configure access permissions

---

### Activate Workflow

* Activate the workflow in n8n
* Send a message to your Telegram bot
* The bot will respond with analyzed data

---

## Project Structure

```
.
├── workflow.json
├── README.md
```

---

## Use Cases

* Sales and business data analysis
* Automated reporting assistant
* Student or academic data queries
* FAQ and decision-support chatbot

---

## Future Improvements

* Data visualization integration
* Support for databases like MySQL or MongoDB
* Multi-user handling
* Voice input processing

---

## Security Notes

* Do not upload API keys or credentials
* Use environment variables for sensitive data

---

## Project Impact

This project demonstrates practical implementation of AI with automation tools, enabling real-time data-driven decision making through conversational interfaces.

---

## Contribution

Contributions are welcome. Feel free to fork the repository and submit improvements.

---

## License

This project is licensed under the MIT License.

---

## Author

Your Name
https://github.com/your-username
