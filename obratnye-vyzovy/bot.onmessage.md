---
description: >-
  Данный вызов отвечает за работу команд бота. Вы не можете использовать его как
  систему xp. Вместо этого используйте $alwaysExecute
---

# bot.onMessage

```javascript
const dbd = require("dbd.js") //включает работу dbd.js

const bot = new dbd.Bot({ //делает новый клиент бота
token: "token", 
prefix: "prefix"
})

bot.onMessage() //включает создание команд
```

Это позволит запускать все команды и обратные вызовы \(bot.command, bot.UpdateCommand и т.д.\)

Эй, а ты знал, что можно разрешить командам работать в Личных Сообщениях? Просто сделай это

```javascript
const dbd = require("dbd.js") //включает работу dbd.js

const bot = new dbd.Bot({ //делает новый клиент бота
token: "token", 
prefix: "prefix"
})

bot.onMessage({
  guildOnly: false //Включает возможность запуска команд из личных сообщений
})
```

{% hint style="danger" %}
bot.onMessage\(\) необходим для того, чтобы ваш бот работал
{% endhint %}

