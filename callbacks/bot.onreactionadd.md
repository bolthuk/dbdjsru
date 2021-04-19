---
description: >-
  Этот обратный вызов позволит боту каждый писать сообщение, когда пользователь
  реагирует на сообщение
---

# bot.onReactionAdd



```javascript
bot.reactionAddCommand({ 
        channel: "channel id", 
        code: `your code`
})
Bot.onReactionAdd()
```

Использование

```javascript
bot.reactionAddCommand({
        channel: "772414449839636490", 
        code: `$username поставил реакцию $emojiToString`
        /*        Code Breakdown
        $username - пользователь который поставил
        $emojiToString - Эмодзи которое он поставл
        */
})
bot.onReactionAdd()
```

{% hint style="info" %}
Чтобы бот не срабатывал каждый раз. Вы можете использовать $onlyForChannels, к примеру
{% endhint %}

