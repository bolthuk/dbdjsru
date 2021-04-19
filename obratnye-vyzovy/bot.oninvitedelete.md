---
description: Данный вызов срабатывает каждый раз при удалении приглашения
---

# bot.onInviteDelete

```text
bot.inviteDeleteCommand({  //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onInviteDelete() //обратный вызов
```

Использование:

```text
bot.inviteDeleteCommand({ 
    channel: '772414449839636490', 
    code: `Информация о приглашении:
    Создал: $inviteUserID
    Ссылка: $inviteURL
    Использовано: $inviteUses
    Канал в котором создан: $inviteChannelID
    `, 
})
bot.onInviteDelete() 
```



Вы можете использовать данные функции в коде

* $inviteUses 
* $inviteURL 
* $inviteCode 
* $inviteGuildID
* $inviteChannelID 
* $inviteUserID 
* $inviteMaxUses

