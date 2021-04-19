---
description: Данный вызов срабатывает каждый раз при удаление бота с сервера
---

# bot.onGuildLeave

```text
bot.botLeaveCommand({ //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onGuildLeave()//обратный вызов
```

Использование:

```text
bot.botLeaveCommand({
    channel: "772414449839636490",
    code: `Я вышел с $serverName!`
    /*
        Разъяснение
        $serverName - сервер с которого удалён бот
    */
})
bot.onGuildLeave()
```

