---
description: Этот обратный вызов позволяет боту логировать каждый выданный бан
---

# bot.onBanAdd

    bot.banAddCommand({ //команда
    channel: "channel id", //канал куда будет писать бот при выдаче бана
    code: `код` // код
    })
    bot.onBanAdd() //обратка

Использование:



```bash
bot.banAddCommand({
channel: "772414449839636490",
code: `$username забанен на $serverName`
})
/*    Объяснение
$username - Пользователь который получил бан
$serverName - Сервер на котором получен бан
*/
bot.onBanAdd()
```

Если ваш сервер имеет Переменную для канала логов:

```bash
bot.banAddCommand({ 
channel: "$getServerVar[variable]", // Используйте getServerVar для получения канала для логов(Он устанвливается отдельно)
code: `$username забанен на $serverName`
})
bot.onBanAdd()
```

