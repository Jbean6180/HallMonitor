import discord
from discord.ext import commands, tasks
from discord.voice_client import VoiceClient
import youtube_dl
import os, shutil
import uuid
import requests
from random import choice


client = commands.Bot(command_prefix='?',intents = discord.Intents.all(),case_insensitive=True)


status = ['You!','Dash Parr','that ass!']


@client.event
async def on_ready():
    change_status.start()
    print('Bot is online!')

@client.event
async def on_message(message):
    rules = [
        '#1  NO Mistakes',
        '#2  NO weird noises until 12:00 AM EST',
        '#3  NO weird questions until 12:00 AM EST',
        '#4  "None of that"',
        '#5  NO burping in VC',
        '#6  NO slurping',
        '#7  No Heavy breathing',
        '#8  NO Bitching about the rules',
        '#9  NO Fucking da rules',
        '#10 NO Masturbating in the VC',
        '#11 NO Simping',
        '#12 NO "Cummies"',
        '#13 NO Free Clout',
        '#14 NO Spoiling',
    ]
    if message.content.startswith("?rule 01"):
        await message.channel.send(rules[0])
    elif message.content.startswith("?rule 2"):
        await message.channel.send(rules[1])
    elif message.content.startswith("?rule 3"):
        await message.channel.send(rules[2])
    elif message.content.startswith("?rule 4"):
        await message.channel.send(rules[3])
    elif message.content.startswith("?rule 5"):
        await message.channel.send(rules[4])
    elif message.content.startswith("?rule 6"):
        await message.channel.send(rules[5])
    elif message.content.startswith("?rule 7"):
        await message.channel.send(rules[6])
    elif message.content.startswith("?rule 8"):
        await message.channel.send(rules[7])
    elif message.content.startswith("?rule 9"):
        await message.channel.send(rules[8])
    elif message.content.startswith("?rule 10"):
        await message.channel.send(rules[9])
    elif message.content.startswith("?rule 11"):
        await message.channel.send(rules[10])
    elif message.content.startswith("?rule 12"):
        await message.channel.send(rules[11])
    elif message.content.startswith("?rule 13"):
        await message.channel.send(rules[12])
    elif message.content.startswith("?rule 14"):
        await message.channel.send(rules[13])
    elif message.content.startswith("?rule"):
        await message.channel.send("Nigga that isn't a rule.")
    

@tasks.loop(seconds=20)
async def change_status():
    activity = discord.Activity(type=discord.ActivityType.watching, name = (choice(status)))
    await client.change_presence(activity=activity)


client.run("DISCORD-BOT-TOKEN")






