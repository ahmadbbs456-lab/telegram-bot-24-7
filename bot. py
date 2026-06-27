import os
import telebot

TOKEN = os.environ['BOT_TOKEN']
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Салом! Ман боти шумо ҳастам. Тайёр ба кор 💪")

@bot.message_handler(func=lambda message: True)
def echo_all(message):
    bot.reply_to(message, f"Ман медонам ту саволои духӯро зиёд медӣ, хамин ҳел бош 😄")

print("Bot is running...")
bot.polling()
