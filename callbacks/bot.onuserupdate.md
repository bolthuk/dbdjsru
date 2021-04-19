---
description: Срабатывает каждый раз когда пользователь обновляет профиль
---

# bot.onUserUpdate

```javascript
bot.userUpdateCommand({ //command
        channel: "channel id",
        code: `your code`
})
bot.onUserUpdate()
```

```javascript
bot.userUpdateCommand({ 
        channel: "772414449839636490", 
        code: `$username обновил свой аватар
        $oldUser[avatar]`
        })
bot.onUserUpdate()
```

