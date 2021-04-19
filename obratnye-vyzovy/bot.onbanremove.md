---
description: Этот обратный вызов позволяет боту логировать каждый снятый бан
---

# bot.onBanRemove

```text
bot.banRemoveCommand({ //команда
channel: "channel id", //канал для логирования
code: `код` //код
})
bot.onBanRemove() //обратный вызов
```

Использование:

```text
bot.banRemoveCommand({ 
channel: "772414449839636490",
code: `$username был разбанен на $serverName`
})
/*    Разъяснение
$username - Пользователь которого разбанили
$serverName - Сервер на котором разбанен
*/
bot.onBanRemove()
```

Если вы используете Переменные для канала логов:

```text
bot.banRemoveCommand({ 
channel: "$getServerVar[variable]", //Используйте getServerVar для получения канала логов (Устанавливается отдельно)
code: `$username без разбанен на $serverName`
})
bot.onBanRemove()
```

