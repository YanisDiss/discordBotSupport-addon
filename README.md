# Discord Bot Support Addon
This is an APS++ Addon that adds the possibility to manage and control your game with a discord bot. You need to have a basic understanding of the discord developer portal in order to set up your own bot and use this addon. Let me know if you find any bugs.
# Setup Guide

## Prerequisites
You need a discord server with the following:
- a channel for your logs
- a channel for your ingame chat
- a channel for bot commands
- a Developer role
- an Owner role
- a basic Member role
- a Muted role

## Creating the bot
- Go in the [Discord Developer Portal](https://discord.com/developers/applications), and create a new Application (call it whatever you want)
- You can edit your application's info in the **General Information** 

## Inviting it to your server
- After doing the above, go in the **OAuth2** section > **URL Generator**
- Set the scopes to **bot** and the permissions to **Administrator**
- It will give you a link to invite the bot. Choose the server you want your bot to be in and voila ! 

## Connecting it
- Go in the **bot** section of your application and click Reset token, it will give you the token of your discord bot Copy it in your clipboard.
- After that, go in **.env** in your game and add in here `BOT_TOKEN=thetokenyoupasted`
- For the next steps, you need to enable Developer mode on discord, and you do it by going in **Options** > **Advanced** > **Developer Mode**

## Setting it up
- Put the discordBotSupport addon in server/modules/definitions/addons
- Search for `toedit` and change all the variables marked with it in the addon (with developer mode, right click to copy IDs of roles and channels.)
- Before launching the server , You need the eris module for the bot to work, Install it by doing `npm install -f eris` in the terminal.
- if you see a `server initialized: bot is ready for use` in your logs channel, your bot is working. GG!