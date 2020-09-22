
# NewDiscordBridge

NewDiscordBridge is a new plugin that will allow you not only to exchange messages with a chat on your server, but also
moderate directly from discord!

This is a modified fork of the original repo <https://github.com/Mortmael/NewDiscordBridge>. This fork adds new config options
for better customization and control of the Discord Bot account.

Supports: [Original TShock](https://github.com/Pryaxis/TShock), [Mobile TShock](https://github.com/Fe7n/TShockMobile)

## Commands
* **ban <player/IP> \<time> [reason]** - ban user or ip. **Requires the ban permission!**
	* **unban <player/IP>**
* **kick \<player> [reason]** - kicks the player.  **Requires the kick permission!**
* **mute \<player>** - mute/unmute player.  **Requires the mute permission!**
* **off** - shuts down the server while saving.  **Requires the administrator permission!**
* **info <player/IP>** - shows information about the player's account or IP.
* **who** - displays a list of players.

## Config (NewDiscordBridge.json)
Name | Description | Type
:----|:------------|:----
DiscordBotToken | Insert the token for your bot from the [Developer Portal](https://discord.com/developers/) here | String
Prefix | Prefix for your commands, e. g. "/", or "bot-" | String
Playing | "Playing" status for Discord Bot | String
Chat | Enable if you need chat between server and discord | Boolean
AllowBots | Whether or not bot messages should send to the Terraria server | Boolean
Commands | Enable if you need commands | Boolean
ChatID | ID of channel for chat | UInt64
LogID | ID of channel for logs | UInt64
JoinLogID | ID of channel for join/leave messages | UInt64
DiscordToTerrariaFormat | Format of messages from discord. <br/>*{0} - Username, {1} - Message* | String
TerrariaToDiscordFormat | Format of messages from server. <br/>*{0} - Prefix, {1} - Username, {2} - Suffix, {3} - Message* | String
Messagecolor | RGB color for messages from discord | Int32[]
