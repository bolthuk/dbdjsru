---
description: Данный вызов срабатывает каждый раз при удалении канала на сервере
---

# bot.onChannelDelete

```text
bot.channelDeleteCommand({ //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
Bot.onChannelDelete() //Обратный вызов
```

```text
bot.channelDeleteCommand({ 
        channel: "772414449839636490", 
        code: `Канал удалён:
        $oldChannel[name]`
        })
Bot.onChannelDelete()
```

