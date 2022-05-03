# spotted-bot-dc
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

CREATED BY: Abstergo using Discord Bot Maker

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
IMPORTANT: READ THIS BEFORE RUNNING BOT OR ADIING IT TO SERVER
#################################################################################################
INTRODUCTION

This is bot that creates spotted infrascturcture on your dc server
when it joins it creates 2 channels and 1 role

1. Spotted channel	- bot sends here anonymous messages after command /spotted was used by member

2. Logs channel		- only administrator can see this channel
			- here are gathered logs of spotted such as author and his message including attachment
			- this is your only way to punish trolls
3. Damn Troll role	- as any one on server can use spotted bot creates role to mark users banned from using spotted (both of them)
#################################################################################################
Other commands

/rc - recreates post, logs and spotted channel (in case of admin betrayal)(recreated channel doesn't contain previous messages)

/cl - in other words clean message - it may happen that mute reminder will not be deleted so with this command you can delete bulk messages

/nsfw - its addon that creates spotted nsfw channels
####################################################################################################
/nsfw addon

Creates one channel and one role:
1. nsfw channel - its just like spotted but for nsfw materials (hidden for every one without role)
2. nsfw spotter role - eneables people to use nsfw addon's channel (decide yourself who should have it)
###################################################################################################
Configuring your bot:

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

To add bot to your server insert this url in your web browser: https://discord.com/api/oauth2/authorize?client_id=YOUR BOT APP ID&permissions=8&scope=bot%20applications.commands
################################################################################################################

Youre welcome to insert your own changes to this bot but it was created using Discord Bot Maker so it might be really hard to do without this tool, 
Any true programmer should rather try writting his own bot from scratch.

####################################################################################################################
