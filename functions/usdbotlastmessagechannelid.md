---
description: Возвращает ID канала где бот последний раз отправил сообщение
---

# $botLastMessageChannelID

#### Использование

```javascript
bot.command({
    name: "id",
    code: `
Моё последнее сообщение было отправлено <#$botLastMessageChannelID>
    `
})
```

