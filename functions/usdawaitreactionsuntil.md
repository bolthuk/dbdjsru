---
description: >-
  Эта функция заставит бота отвечать, когда пользователь реагирует с заданным
  смайликом в определенном количестве реакций.
---

# $awaitReactionsUntil



#### Fields

Эта функция имеет 7 обязательных полей

Channel ID \(Required\)

1.  Channel ID \(обязательно\)
2. Message ID \(обязательно\)
3. User Filter \(обязательно\)
4. Time \(обязательно\)
5. Reaction\(s\) \(обязательно\)
6. Count\(s\) \(обязательно\)
7. Awaited Command\(s\) \(обязательно\)
8. Error \(необязательно\)

Пример Использования: `$awaitReactionsUntil[channelID;messageID;userFilter;time;reaction1,reaction2,...;count1;count2;...awaitedCommand1,awaitedCommand2,...;error message (optional)]`

#### Опции

* Channel ID - Канал где находится сообщение
* Message ID - Сообщение
* User Filter - Может использовать everyone или userID
* Time - Время на реакцию
* Reaction\(s\) - Реакция или несколько реакций
* Count\(s\) - кол-во необходимых реакций
* Awaited Command\(s\) - Команда которая будет выполнена
* Error - Сообщение при окончании времени

#### Usage

```javascript
bot.command({
name: "test",
code: `$awaitReaction[804505335397744650;826583338634182656;everyone;1m;1️⃣;5;reactionMessage;Время кончилось] !
`
}) //Это выполнит команду

bot.awaitedCommand({
name: "reactionMessage",
code: `Вау, 1️⃣ получил 5 реакций`
}) //Команда которая набрала 5 реакций
```

#### Suffixes

* s - секунда
* m - минута
* h - чат
* d - день
* w - неделя

