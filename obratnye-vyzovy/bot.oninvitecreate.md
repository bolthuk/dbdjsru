---
description: Данный вызов срабатывает каждый раз при создании приглашения
---

# bot.onInviteCreate

```text
bot.inviteCreateCommand({  //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onInviteCreate() //обратный вызов
```

Использование:

```text
bot.inviteCreateCommand({
    channel: '772414449839636490',
    code: `Информация о приглашении:
    Создал: $inviteUserID
    Ссылка: $inviteURL
    Канал где создан: $inviteChannelID
    `,
})
bot.onInviteCreate()
```



Вы можете использовать данные функции в коде

* $inviteUses 
* $inviteURL 
* $inviteCode 
* $inviteGuildID
* $inviteChannelID 
* $inviteUserID 
* $inviteMaxUses

