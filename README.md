# Discord Ticket & Info Bot (Skript + DiSky)

A fully-featured Minecraft server utility and support ticket bot built using Skript and the DiSky add-on.

## Requirements
* **Minecraft Server:** Paper / Purpur (or any modern Spigot fork) 1.19+
* **Skript:** Version 2.10.0 or higher
* **DiSky:** Version 4.11.1 or higher

## Installation
1. Install **Skript** and **DiSky** into your server's `plugins` folder and restart the server.
2. Place the `bot.sk` script inside your `plugins/Skript/scripts/` directory.
3. Set up your configuration file or environment variables for your bot token securely (see below).

## Configuration
1. Copy `config.example.yml` to a secure configuration location or fill out your IDs directly at the top of `bot.sk`.
2. Insert your Discord IDs:
   * **Ticket Category ID**: The category channel where tickets will be spawned.
   * **Staff Role ID**: The role given permission to view tickets and assist players.
   * **Server Info Channel ID**: The text channel where `/serverinfo` posts server statistics.

## Security Warning
* **Never** commit your live bot token to GitHub. Use environment variables or local server configs. The `.gitignore` file provided ensures sensitive files are ignored.

## Usage & Commands
* `/setticketpanel` — Posts the interactive support ticket embed and dropdown menu.
* `/serverinfo` — Posts live server statistics (online players) to the designated channel.
* **Tickets:** Select any category from the dropdown menu to instantly spin up a private channel accessible only to you and the staff team.
