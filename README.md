<h1 align="center"> 
    ✨ Aideen Smart Group Manager ✨ 
</h1>

<h3 align="center"> 
    An AI-Powered Telegram Group Manager Bot + Userbot Written In Python Using Pyrogram.
</h3>

<p align="center">
    <a href="https://python.org">
        <img src="http://forthebadge.com/images/badges/made-with-python.svg" alt="made-with-python">
    </a>
    <a href="https://GitHub.com/TheHamkerCat">
        <img src="http://ForTheBadge.com/images/badges/built-with-love.svg" alt="built-with-love">
    </a> <br>
    <img src="https://img.shields.io/github/license/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="LICENSE">
    <img src="https://img.shields.io/github/contributors/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="Contributors">
    <img src="https://img.shields.io/github/repo-size/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="Repository Size"> <br>
    <img src="https://img.shields.io/badge/python-3.9-green?style=for-the-badge&logo=appveyor" alt="Python Version">
    <img src="https://img.shields.io/github/issues/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="Issues">
    <img src="https://img.shields.io/github/forks/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="Forks">
    <img src="https://img.shields.io/github/stars/thehamkercat/AideenSmartGroupManager?style=for-the-badge&logo=appveyor" alt="Stars">
</p>

<h3 align="center"> 
    Ready to use method
</h3>

<p align="center">
    A Support Group and ready-to-use running instance of this bot can be found on Telegram <br>
    <a href="https://t.me/AideenSmartGroupManager"> Aideen Smart Group Manager </a> | 
    <a href="https://t.me/ASGMSupport"> ASGMSupport </a>
</p>

<h2 align="center"> 
   ⇝ Requirements ⇜
</h2>

<p align="center">
    <a href="https://www.python.org/downloads/release/python-390/"> Python3.9 </a> |
    <a href="https://docs.pyrogram.org/intro/setup#api-keys"> Telegram API Key </a> |
    <a href="https://t.me/botfather"> Telegram Bot Token </a> | 
    <a href="https://telegra.ph/How-To-get-Mongodb-URI-04-06"> MongoDB URI </a>
</p>

<h2 align="center"> 
   ⇝ Install Locally Or On A VPS ⇜
</h2>

```console
thehamkercat@arch:~$ git clone https://github.com/thehamkercat/AideenSmartGroupManager
thehamkercat@arch:~$ cd AideenSmartGroupManager
thehamkercat@arch:~$ pip3 install -U -r requirements.txt
thehamkercat@arch:~$ cp sample_config.py config.py
```
 
<h3 align="center"> 
    Edit <b>config.py</b> with your own values
</h3>

<h2 align="center"> 
   ⇝ Run Directly ⇜
</h2>

```console
thehamkercat@arch:~$ python3 -m asgm
```

<h3 align="center"> 
   Generating Pyrogram Session For Heroku
</h3>

```console
thehamkercat@arch:~$ git clone https://github.com/thehamkercat/AideenSmartGroupManager
thehamkercat@arch:~$ cd AideenSmartGroupManager
thehamkercat@arch:~$ pip3 install pyrogram TgCrypto
thehamkercat@arch:~$ python3 str_gen.py
```

<h1 align="center"> 
   ⇝ Docker ⇜
</h1>

```console
thehamkercat@arch:~$ git clone https://github.com/thehamkercat/AideenSmartGroupManager
thehamkercat@arch:~$ cd AideenSmartGroupManager
thehamkercat@arch:~$ cp sample_config.env config.env
```

<h3 align="center"> 
    Edit <b> config.env </b> with your own values
</h3>

```console
thehamkercat@arch:~$ sudo docker build . -t asgm
thehamkercat@arch:~$ sudo docker run asgm
```

<h2 align="center"> 
   ⇝ Write new modules ⇜
</h2>

```py
# Add license text here, get it from below

from asgm import app # This is bot's client
from asgm import app2 # userbot client, import it if module is related to userbot
from pyrogram import filters # pyrogram filters
...


# For /help menu
__MODULE__ = "Module Name"
__HELP__ = "Module help message"


@app.on_message(filters.command("start"))
async def some_function(_, message):
    await message.reply_text("I'm already up!!")

# Many useful functions are in, asgm/utils/, asgm, and asgm/core/
```

### Enhanced Description

Aideen Smart Group Manager (ASGM) is a cutting-edge, AI-powered Telegram bot designed to revolutionize the way communities interact and are managed on the platform. Built using Python and leveraging the Pyrogram library, ASGM goes beyond traditional group management tasks such as moderation, welcome messages, and user verification. It introduces intelligent interaction capabilities, enabling it to engage with community members in a more personalized and dynamic manner.

The AI component of ASGM is designed to understand and respond to user queries, facilitate discussions by prompting engaging topics, and even mediate conflicts within the community by detecting and addressing negative behaviors. This not only enhances the overall user experience but also significantly reduces the workload on human administrators by automating routine tasks and interactions.

Whether you're running a small community group or managing a large online gathering, Aideen Smart Group Manager stands ready to assist. It is constantly learning and evolving, promising to bring a new level of intelligence and efficiency to Telegram group management.


<h3 align="center"> 
   And put that file in wbb/modules/, restart and test your bot.
</h3>
