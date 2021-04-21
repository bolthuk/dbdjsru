---
description: >-
  Эта функция заставит бота отвечать, когда пользователь ставит реакцию на
  команду (например: !test)
---

# $awaitCmdReaction

#### Поля

Данная функция имеет 5 полей

1. userFilter \(обязательно\)
2. time \(обязательно\)
3. bot message \(обязательно\)
4. reaction \(обязательно\)
5. awaitedCommand \(обязательно\)
6. error \(необязательно\)

Пример использования: `$awaitCmdReaction[userFilter;time;bot message;reaction1,reaction2,...;awaitedCommand1,awaitedCommand2,...;error message (optional)]`

#### Options

* userFilter - Используй everyone или userID что бы указать кто может реагировать
* time - Время через которое реакция будет неактивна
* bot message - Сообщение которое отправит бот
* reaction - Реакция, при которой будет выполняться awaitedCommand.
* awaitedCommand - Имя awaitedCommand, которое будет выполнено
* error - Сообщение, когда время истекает

#### Usage

```javascript
bot.command({
name: "test",
code: `$awaitCmdReaction[$authorID;1m;Реагируй на 1️⃣ и я отвечу;1️⃣;reactionMessage;Время закончилось] !
`
}) // Это выполнит ожидаемую команду, если пользователь отреагирует. 

bot.awaitedCommand({
name: "reactionMessage",
code: `Привет, ты отреагировал на 1️⃣ и я ответил!`
}) //Это сообщение бота когда пользователь отреагирует
```

#### Suffixes

* s - секунды
* m - минуты
* h - часы
* d - дни
* w - недели

