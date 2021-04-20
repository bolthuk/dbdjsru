---
description: Эта функция возвращает число каналов боте
---

# $allChannelsCount

## Использование

У данной функции имеется одна подфункция

1. Type \(Необязательно\)

Пример использования: `$allChannelsCount[type (Необязательно)]`

#### Типы

* text - Текстовые каналы
* voice - Голосовые каналы
* category - Категории

#### Usage

```javascript
bot.command({
name: "channelCount",
code: `
$allChannelsCount каналов всего
  - $allChannelsCount[category] категории
    - $allChannelsCount[text] текстовые каналы
    - $allChannelsCount[voice] голосовые каналы`
})
```

