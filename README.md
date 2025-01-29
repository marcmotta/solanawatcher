# Solana Watcher

Solana Watcher is a simple Python script that monitors the price of Solana (SOL) and sends notifications via Telegram when the price crosses a specified threshold.

## Features

* Monitors the price of Solana (SOL) from a specified exchange (e.g., Binance).
* Sends notifications via Telegram when the price crosses a user-defined threshold.
* Configurable notification thresholds (both upper and lower).
* Simple and easy to use.

## Requirements

* Python 3.6 or higher
* Required Python libraries: `requests`, `python-telegram-bot`
* A Telegram bot token. You can obtain one by talking to the BotFather on Telegram.
* An API key for the exchange you want to use (e.g., Binance API key).

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/marcmotta/solanawatcher
Navigate to the project directory:

Bash

cd solanawatcher
Install the required dependencies:

Bash

pip install -r requirements.txt
Configuration
Create a .env file in the project directory.   

Add the following environment variables to the .env file:   

BINANCE_API_KEY=<YOUR_BINANCE_API_KEY>

BINANCE_API_SECRET=<YOUR_BINANCE_API_SECRET>

TELEGRAM_BOT_TOKEN=<YOUR_TELEGRAM_BOT_TOKEN>

TELEGRAM_CHAT_ID=<YOUR_TELEGRAM_CHAT_ID>

PRICE_THRESHOLD_UPPER=<UPPER_PRICE_THRESHOLD>

PRICE_THRESHOLD_LOWER=<LOWER_PRICE_THRESHOLD>

Replace <YOUR_BINANCE_API_KEY> and <YOUR_BINANCE_API_SECRET> with your actual Binance API key and secret.

Replace <YOUR_TELEGRAM_BOT_TOKEN> with your Telegram bot token.

Replace <YOUR_TELEGRAM_CHAT_ID> with your Telegram chat ID. You can use a bot to get it or find it in the Telegram group settings if it's for a group.

Replace <UPPER_PRICE_THRESHOLD> and <LOWER_PRICE_THRESHOLD> with the desired upper and lower price thresholds.

Usage

Run the script:

Bash

python solanawatcher.py

The script will start monitoring the price of Solana and send notifications via Telegram when the price crosses the defined thresholds.
