import disnake
from disnake.ext import commands

intents = disnake.Intents.all()
bot = commands.Bot(command_prefix+"!", intents=intents)

@bot.event
async def on_ready():
    print("Bot is ready")

@bot.command()
async def pang(ctx):
    await ctx.send("Pong!")

    bot.run("MTIzNTE3NzQ5MTA0NDM3MjUyMA.G4bXTk.x89E1UBKCLlpJXyonOmOLiGvdtmNowqV3G-d1s")
