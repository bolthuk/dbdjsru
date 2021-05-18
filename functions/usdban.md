---
description: Позволяет выдать бан пользователю по айди
---

# $ban

#### Поля

Эта функция имеет 3 поля - 1 обязательная и 2 дополнительных.

1. User ID.
2. Reason \(Необязательно\)
3. MessagesToDelete\(В днях, необязательно\)

Пример использования: `$ban[userID;reason (Optional);MessagesToDelete (Optional)`

#### Опции

* UserID - Пользователь которого бот забанит
* Reason - Причина в журнале аудита
* MessagesToDelete - Удаляет сообщения пользователя за столько дней за сколько укажете

#### Использование

```javascript
bot.command({
    name: "ban",
    code: `
    $username[$message] был забанен на сервере.
    $ban[$message]
    $argsCheck[1;Введите ID пользователя которого хотите забанить]
    `
});
```

{% hint style="danger" %}
`Мы рекомендуем добавить:  
$onlyPerms[ban;Вы не имеете право на бан]` в код!

Это даст использовать команду только тем кто имеет право на бан
{% endhint %}

Пример кода с `$onlyPerms[]`:

```javascript
bot.command({
    name: "ban",
    code: `
    $username[$message] был забанен на сервере.
    $ban[$message]
    $argsCheck[1;Введите ID пользователя которого хотите забанить]
    $onlyPerms[ban;Эту команду могут использовать только те кто имеет право бана]
    `
});
```

