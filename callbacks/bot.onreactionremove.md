---
description: >-
  Этот обратный вызов пишет каждый раз, когда пользователь не реагирует на
  сообщение
---

# bot.onReactionRemove

```javascript
bot.reactionRemoveCommand({
        channel: "channel id",
        code: `your code`
})
bot.onReactionRemove()
```

Using the callback

```javascript
bot.reactionRemoveCommand({
        channel: "772414449839636490", 
        code: `$username убрал реакцию $emojiToString`
/*         Code Breakdown
$username - Пользователь который поставил реакцию
$emojiToString - Эмодзи которое убрал пользователь
*/
}) 
bot.onReactionRemove()
```

{% hint style="info" %}
Чтобы бот не срабатывал каждый раз. Вы можете использовать $onlyForChannels, к примеру
{% endhint %}

