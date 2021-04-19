# $addMessageReactions

Данная функция позволяет добавлять реакции на сообщение по ID

#### Функции

Эта функция имеет 3 обязательных функций

1. Channel ID \(Обязательно\)
2. Message ID \(Обязательно\)
3. Reaction \(Обязательно\)
4. Reaction 2 \(Необязательно\)
5. и т.д.

Пример использования: `$addMessageReactions[Channel ID;Message ID;Reaction 1;Reaction 2,...]`

#### Опции

* Channel ID - Канал где находится нужное сообщение &lt;messageID&gt; 
* Message ID - Нужное сообщение куда надо поставить реакцию
* Reaction - Эмоция которая будет поставлена на сообщение &lt;message&gt;

#### Использование

Одиночная реакция

```javascript
bot.command({
    name: "react",
    code: `
    $addMessageReactions[$channelID;$messageID;🌸]
    Здесь красивый цветок
    `
});
```

Несколько реакций

```javascript
bot.command({
    name: "question",
    code: `
    $addMessageReactions[$channelID;$messageID;✔;❌]
    `
});
```

