---
description: Данный вызов срабатывает каждый раз при обновлении сообщения.
---

# bot.onMessageUpdate

```javascript
bot.updateCommand({  //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onMessageUpdate() //обратный вызов
```

Пример:

```javascript
bot.updateCommand({
        channel: "782446718704812032", 
        code: `Сообщение обновлено $username в <#$channelUsed>:
$message
Старое сообщение: $oldMessage`
/*
        Разъяснение
$message - Новое сообщение
$oldMessage - Старое сообщение которое было обновлено. (Работает только в обратных вызовах)
$username - Пользователь который изменил сообщение
$channelUsed - Канал где обновлено сообщение
*/
})
bot.onMessageUpdate()
```

