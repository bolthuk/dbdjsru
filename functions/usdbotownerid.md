---
description: Возвращает ID создателя бота
---

# $botOwnerID

#### Поля <a id="fields"></a>

Эта функция имеет 1 необязательное поле

1. Separator \(Необязательно\)

Пример использования: `$botOwnerID[separator (optional)`

#### Опции <a id="options"></a>

* Separator - Символ/буква, разделяющая 2 или более идентификаторов \(если у бота 2 или более владельцев\)

#### Использование <a id="usage"></a>

```javascript
bot.command({
name: "botOwner",
code: `Here are my owners: $botOwnerID`
})
```

