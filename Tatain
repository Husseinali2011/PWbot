import discord
from discord.ext import commands

# Bot configuration
TOKEN = 'MTM0NTQ2MjIwMzgyMTcxOTY5NA.GADjGK.74j_KUx_I1YHwTK1w5zvrnLIp4D6nHqLZbfe08'
intents = discord.Intents.default()
intents.messages = True
intents.guilds = True
intents.members = True
bot = commands.Bot(command_prefix='/titan ', intents=intents)

# Basic command example
@bot.event
async def on_ready():
    print(f'Logged in as {bot.user}')

@bot.command()
async def register(ctx):
    await ctx.send("You are now registered with Titan Bot!")

@bot.command()
async def deposit(ctx, amount: float):
    await ctx.send(f"Deposited {amount} into your Titan account!")

@bot.command()
async def withdraw(ctx, amount: float):
    await ctx.send(f"Withdrew {amount} from your Titan account!")

@bot.command()
async def meme(ctx):
    await ctx.send("Here's a meme for you! [Meme URL]")

bot.run(TOKEN)
