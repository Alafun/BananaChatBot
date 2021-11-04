# BananaChatBot
 Task for NLP class. 



## Intro for program



## Slide MindMap

### Background

1. Q&A robot
2. [CU GAME](https://www.bilibili.com/video/BV1L44y147zC)

### DEMO Code

Telegram or Dingding Chat Bot

#### NLPLover commends list

```shell
start - Let's start chat.
hello - Say "Hi! "
keeprunning - Change to cheer mode. 
help - Ask bot for help.
```

#### NLPLover code

Buffer code(copy):

```python
# # import job
# import os
# import telebot
# from telebot import custom_filters
# # import random

# #define job
# API_KEY = os.getenv('API_KEY')
# bot = telebot.TeleBot(API_KEY)


# # Check if message starts with @LYB tag
# @bot.message_handler(text_startswith="@卢源斌")
# def start_filter(message):
#     bot.send_message(message.chat.id,
#                      "Looks like you are calling 卢源斌, wait...")


# # Check if text is hi or hello
# @bot.message_handler(text_contains=['不跑', '累', '好多', '跑不'])
# def keep_running_filter(message):
#     bot.send_message(
#         message.chat.id,
#         "加油啊, {name}!".format(name=message.from_user.first_name + ' ' +
#                               message.from_user.last_name))


# # words=["加油","别放弃","继续跑","你可是年轻人","要不再跑几公里试试？","Come~On~","卢源斌好帅（超大声）"]

# # Do not forget to register filters
# # bot.add_custom_filter(custom_filters.TextMatchFilter())
# bot.add_custom_filter(custom_filters.TextStartsFilter())
# bot.add_custom_filter(custom_filters.TextContainsFilter())

# bot.infinity_polling()


# import job
import os
import telebot
from telebot import custom_filters

#define job
API_KEY = os.getenv('API_KEY')
bot = telebot.TeleBot(API_KEY)

# Check if message starts with @admin tag
@bot.message_handler(text_startswith="@admin")
def start_filter(message):
    bot.send_message(message.chat.id, "Looks like you are calling admin, wait...")

# Check if text is hi or hello
@bot.message_handler(text=['hi','hello'])
def text_filter(message):
    bot.send_message(message.chat.id, "Hi, {name}!".format(name=message.from_user.first_name))

@bot.message_handler(text_contains=['不跑', '累', '好多', '跑不'])
def keep_running_filter(message):
    bot.send_message(
        message.chat.id,
        "加油啊, {name}!".format(name=message.from_user.first_name + ' ' +
                              message.from_user.last_name))

# Do not forget to register filters
bot.add_custom_filter(custom_filters.TextMatchFilter())
bot.add_custom_filter(custom_filters.TextStartsFilter())
bot.add_custom_filter(custom_filters.TextContainsFilter())

bot.infinity_polling()

```

Result code(mine)

```python
# import job
import os
import telebot
from telebot import custom_filters
import random
#define job
API_KEY = os.getenv('API_KEY')
bot = telebot.TeleBot(API_KEY)

# Check if message starts with @LYB tag
@bot.message_handler(text_startswith="@卢源斌")
def start_filter(message):
    bot.send_message(message.chat.id, "Looks like you are calling 卢源斌, wait...")

# Check if text is hi or hello
@bot.message_handler(text_contains=['不跑','累','好多','跑不'])
def keep_running_filter(message):
    bot.send_message(message.chat.id, "加油啊, {name}!".format(name=message.from_user.first_name+' '+message.from_user.last_name))

# words=["加油","别放弃","继续跑","你可是年轻人","要不再跑几公里试试？","Come~On~","卢源斌好帅（超大声）"]


# Do not forget to register filters
# bot.add_custom_filter(custom_filters.TextMatchFilter())
bot.add_custom_filter(custom_filters.TextStartsFilter())
bot.add_custom_filter(custom_filters.TextContainsFilter())

bot.infinity_polling()
```



## Ref link: 

1. https://github.com/nlpinaction/learning-nlp
   1. https://github.com/nlpinaction/learning-nlp/tree/master/chapter-10/seq2seq

2. https://blog.csdn.net/daniellibin/article/details/103290169
3. http://www.lcsays.com/tags/%E8%87%AA%E5%B7%B1%E5%8A%A8%E6%89%8B%E5%81%9A%E8%81%8A%E5%A4%A9%E6%9C%BA%E5%99%A8%E4%BA%BA/

## Ref book:

1. 《Python聊天机器人开发 基于自然语言处理与机器学习》 【印】Sumit Raj
