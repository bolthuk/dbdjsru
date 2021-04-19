---
description: Данный вызов срабатывает каждый раз при обновлении пользователя
---

# bot.onMemberUpdate

```text
bot.memberUpdateCommand({  //Команда
        channel: "channel ID", //Канал для логов
        code: `код` //Код который высылается в <канал>
        })
bot.onMemberUpdate()//обратный вызов
```

Пример:

```text
bot.memberUpdateCommand({ 
        channel: "772414449839636490", 
        code: `$newMember[name] права были изменены 
        $oldMember[permissions] на $newMember[permissions]`
        })
bot.onMemberUpdate()
```



#### Свойства для $newMember & $oldMember

*  `id` - ID пользователя
* `name` - Имя пользователя 
* `guildID` - ID сервера где был изменён пользователь 
* `nick` - Никнейм если был изменён 
* `roles` - Роли если были изменены 
* `partial` - Н/Д
* `premiumStamp` - Дата бустинга сервера. 0 значит что он не бустил
* `joinedStamp` - Дата входа на сервер 
* `voiceID` - ID голосового канала если он туда зашёл 
* `displayHex` - Возвращает HEX \(Цвет\) роли которой отображается в списке пользователей 
* `highestRoleID` - ID высшей роли 
* `permissions` - Права пользователя 
* `bannable` - Можно ли банить 
* `kickable` - Можно ли кикать 
* `manageable` - Если можно изменять пользователя 
* `displayColor` - Возвращает цвет роли которой отображается в списке пользователей 
* `status` - Статус пользователя 
* `activities` - Активность пользователя

