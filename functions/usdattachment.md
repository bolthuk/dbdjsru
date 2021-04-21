---
description: Приложить файл к сообщению
---

# $attachment

#### Поля

Эта функция имеет 1 поле

1. URL \(Обязательно\)

Пример использования: `$attachment[url]`

#### Опции

* URL - Ссылка на фото\гиф\видео которое отправит бот.

#### Usage

```javascript
bot.command({
    name: "dog",
    code: `$attachment[https://cdn.discordapp.com/attachments/773357374328012840/780585674541105152/20201116_133035.jpg] возьми фотографию собаки!`
});
```

