# Discord Bot with Webhook & Role Management

## Overview

This is a simple Discord bot built using the `discord.js` library. It provides a few basic commands, such as `kick`, `ban`, and `announce`, along with role management features based on emoji reactions. The bot also sends announcements via a webhook and reacts to certain message reactions to assign or remove roles in the server.

## Features

- **Kick Command**: Kicks a member from the server.
- **Ban Command**: Bans a member from the server.
- **Announce Command**: Sends an announcement via a webhook.
- **Role Management**: Assigns roles based on emoji reactions to a specific message.

## Requirements

- Node.js
- `discord.js`
- `dotenv`
- Webhook setup in Discord

### Installation

1. Clone the repository.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add your `DISCORDJS_BOT_TOKEN` and `WEBHOOK_ID`, `WEBHOOK_TOKEN` values.
4. Start the bot:
   ```bash
   node index.js
   ```

## Commands

- `$kick <user_id>`: Kicks a user from the server (requires `KICK_MEMBERS` permission).
- `$ban <user_id>`: Bans a user from the server (requires `BAN_MEMBERS` permission).
- `$announce <message>`: Sends an announcement to a configured webhook.

## Role Management via Emoji Reactions

- Users can react to a specific message with emojis to receive roles:
  - 🍎 → Role 1
  - 🍋 → Role 2
  - 🍐 → Role 3
  - 🍑 → Role 4

