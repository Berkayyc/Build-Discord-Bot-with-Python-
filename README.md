# Build-Discord-Bot-with-Python-
"A fun and lightweight Discord bot built with Python that serves random memes and greets users."

# 🤖 Discord Meme & Greet Bot

A fun and lightweight Discord bot built with Python (`discord.py`) and the `requests` library that instantly sends random memes to your server and greets users.

This is a great foundational project to understand the logic of fetching data from a public API (HTTP requests) and interacting with the Discord API.

## ✨ Features and Commands

The bot currently supports two basic commands:

* **`$hello`** : When you greet the bot, it instantly replies with "Hello World!". Ideal for testing if the bot is online and responsive.
* **`$meme`** : Fetches a random and funny meme image in real-time from `meme-api.com` and sends it to the server.

## 🛠️ Technologies Used

* **Python 3.x:** Main programming language.
* **discord.py:** Used to communicate with the Discord API and handle bot events.
* **requests & json:** Used to fetch and parse data from an external API on the internet.

## 🚀 Setup and Run

To run the bot on your local machine or server, follow these steps:

### 1. Prerequisites
Ensure Python is installed on your computer. Then, run the following command in your terminal (or command prompt) to install the required libraries:
\`\`\`bash
pip install discord.py requests
\`\`\`

### 2. Discord Developer Settings
1. Go to the [Discord Developer Portal](https://discord.com/developers/applications) and create a new application (bot).
2. Copy your bot's **Token**.
3. Under the Bot settings tab, make sure to toggle on the **"Message Content Intent"** under Privileged Gateway Intents (Otherwise, the bot won't be able to read messages).

### 3. Editing the Code
Open the `bot.py` file in your project folder. Locate the last line and replace `Your Token Here` with your actual bot token, keeping the quotation marks:
\`\`\`python
client.run('YOUR_ACTUAL_TOKEN_HERE')
\`\`\`

### 4. Starting the Bot
Open your terminal, navigate to the folder where your project is located, and run the bot:
\`\`\`bash
python bot.py
\`\`\`
Once you see `Logged on as BotName#1234!` in your console, your bot is ready to use! Go to your Discord server and type `$meme` to test it out.
