# ModMail-Lite
ModMailLite is a powerful yet lightweight Discord ModMail system that allows server members to contact staff through direct messages to the bot. It creates organized thread-based conversations, making it easy for staff to manage user inquiries, reports, and support requests.
> 💡 **Built for the Zygnal Ecosystem — to download and use this extension, you must be part of the Zygnal Ecosystem.**  
> This extension (cog) is part of the **Zygnal Ecosystem** and is only available through its supported platforms.  
> You can use it with:  
> - The **[Discord Bot Framework](https://github.com/TheHolyOneZ/discord-bot-framework)** — ideal for developers who want full control and flexibility *(includes an integrated extension marketplace)*, or  
> - The **[ZygnalBot](https://zygnalbot.de)** — a prebuilt, plug-and-play Discord bot *(also includes an integrated extension marketplace)*.  
>
> Browse and install extensions at [zygnalbot.com/extension](https://zygnalbot.com/extension).  
> For help or community discussions, join us on Discord: [discord.gg/sgZnXca5ts](https://discord.gg/sgZnXca5ts)
# ModMailLite

A lightweight, feature-rich ModMail system for Discord bots created by TheHolyOneZ.

## Description

ModMailLite is a powerful yet lightweight Discord ModMail system that allows server members to contact staff through direct messages to the bot. It creates organized thread-based conversations, making it easy for staff to manage user inquiries, reports, and support requests.

## Features

- **Thread-Based Communication**: Each user conversation creates a dedicated thread in your ModMail channel
- **Multi-Server Support**: Users can select which server to contact if the bot is in multiple servers
- **Staff Assignment**: Staff members can claim threads to avoid duplicate responses
- **Anonymous Mode**: Toggle between sending messages as yourself or anonymously as "Staff Team"
- **Exclusive Mode**: Restrict thread responses to only the assigned staff member
- **Thread Transfer**: Transfer ownership of a thread to another staff member
- **Conversation Export**: Export entire conversations to text files
- **Logging**: Optional logging of closed threads to a dedicated channel
- **User Blocking**: Block problematic users from using ModMail
- **Staff Notifications**: Ping a specific role when new threads are created
- **Persistent Storage**: Conversations persist through bot restarts

## Commands

### User Commands (DM only)
- `!report` - Start a new ModMail conversation
- `!cancel` - Cancel a pending report
- `!close` - Request to close your active conversation
- `!status` - Check if you have any active conversations
- `!help` - Show available commands

### Staff Commands
- `!modmail setup [#channel]` - Set up ModMail in a channel
- `!modmail claim` - Claim a ModMail thread
- `!modmail close [reason]` - Close a ModMail thread
- `!modmail anonymous <message>` - Send a one-time anonymous message
- `!modmail anonymous_mode` - Toggle anonymous mode for all messages
- `!modmail exclusive_mode` - Toggle exclusive mode (only assigned staff can reply)
- `!modmail transfer @member` - Transfer thread to another staff member
- `!modmail export` - Export the current thread
- `!modmail status` - Show ModMail status
- `!modmail logs [#channel]` - Set a channel for ModMail logs
- `!modmail staffrole @role` - Set a staff role to be pinged for new threads
- `!modmail block <user_id> [reason]` - Block a user from using ModMail
- `!modmail unblock <user_id>` - Unblock a user
- `!modmail blocklist` - Show all blocked users
- `!modmail cleanup` - Clean up invalid threads
- `!modmail debug` - Debug active threads (admin only)

## Installation

1. Place the `modmail_lite.py` file in your bot's extensions folder
2. Load the extension in your bot:
   ```python
   bot.load_extension("extensions.modmail_lite")
   ```
3. Use `!modmail setup #channel` in your server to set up ModMail

## Configuration

ModMailLite automatically creates and manages two configuration files:
- `data/TheZModMail/modmail_config.json` - Stores server-specific settings
- `data/TheZModMail/modmail_threads.json` - Stores active thread information


## Credits

Created by TheHolyOneZ

---

