# One Tip Bot

This bot will be used to Tip Members using Telegram Channel and Twitter

Following dendencies needs to be installed for running this bot.

## Needs to install MongoDB, please following below link to install MongoDB

> https://www.digitalocean.com/community/tutorials/how-to-install-mongodb-on-ubuntu-20-04

## Python
> pip3 install pyhmy

> pip3 install pymongo

> pip3 install python-telegram-bot

> pip3 install telethon

> pip3 install qrcode

> pip3 install Image

## Need to install hmy binary

Create hmydir directory under main directory and download the hmy binary

> https://docs.harmony.one/home/wallets/harmony-cli/download-setup

## Node JS needs be installed on the machine, please follow below link to instal Node

> https://nodejs.org/en/download/package-manager/

## Node 
> sudo npm install twitter-autohook --save

Please check following link for more detail on Twitter Autohook

> https://github.com/twitterdev/autohook

Get Auth token from NGROK
> https://dashboard.ngrok.com/signup

> sudo npm install mongoose

## Api Keys

- Go to the following and create a new app: https://developer.twitter.com/en/portal/apps/
- Go to the settings of app created above and change app permissions to "Read, Write, and Direct Messages".
- In the navigation panel go to Products -> Premium -> Dev Environment and setup "Account Activity APISandbox".
- Put all the api keys in the secret.js and secret.py file.
- TWITTER_WEBHOOK_ENV refers to the Dev environment label in twitter API dashboard
- In Twitter > More > Settings > Privacy and Safety > Direct Messages , tick "Allow message requests from everyone"
- Change bot_name, twitter_bot_name, twitter_bot_handle in telegramtipbot.py 
- Change twitter_uid, bot_twitter_handle in twittertipbot.py
- Change _networkUrl in hmyclient.py to point to production
- Change explorer_url in telegramtipbot.py and twittertipbot.py  to point to production
- Change botTwitterId,botHandle variables in  twitter_autohook.js

## Running the Bot
> tmux new-session -s python

> python3 onetipbot.py

> Ctrl-B and D

> tmux new-session -s node

> node twitter_autohook.js

> Ctrl-B and D

# You can attached to a session to close or run by 

> tmux attach-session -t session-name
