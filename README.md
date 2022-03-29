# spotted-bot-dc
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

CREATED BY: Abstergo using Discord Bot Maker

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
IMPORTANT: READ THIS BEFORE RUNNING BOT OR ADIING IT TO SERVER
#################################################################################################
INTRODUCTION

This is bot that creates spotted infrascturcture on your dc channel
when it joins it creates 3 channels

1. Post channel 	- people can send their messages here, it gets deleted as soon as it appears on channel
			- if someone wants to attach image to this file he has to type 'img' in his message, also please don't dype it if not attaching any image
			- you cant attach any other files
			- bot will be sending message 'Have you muted this channel?' every 15 minutes and delete them soon after, so user who didn't mute this channel will be constantly getting notifications

2. Spotted channel	- bot sends here anonymous messages sent by users

3. Logs channel		- only administrator can see this channel
			- here are gathered logs of spotted such as author and his message including attachment
			- this is your only way to punish trolls
#################################################################################################
Other commands

!rc - recreates post, logs and spotted channel (in case of admin betrayal)(recreated channel doesn't contain previous messages)

!cl x y - in other words clean message - it may happen that mute reminder will not be deleted so with this command you can delete bulk messages, x means number of messages to dele on post, and y on nsfw (read further to understand nsfw channel)

!nsfw - its addon that creates spotted nsfw channels
####################################################################################################
!nsfw addon

Creates two channels and one role:
1. nsfw channel - its just like post but for nsfw materials (hidden for every one without role)
2. nsfw spotted channel - just like spotted but for nsfw materials (hidden for every one without role)
3. nsfw spotter role - eneables people to nsfw addon's channel
###################################################################################################
Configuring your bot:

Since only polish version of this bot is hosted by me (no you cant get the link for it)
you have to host it yourself
1. enter https://discord.com/developers/applications
2. create your bott aplication
3. find app id and bot token
4. open 'bot directory'/data/settings.json
5. insert previously gathered data in indicated fields
6. save file
####################################################################################################
Run your bot

1 method on your computer (your computer has to be constantly working for this bot to be running)

- install node.js and open it
- type node 'bot directory'/bot.js
- done
- add bot to your server

2 method on heroku (free)
- create Procfile and put it in bot's directory
- in procfile type 'worker: node bot.js'
- deploy bot to heroku
- change dyno formation to worker 
- add bot to your server
- done

YOU HAVE TO RUN BOT FIRST AND THEN ADD IT TO SERVER OR CHANNELS WON'T BE CRAETED

To add bot to your server insert this url in your web browser: https://discordapp.com/oauth2/authorize?client_id='your application id'&scope=bot&permissions=2146958591
################################################################################################################

Youre welcome to insert your own changes to this bot but it was created using Discord Bot Maker so it might be really hard to do without this tool, 
Any true programmer should rather try writting his own bot from scratch.

####################################################################################################################