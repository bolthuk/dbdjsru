---
description: Данный вызов срабатывает каждый раз при создании нового канала на сервере
---

# bot.onChannelCreate

```text
bot.channelCreateCommand({ //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
Bot.onChannelCreate() //Обратный вызов
```

```text
bot.channelCreateCommand({ 
        channel: "772414449839636490", 
        code: `Канал создан:
        $newChannel[name]`
        })
Bot.onChannelCreate()
```

