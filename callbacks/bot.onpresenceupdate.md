---
description: Срабатывает при обновлении статуса какого либо пользователя
---

# bot.onPresenceUpdate

```javascript
bot.presenceUpdateCommand({ 
        channel: "channel id", 
        code: `your code`
})
Bot.onPresenceUpdate()
```

```javascript
bot.presenceUpdateCommand({ 
        channel: "782446718704812032",
        code: `$username обновил свой статус!
        Старый статус: $oldPresence[status]` 
        })
Bot.onPresenceUpdate()
```

