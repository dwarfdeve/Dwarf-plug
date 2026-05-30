# Dwarf Plug Telegram Bot

This bot handles order processing, customer FAQs, and payment collection for the Dwarf Plug shop.

## Features
- **Order Parsing**: Automatically detects order summaries pasted from the website.
- **Shipping Collection**: Step-by-step flow to collect delivery details.
- **Payment Handling**: Support for BTC, ETH, XMR, and Gift Cards.
- **FAQ System**: Preset answers for Shipping, Quality, Tracking, etc.
- **Admin Dashboard**: Notifications for new orders and ability to update crypto addresses.

## Setup Instructions

### 1. Requirements
- Python 3.10+
- `python-telegram-bot` library

### 2. Installation
```bash
pip install python-telegram-bot --upgrade
```

### 3. Running the Bot
```bash
python bot.py
```

### 4. Admin Setup
1. Open the bot in Telegram.
2. Send the command `/start_admin` to register yourself as the seller.
3. Use `/set_address <COIN> <ADDRESS>` to update your payment addresses (e.g., `/set_address BTC bc1q...`).

## Usage Flow
1. Customer finishes browsing on the website.
2. Customer clicks "Submit Order", which copies the summary and opens this bot.
3. Customer pastes the summary into the bot.
4. Bot asks for shipping details.
5. Bot provides payment instructions.
6. Seller (Admin) receives a notification of the new order.
