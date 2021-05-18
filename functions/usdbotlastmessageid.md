---
description: Возвращает ID последнего сообщения бота.
---

# $botLastMessageID

#### Использование

```javascript
bot.command({
    name: "id",
    code: `
ID сообщения: $loop[1;cmd]
    `
})

bot.awaitedCommand({
nme: "cmd",
code: `$botLastMessageID`
)}
```

