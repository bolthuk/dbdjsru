---
description: Срабатывает когда пользователь выходит с сервера
---

# bot.onLeave

```javascript
bot.leaveCommand({ //команда
        channel: "channel id", //канал для логов
        code: `your code` //будет отправлено в указанный канал
})
bot.onLeave() //обратный вызов
```

{% hint style="danger" %}
Убедитесь, что &lt;канал&gt; находится на сервере. Поэтому рекомендуется использовать серверные переменные \(если ваш бот не предназначен для 1 сервера\)
{% endhint %}

```javascript
bot.leaveCommand({ 
        channel: "782446718704812032", 
        code: `Прощай, $username, ждём тебя снова на $serverName`
        /*
                Разъяснение
        $serverName - пользователь который вышел
        $username - Сервер
        */
})
bot.onLeave() 
```

