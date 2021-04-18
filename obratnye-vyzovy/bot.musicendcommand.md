---
description: 'Эта команда срабатывает всякий раз, когда очередь заканчивается'
---

# bot.musicEndCommand

Шаблон:

    bot.musicEndCommand({ //Команда
    channel: "channel", //Канал где была включена музыка
    code: `твой код` //Код
    })

Пример использования:

```bash
bot.musicEndCommand({ 
channel: "$channelID", 
code: `Очередь закончена` 
})
/*
$channelID канал в котором был произведён процесс включения музыки
*/
```



