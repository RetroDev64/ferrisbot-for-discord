# Discord Mods Bot

## Inviting the bot

Some permissions are required:
- Send Messages: base command functionality
- Manage Roles: for `?rustify` command
- Manage Messages: for `?cleanup` command
- Add Reactions: for `?rustify` command feedback

The permissions integer for these four permissions is `268445760`.

Here's an invite link to an instance hosted by me on my Raspberry Pi:
https://discord.com/oauth2/authorize?client_id=804340127433752646&permissions=268445760&scope=bot

## Hosting the bot

Run the bot using `cargo run --release`. You will need to provide several environment variables:
- DISCORD_TOKEN: the Discord bot token acquired via the Discord Developer Portal
- MOD_ROLE_ID: the ID of the Moderator role on your Discord server

An example command-line for Linux would be:
`MOD_ROLE_ID=788427199761481799 DISCORD_TOKEN=... cargo run --release`
