---
description: >-
  Эта функция позволяет вам добавить «автора» к встроенному сообщению и значок
  автору, если указан URL-адрес.
---

# $author

#### Поля

Отвечая на ваш вопрос, `$author[]` имеет 3 поля.

1. text.
2. icon URL.
3. Hyper link \(Необязательно\)

Пример использования: `$author[text;icon url;url (optional)]`

#### Options

* Text - Автор текста
* icon URL - Ссылка на изображение для текста
* HyperLink URL - Ссылка на сайт\фото и т.д.

{% hint style="warning" %}
Ссылка должна оканчиваться только на `.gif`, `.png или .jpg`
{% endhint %}

#### Использование

```javascript
bot.command({
    name: "embed",
    code: `$author[Это пример;$authorAvatar]`
});

//используя гипер ссылку

bot.command({
    name: "embed",
    code: `$author[DBD.js;$serverIcon;https://dbd.js.org]`
});
```

