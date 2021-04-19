---
description: >-
  Эта команда срабатывает всякий раз, когда начинает играть новая песня. Вы
  можете использовать $songInfo в коде
---

# bot.musicStartCommand

Шаблон:

    bot.musicStartCommand({ //Command
    channel: "channel", //Channel where the logs are going
    code: `your code` //Code
    })

Пример использования:

```javascript
bot.musicStartCommand({ 
channel: "$channelID", 
code: `Началось проигрывание: $songInfo[title]` 
})
/*
$channelID канал из которого началось воспроизведение
*/
```





