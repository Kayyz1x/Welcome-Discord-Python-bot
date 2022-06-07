import discord
from discord.ext import commands
from discord.utils import get
import time
from time import sleep
import json
import asyncio
import requests
import datetime
import aiohttp
import random
#intents = discord.Intents(messages=True, members = True, guilds=True)
intents = discord.Intents().all()
bot = commands.Bot(command_prefix="!", intents=intents, help_command=None)


@bot.event
async def on_ready():  
    print("Online")

@bot.event
async def on_member_join(member):
    embedVar = discord.Embed(author="Kayyz", description=f"{member.mention} Willkommen auf Latest-V", color=0x4f42b5)
    await bot.get_channel(980889299975295109).send(embed=embedVar)
@bot.event
async def on_member_remove(member):
    embedVar = discord.Embed(author="Kayyz", description=f"{member.mention} hat den server verlassen.", color=0x4f42b5)
    await bot.get_channel(979467832305782786).send(embed=embedVar)


bot.run("token")
