# Currency_bot
The bot returns the price of a certain amount of currency (euro, dollar or ruble).
The person has to send a message to the bot in the form <name of the currency whose price they want to know> <name of the currency in which you want to know the price of the first currency> <quantity of the first currency>.
Typing /start or /help will give the user instructions on how to use the bot.
Typing /values should display all available currencies in a readable form.
The text of any error, specifying the type of error, must be sent to the user in messages.
To send requests to API, describe a class with static method get_price(), which accepts three arguments and returns the desired currency amount:
the name of the currency whose price to find out - base;
The name of the currency whose price is to be found out - quote;
the amount of currency to be converted - amount.
Also you need to create config.py with lines 
  
TOKEN = 'your bot token'

exchanges = {
    'доллар': 'USD',
    'евро': 'EUR',
    'рубль': 'RUB',
    'сум': 'UZS',
    'лира': 'TRY',
    'песо': 'ARS',
    'кдоллар': 'CAD'
}
