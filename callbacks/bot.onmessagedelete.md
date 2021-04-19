---
description: Данный вызов срабатывает каждый раз при удалении сообщения
---

# bot.onMessageDelete

```javascript
bot.deletedCommand({ //Команда
channel: "channel", //Канал где была включена музыка
code: `твой код` //Код
})
bot.onMessageDelete() //обратный вызов
```

Пример использования

```javascript
bot.deletedCommand({
    channel: "782446718704812032",
    code: `Сообщение от $username, было удалено в <#$channelUsed>: $message`
    /*
        Разъяснение
        $username - Пользователь который написал сообщение
        $channelUsed - Канал где сообщение было удалено
        $message - Содержимое сообщения
    */
})
bot.onMessageDelete()
```

