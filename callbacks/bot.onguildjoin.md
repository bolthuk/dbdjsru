---
description: Данный вызов срабатывает каждый раз при добавлении бота на сервер
---

# bot.onGuildJoin

```text
bot.botJoinCommand({ //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onGuildJoin()//обратный вызов
```

Использование:

```text
bot.botJoinCommand({
    channel: "772414449839636490",
    code: `Я зашёл на $serverName!`
    /*
        Разъяснение
        $serverName - Сервер куда был добавлен бот
    */
})
bot.onGuildJoin()
```

Вы также можете отправить его на сервер, где он присоединился, используя $systemChannelID

```text
bot.botJoinCommand({
    channel: "$systemChannelID",
    code: `Привет, я отличный бот.`
 
})
bot.onGuildJoin()
```

{% hint style="danger" %}
WARNING: Не все серверы имеют системный канал
{% endhint %}



