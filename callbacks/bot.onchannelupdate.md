---
description: Данный вызов срабатывает каждый раз при обновлении канала на сервере
---

# bot.onChannelUpdate

```text
bot.channelUpdateCommand({ //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
Bot.onChannelUpdate() //Обратный вызов
```

```text
bot.channelUpdateCommand({ 
        channel: "772414449839636490", 
        code: `Имя канала изменено
        Старое имя: $oldChannel[name]
        Новое имя: $newChannel[name]`
        })
Bot.onChannelUpdate()
```

