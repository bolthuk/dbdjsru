---
description: Эта функция реагирует на каждое отправленное сообщение
---

# $alwaysExecute

{% hint style="danger" %}
Используйте эту функцию с умом
{% endhint %}

#### Usage

```javascript
bot.command({
name: "$alwaysExecute", //ставим так что бы бот начал реагировать на все сообщения
code: `your code here` //Код который будет активироваться
})
```

Теперь, сделаем счётчик сообщений

```javascript
bot.variables({
messages: 0 //делаем переменную
})
bot.command({
name: "$alwaysExecute", 
code: `$setVar[messages;$sum[$getVar[messages];1]]` //Будет считать все отправленные сообщения
})
```

{% hint style="danger" %}
Используя данную функцию бот может иметь большой пинг
{% endhint %}

