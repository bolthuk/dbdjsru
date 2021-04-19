---
description: Срабатывает каждый раз при изменении роли
---

# Bot.onRoleUpdate

```javascript
bot.roleUpdateCommand({
        channel: "channel ID",
        code: `your code`
        })
Bot.onRoleUpdate()
```

```javascript
bot.roleUpdateCommand({ 
        channel: "772414449839636490", 
        code: `Имя роли изменено:
        Старое название: $oldRole[name]
        Новое название: $newRole[name]`
        })
Bot.onRoleUpdate()
```

