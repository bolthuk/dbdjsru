# bot.loopCommand

```javascript
bot.loopCommand({
code: `
...
`,
channel: "channel id",
executeOnStartup: true/false,
every: ms
})
```

Использование:

```javascript
bot.loopCommand({
code: `
привет
`,
channel: "804505461076131840",
executeOnStartup: true,
every: 500000
})

/*
Эта команда будет посылать "привет" на данный идентификатор канала каждые 5 минут. 
ExecuteOnStartup означает, что когда бот запускается/выходит в Сеть, цикл запускается
*/
```

