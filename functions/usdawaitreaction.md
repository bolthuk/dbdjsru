---
description: Ожидание реакции пользователя на сообщение
---

# $awaitReaction



#### Поля

Эта функция имеет 5 обязательных полей

1. userFilter \(обязательно\)
2. time \(обязательно\)
3. bot message \(обязательно\)
4. reaction \(обязательно\)
5. awaitedCommand \(обязательно\)
6. error \(необязательно\)
7. deleteMessageUponReact \(Необязательно\)

Пример использования: `$awaitReaction[userFilter;time;bot message;reaction1,reaction2,...;awaitedCommand1,awaitedCommand2,...;error message;deleteMessageUponReact (yes/no) (optional)]`

#### Options

* userFilter - Используй everyone или userID что бы указать кто может реагировать
* time - Время через которое реакция будет неактивна
* bot message - Сообщение которое отправит бот
* reaction - Реакция, при которой будет выполняться awaitedCommand.
* awaitedCommand - Имя awaitedCommand, которое будет выполнено
* error - Сообщение, когда время истекает
* deleteMessageUponReact - Когда кто-то отреагирует, он удалит &lt;сообщение бота&gt;

#### Usage

```javascript
bot.command({
name: "test",
code: `$awaitReaction[$authorID;1m;Реагируй на 1️⃣ и я отвечу;1️⃣;reactionMessage;Время закончилось] !
`
}) //Это выполнит ожидаемую команду, если пользователь отреагирует. 

bot.awaitedCommand({
name: "reactionMessage",
code: `Hi, You reacted to 1️⃣ and now i responded!`
}) //Это сообщение бота когда пользователь отреагирует
```

{% hint style="warning" %}
The error message will respond if the time has ran out \(If user doesn't do anything\)
{% endhint %}

Временные суффиксы:

* s - секунды
* m - минуты
* h - часы
* d - дни
* w - недели

{% hint style="info" %}
При наличии нескольких слотов  убедитесь, что у вас одинаковое количество awaitedCommands.
{% endhint %}

